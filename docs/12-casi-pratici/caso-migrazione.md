# Caso pratico: migrazione sistemi

> Simulazione reale: migrazione da un sistema legacy a un nuovo sistema con gestione dati, utenti e continuità operativa.

---

## 🎯 Obiettivo del caso

Allenarsi a:

- analizzare una migrazione complessa  
- gestire dati e mapping  
- identificare rischi operativi  
- pianificare cut-over e rollback  
- ragionare come un analista senior  

---

## 🧭 Scenario

L’azienda utilizza un sistema legacy per la gestione clienti e ordini.

Caratteristiche del sistema legacy:
- dati non normalizzati  
- campi inconsistenti  
- logiche non documentate  
- integrazioni “hardcoded”  

---

### 📦 Nuovo sistema

È stato introdotto un nuovo sistema moderno con:

- modello dati strutturato  
- API standard  
- integrazioni pulite  
- maggiore scalabilità  

---

## 📥 Esigenza di business

> Migrare tutti i dati e passare al nuovo sistema senza interrompere il servizio

---

## ⚠️ Attenzione iniziale

La migrazione non è:

👉 “copiare dati da A a B”

È:

👉 **trasformare, pulire, validare e riallineare un intero ecosistema**

---

## 🧠 Fase 1: analisi del sistema legacy

---

### Domande chiave

- quali dati esistono davvero?  
- quali campi sono obbligatori?  
- quali dati sono inconsistenti?  
- quali logiche sono implicite nel sistema?  
- quali integrazioni dipendono da questi dati?  

---

### Problema reale

👉 il sistema legacy spesso è poco documentato

---

## 📊 Fase 2: analisi dei dati

---

### Tipologie di problemi

---

#### 📉 Dati incompleti
- campi null  
- informazioni mancanti  

---

#### 🔁 Dati duplicati
- clienti duplicati  
- ordini replicati  

---

#### ⚠️ Dati incoerenti
- formati diversi  
- valori non validi  

---

#### 🧩 Dati “sporchi”
- errori manuali  
- codifiche non standard  

---

👉 Prima di migrare, bisogna capire **la qualità dei dati**

---

## 🔗 Fase 3: mapping dati

---

### Obiettivo

Collegare:

> dati legacy → dati nuovo sistema

---

### Esempio

| Legacy | Nuovo sistema |
|--------|---------------|
| nome_cliente | first_name |
| cognome_cliente | last_name |
| indirizzo | address |

---

### Problemi possibili

- campi che non esistono più  
- campi nuovi non presenti nel legacy  
- differenze di struttura  

---

👉 Il mapping è uno dei punti più critici

---

## ⚠️ Fase 4: trasformazione dati

---

### Attività necessarie

- normalizzazione  
- pulizia  
- conversione formati  
- deduplicazione  

---

### Esempio

- data formato testo → data standard  
- telefono con formati diversi → formato unico  

---

## 🧠 Fase 5: strategia di migrazione

---

### Opzione 1 — Big bang

- tutto migrato in un’unica soluzione  

**Vantaggi**
- semplice concettualmente  

**Rischi**
- alto impatto  
- difficile rollback  

---

### Opzione 2 — Migrazione graduale

- migrazione per fasi  

**Vantaggi**
- rischio ridotto  

**Svantaggi**
- maggiore complessità  

---

### Opzione 3 — Parallel run

- vecchio e nuovo sistema attivi  

**Vantaggi**
- maggiore sicurezza  

**Svantaggi**
- doppia gestione  

---

👉 La scelta dipende da rischio e contesto

---

## 🔄 Fase 6: cut-over

---

### Cos’è

Il momento in cui si passa dal sistema legacy al nuovo sistema

---

### Attività

- blocco inserimento dati legacy  
- esecuzione migrazione finale  
- verifica dati  
- attivazione nuovo sistema  

---

### Rischi

- perdita dati  
- incoerenza  
- downtime  

---

## 🔙 Fase 7: rollback

---

### Domanda fondamentale

> Cosa facciamo se qualcosa va storto?

---

### Possibili strategie

- tornare al sistema legacy  
- ripristinare backup  
- correggere dati e rilanciare  

---

👉 Senza piano di rollback, il rischio è altissimo

---

## ⚠️ Fase 8: rischi principali

---

### 📉 Perdita dati
→ dati non migrati  

---

### 🔁 Duplicazioni
→ dati replicati  

---

### ⚠️ Incoerenza
→ dati non allineati  

---

### ⏱️ Downtime
→ servizio non disponibile  

---

### 👥 Impatto utenti
→ difficoltà operative  

---

## 🧪 Fase 9: test

---

### Tipologie

---

#### ✔ Test di migrazione

- verifica dati migrati  

---

#### ✔ Test funzionali

- verifica comportamento sistema  

---

#### ✔ Test integrativi

- verifica integrazioni  

---

#### ✔ Test utenti (UAT)

- validazione business  

---

## 📊 Fase 10: monitoraggio post-migrazione

---

### Cosa controllare

- errori  
- dati incoerenti  
- performance  
- segnalazioni utenti  

---

👉 La migrazione non finisce al go-live

---

## 👥 Fase 11: stakeholder

---

### Business
- validazione dati  
- accettazione  

---

### IT
- migrazione tecnica  
- integrazioni  

---

### Utenti
- utilizzo sistema  

---

### Supporto
- gestione problemi  

---

## ⚠️ Errori tipici (junior)

---

### Sottovalutare i dati
→ problemi gravi  

---

### Non testare abbastanza
→ errori in produzione  

---

### Non prevedere rollback
→ rischio elevato  

---

### Non coinvolgere utenti
→ rifiuto del sistema  

---

## 🧠 Come ragiona un analista senior

Un analista senior:

- analizza profondamente i dati  
- definisce mapping preciso  
- considera qualità dati  
- pianifica strategia di migrazione  
- definisce cut-over e rollback  
- anticipa problemi operativi  

👉 Non pensa solo alla migrazione, ma alla **continuità del business**

---

## 📌 Lezioni apprese

- i dati sono la parte più critica  
- la migrazione è un processo, non un evento  
- il rischio va gestito in modo esplicito  
- il testing è fondamentale  
- il supporto post-migrazione è essenziale  

---

## 🚀 In sintesi

Una migrazione richiede:

- analisi dati  
- mapping  
- trasformazione  
- strategia  
- gestione rischio  

E soprattutto:

> **proteggere il business durante il cambiamento**

---

## ▶️ Prossimo caso

➡️ Vai a: [Caso gestione anomalia](caso-gestione-anomalia.md)