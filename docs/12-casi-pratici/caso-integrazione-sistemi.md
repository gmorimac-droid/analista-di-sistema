# Caso pratico: integrazione sistemi

> Simulazione reale: progettazione e analisi di un’integrazione multi-sistemi in un contesto enterprise.

---

## 🎯 Obiettivo del caso

Allenarsi a:

- analizzare un’integrazione complessa  
- identificare sistemi, flussi e dipendenze  
- gestire errori e casi limite  
- ragionare come un analista di sistema senior  

---

## 🧭 Scenario

L’azienda vende prodotti online attraverso un portale e-commerce.

Sistemi coinvolti:

- **Portale e-commerce** → ricezione ordini
- **ERP** → gestione ordini, fatturazione, anagrafiche
- **WMS** (Warehouse Management System) → gestione magazzino e spedizioni
- **CRM** → storico cliente e comunicazioni
- **Sistema notifiche** → email e messaggi automatici
- **Gateway pagamenti** → autorizzazione e conferma pagamento

---

## 📥 Esigenza di business

Il business richiede che, dopo la conferma di un ordine online, il processo sia completamente integrato e automatizzato:

1. ordine acquisito dal portale  
2. pagamento verificato  
3. ordine registrato in ERP  
4. disponibilità verificata in WMS  
5. cliente aggiornato in CRM  
6. notifica inviata al cliente  

Obiettivo:

> ridurre tempi, errori manuali e disallineamenti tra sistemi

---

## ⚠️ Attenzione iniziale

La richiesta sembra lineare, ma in realtà introduce molte domande:

- quale sistema è il master dell’ordine?
- quando un ordine è davvero “confermato”?
- cosa succede se il pagamento va a buon fine ma ERP non risponde?
- cosa succede se il magazzino non ha disponibilità?
- cosa succede se il CRM non viene aggiornato?
- la notifica al cliente parte subito o solo dopo verifica completa?

👉 Questo è il punto in cui inizia il lavoro dell’analista senior.

---

## 🧠 Fase 1: chiarimento del processo

### Domande chiave

- Quando nasce formalmente l’ordine?
- Il portale crea direttamente l’ordine o solo una prenotazione?
- Il pagamento è autorizzato o contabilizzato subito?
- L’ERP accetta ordini anche se il WMS non ha stock?
- Il CRM deve essere aggiornato in real time?
- Le notifiche dipendono dall’esito di tutti i sistemi o solo di alcuni?

---

## 🔍 Fase 2: mappatura del processo atteso

### Flusso logico desiderato

1. Il cliente conferma l’acquisto sul portale
2. Il gateway pagamenti restituisce esito
3. Il portale invia l’ordine all’ERP
4. L’ERP registra l’ordine
5. L’ERP richiede verifica disponibilità al WMS
6. Il WMS restituisce esito disponibilità
7. L’ERP aggiorna stato ordine
8. Il CRM riceve aggiornamento cliente/ordine
9. Il sistema notifiche invia conferma al cliente

---

## 🧩 Fase 3: identificazione dei sistemi master

Uno dei punti più critici è definire le responsabilità.

### Possibile distribuzione

| Oggetto | Sistema master |
|--------|----------------|
| carrello / checkout | Portale e-commerce |
| pagamento | Gateway pagamenti |
| ordine ufficiale | ERP |
| disponibilità magazzino | WMS |
| storico relazione cliente | CRM |
| comunicazioni | Sistema notifiche |

👉 Senza questa definizione, l’integrazione diventa fragile.

---

## 🔗 Fase 4: analisi delle integrazioni

### Integrazione 1 — Portale → Gateway pagamenti
- richiesta autorizzazione pagamento
- ricezione esito

### Integrazione 2 — Portale → ERP
- creazione ordine
- invio dati cliente, righe ordine, importi

### Integrazione 3 — ERP ↔ WMS
- verifica disponibilità
- allocazione stock
- aggiornamento stato preparazione/spedizione

### Integrazione 4 — ERP → CRM
- aggiornamento anagrafica / storico acquisto

### Integrazione 5 — ERP / CRM → Sistema notifiche
- trigger email conferma
- eventuali aggiornamenti successivi

👉 Non esiste “una” integrazione: esiste una **catena di integrazioni**.

---

## ⚖️ Fase 5: scelta del modello di orchestrazione

Qui entra una decisione importante.

### Opzione A — Orchestrazione centrata sul portale
Il portale coordina tutto.

**Vantaggi**
- logica centralizzata inizialmente semplice

**Svantaggi**
- portale troppo carico
- rischio accoppiamento forte
- difficile manutenzione

---

### Opzione B — Orchestrazione centrata su ERP
L’ERP diventa il punto di governo dell’ordine.

**Vantaggi**
- coerenza sul ciclo ordine
- responsabilità chiara

**Svantaggi**
- ERP più esposto
- maggiore dipendenza dal suo comportamento

---

### Opzione C — Event-driven / orchestrazione distribuita
Ogni sistema reagisce a eventi condivisi.

**Vantaggi**
- flessibilità
- maggiore scalabilità

**Svantaggi**
- maggiore complessità
- tracciamento più difficile

---

### Valutazione da analista senior

In un contesto enterprise classico, la soluzione più solida è spesso:

> **ERP come master del ciclo ordine**, con integrazioni orchestrate e responsabilità chiare.

---

## ⚠️ Fase 6: scenari di errore

Questa è la parte che distingue un’analisi superficiale da una professionale.

### Caso 1 — Pagamento OK, ERP KO
Il pagamento è autorizzato, ma l’ERP non crea l’ordine.

