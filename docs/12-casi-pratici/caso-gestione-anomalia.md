# Caso pratico: gestione anomalia

> Simulazione reale: analisi e gestione di un’anomalia in produzione con impatto sul business.

---

## 🎯 Obiettivo del caso

Allenarsi a:

- gestire anomalie in produzione  
- identificare root cause  
- lavorare sotto pressione  
- coordinare stakeholder  
- ragionare come un analista senior  

---

## 🧭 Scenario

Sistema e-commerce in produzione.

Flusso principale:
- creazione ordine  
- pagamento  
- registrazione ERP  
- spedizione  

---

## 📥 Problema segnalato

Il customer care segnala:

> “Alcuni clienti hanno pagato ma non vedono l’ordine nel sistema”

---

## ⚠️ Contesto

- sistema in produzione  
- clienti impattati  
- potenziale perdita economica  
- pressione elevata  

---

## 🧠 Fase 1: gestione immediata

---

### Obiettivo

- capire l’impatto  
- stabilizzare la situazione  

---

### Azioni immediate

- raccogliere esempi concreti (order ID)  
- verificare frequenza problema  
- identificare quando è iniziato  

---

👉 Non partire subito con ipotesi tecniche

---

## 🔍 Fase 2: raccolta informazioni

---

### Dati da raccogliere

- ID ordine  
- timestamp  
- esito pagamento  
- presenza in ERP  
- log sistema  

---

### Domande chiave

- tutti gli ordini sono impattati o solo alcuni?  
- il pagamento è confermato?  
- l’ordine esiste nel portale?  
- l’ERP riceve la richiesta?  

---

## 🔗 Fase 3: analisi del flusso

---

### Flusso atteso

1. cliente paga  
2. pagamento OK  
3. ordine inviato a ERP  
4. ERP crea ordine  

---

### Punto critico

👉 dove si interrompe il flusso?

---

## 📊 Fase 4: analisi tecnica

---

### Possibili punti di rottura

---

#### 💳 Pagamento OK ma ordine non creato
→ problema tra portale e ERP  

---

#### 🔗 Chiamata API fallita
→ timeout / errore integrazione  

---

#### 🔄 Retry non gestito
→ ordine mai reinviato  

---

#### 📦 ERP riceve ma non salva
→ errore interno ERP  

---

## ⚠️ Fase 5: ipotesi

---

### Ipotesi 1
errore integrazione portale → ERP  

---

### Ipotesi 2
timeout non gestito  

---

### Ipotesi 3
errore dati (payload non valido)  

---

👉 Le ipotesi devono essere verificate, non assunte

---

## 🧪 Fase 6: verifica

---

### Analisi log

- verificare chiamate API  
- verificare errori  

---

### Confronto casi OK vs KO

- cosa cambia?  

---

### Verifica dati

- payload corretto?  

---

## 📌 Risultato (esempio)

Si scopre che:

- alcune chiamate verso ERP vanno in timeout  
- il sistema non esegue retry  
- gli ordini non vengono reinviati  

---

👉 Root cause identificata

---

## 🧠 Fase 7: gestione immediata

---

### Azioni

- recuperare ordini non registrati  
- reinviarli manualmente  
- informare customer care  

---

### Obiettivo

- ridurre impatto clienti  

---

## 🛠️ Fase 8: soluzione definitiva

---

### Interventi

- introdurre retry automatico  
- gestire timeout  
- aggiungere logging  

---

### Miglioramenti

- monitoraggio integrazione  
- alert automatici  

---

## ⚠️ Fase 9: gestione comunicazione

---

### Stakeholder

- business  
- customer care  
- IT  

---

### Comunicazione

- stato problema  
- impatto  
- azioni  

---

👉 fondamentale per mantenere fiducia

---

## 🧠 Fase 10: prevenzione

---

### Azioni preventive

- monitoraggio proattivo  
- alert  
- test di resilienza  
- gestione errori migliorata  

---

## ⚠️ Errori tipici (junior)

---

### Saltare subito alla soluzione
→ perdita tempo  

---

### Non raccogliere dati
→ analisi errata  

---

### Non considerare tutto il flusso
→ root cause mancata  

---

### Non comunicare
→ caos organizzativo  

---

## 🧠 Come ragiona un analista senior

Un analista senior:

- mantiene calma sotto pressione  
- raccoglie dati prima di agire  
- analizza end-to-end  
- valida ipotesi  
- coordina stakeholder  
- pensa anche alla prevenzione  

👉 Non risolve solo il problema, ma **migliora il sistema**

---

## 📌 Lezioni apprese

- i problemi vanno analizzati, non indovinati  
- il flusso completo è fondamentale  
- i log sono essenziali  
- la comunicazione è critica  
- ogni problema è un’opportunità di miglioramento  

---

## 🚀 In sintesi

La gestione di un’anomalia richiede:

- analisi strutturata  
- raccolta dati  
- identificazione root cause  
- gestione impatto  
- miglioramento continuo  

E soprattutto:

> **lucidità sotto pressione**

---

## ▶️ Prossimo passo

➡️ Vai a: [Crescita professionale](../13-crescita-professionale/index.md)