**Rischio**
- cliente pagante senza ordine registrato

**Possibili azioni**
- retry automatico
- stato intermedio “da riconciliare”
- alert operativo

---

### Caso 2 — ERP OK, WMS stock insufficiente
L’ordine esiste, ma il magazzino non può evaderlo.

**Rischio**
- ordine confermato ma non evadibile

**Possibili azioni**
- stato “in attesa disponibilità”
- comunicazione al cliente
- gestione parziale/backorder

---

### Caso 3 — ERP OK, CRM KO
Ordine correttamente creato, ma CRM non aggiornato.

**Rischio**
- storico cliente incompleto
- impatti su marketing e customer care

**Possibili azioni**
- asincronia con retry
- logging errore
- coda di riallineamento

---

### Caso 4 — Notifica inviata due volte
Un retry o un doppio trigger genera email duplicate.

**Rischio**
- cattiva esperienza cliente

**Possibili azioni**
- idempotenza
- tracciamento invii
- controllo duplicati

---

### Caso 5 — Timeout su integrazione
Il sistema chiamato non risponde nei tempi attesi.

**Rischio**
- blocco del flusso
- stato incerto

**Possibili azioni**
- timeout gestito
- retry limitato
- stato intermedio
- dashboard di monitoraggio

---

## 🧾 Fase 7: requisiti funzionali e non funzionali

### Requisiti funzionali principali

- il sistema deve registrare l’ordine in ERP dopo esito positivo del pagamento
- il sistema deve verificare disponibilità prodotti tramite WMS
- il sistema deve aggiornare CRM con i dati dell’acquisto
- il sistema deve inviare una notifica di conferma al cliente
- il sistema deve gestire stati intermedi in caso di errore

### Requisiti non funzionali principali

- tracciabilità end-to-end del flusso ordine
- gestione retry controllata
- logging centralizzato
- assenza di duplicazione eventi
- tempo massimo di conferma ordine definito
- resilienza in caso di indisponibilità temporanea di un sistema

---

## 📊 Fase 8: stati dell’ordine

Per evitare ambiguità, è essenziale definire gli stati.

### Esempio stati

- `IN_ATTESA_PAGAMENTO`
- `PAGAMENTO_AUTORIZZATO`
- `INVIATO_A_ERP`
- `REGISTRATO_ERP`
- `IN_VERIFICA_STOCK`
- `PRONTO_PER_EVASIONE`
- `IN_ATTESA_GESTIONE`
- `ERRORE_INTEGRAZIONE`

👉 Gli stati aiutano a governare il processo e a gestire eccezioni.

---

## 🔄 Fase 9: approccio di error handling

Un analista senior non si limita a dire “gestire l’errore”.

Deve distinguere:

### Errori temporanei
- timeout
- indisponibilità momentanea
- lentezza

**Strategia**
- retry automatico
- attesa controllata

### Errori strutturali
- dati errati
- mapping incoerenti
- chiavi mancanti

**Strategia**
- blocco del flusso
- presa in carico operativa
- correzione dati

### Errori funzionali
- prodotto non disponibile
- pagamento rifiutato

**Strategia**
- cambio stato ordine
- comunicazione al cliente

---

## 🧠 Fase 10: monitoraggio e supporto operativo

Una vera integrazione enterprise non vive solo in build time, ma in run time.

### Cosa serve monitorare

- ordini in errore
- integrazioni fallite
- retry in corso
- messaggi in coda
- notifiche duplicate
- tempi medi di attraversamento del flusso

### Output consigliati

- dashboard operativa
- report giornaliero anomalie
- log correlati per order ID

---

## 👥 Fase 11: stakeholder da coinvolgere

### Business
- regole di processo
- gestione eccezioni
- aspettative cliente

### Team ERP
- creazione ordine
- gestione stati

### Team WMS
- disponibilità e allocazione stock

### Team CRM
- aggiornamento storico cliente

### Team integrazione / middleware
- orchestrazione
- retry
- logging

### Customer care
- gestione casi anomali

### QA
- test end-to-end
- test error handling

---

## ⚠️ Errori tipici di un analista junior

- vedere solo il “flusso felice”
- non definire il sistema master
- ignorare stati intermedi
- trattare gli errori come eccezioni rare
- non coinvolgere i team corretti
- non considerare il supporto operativo

---

## 🧠 Come ragiona un analista senior

Un analista senior, davanti a questo scenario:

- scompone il processo end-to-end
- definisce responsabilità dei sistemi
- distingue flussi sincroni e asincroni
- analizza errori come parte del disegno
- pensa a stati, retry, tracciabilità e monitoraggio
- costruisce una soluzione robusta, non solo funzionante

👉 La domanda non è:

> “Come colleghiamo i sistemi?”

Ma:

> “Come garantiamo un processo affidabile anche quando qualcosa va storto?”

---

## 📌 Lezioni apprese

- le integrazioni vanno analizzate come ecosistemi
- il flusso nominale non basta
- error handling e monitoraggio fanno parte della soluzione
- i sistemi master vanno definiti chiaramente
- la resilienza è tanto importante quanto la funzionalità

---

## 🚀 In sintesi

Un’integrazione complessa richiede:

- comprensione del processo  
- definizione delle responsabilità  
- progettazione dei flussi  
- gestione degli errori  
- monitoraggio operativo  

E soprattutto:

> **pensare al comportamento reale del sistema, non solo alla connessione tra componenti**

---

## ▶️ Prossimo caso

➡️ Vai a: [Caso migrazione](caso-migrazione.md)