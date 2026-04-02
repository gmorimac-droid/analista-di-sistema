# Caso pratico: richiesta evolutiva

> Simulazione reale: gestione di una richiesta evolutiva in un sistema esistente.

---

## 🎯 Obiettivo del caso

Allenarsi a:

- analizzare una richiesta reale  
- identificare impatti  
- strutturare una soluzione  
- ragionare come un analista senior  

---

## 🧭 Scenario

Sistema: piattaforma gestione ordini e-commerce

Funzionalità attuale:
- creazione ordine  
- pagamento  
- gestione stato ordine  

---

### 📥 Nuova richiesta

Il business richiede:

> “Vogliamo inviare una notifica email automatica quando un ordine viene spedito”

---

## ⚠️ Attenzione

La richiesta sembra semplice.

👉 Non lo è.

---

## 🔍 Fase 1: Comprensione della richiesta

---

### Domande chiave

- Quando esattamente viene spedito un ordine?  
- Esiste già uno stato “spedito”?  
- Chi riceve la notifica?  
- Che contenuto deve avere l’email?  
- Ci sono sistemi esterni coinvolti?  

---

👉 Un analista senior **non parte dalla soluzione**

---

## 🧠 Fase 2: Analisi del contesto

---

### Sistemi coinvolti

- sistema ordini  
- sistema logistica  
- sistema email  

---

### Flusso attuale

1. ordine creato  
2. pagamento  
3. spedizione gestita da sistema logistica  

---

### Punto critico

👉 chi “sa” che l’ordine è spedito?

---

## 🔗 Fase 3: Analisi delle integrazioni

Possibili scenari:

---

### Caso A
Il sistema ordini riceve aggiornamento stato da logistica  

---

### Caso B
Il sistema logistica gestisce direttamente lo stato  

---

👉 cambia completamente la soluzione

---

## ⚠️ Fase 4: Analisi impatti

---

### 📦 Funzionali

- nuovo trigger (spedizione)  
- nuova funzionalità (invio email)  

---

### 🔗 Tecnici

- integrazione tra sistemi  
- gestione eventi  

---

### 📊 Dati

- email cliente  
- stato ordine  

---

### 🔒 Sicurezza

- gestione dati personali  

---

### ⏱️ Operativi

- invio email affidabile  

---

## 🧱 Fase 5: Definizione soluzione

---

### Opzione 1: trigger da sistema ordini

- stato aggiornato a “spedito”  
- invio email  

---

### Opzione 2: trigger da logistica

- evento spedizione  
- chiamata API verso sistema ordini  

---

👉 scelta dipende dall’architettura

---

## 📊 Fase 6: Specifica funzionale (semplificata)

---

### Funzionalità

Invio email alla spedizione ordine  

---

### Requisiti

- inviare email quando ordine = spedito  
- includere dati ordine  
- gestire errori invio  

---

### Criteri di accettazione

- email inviata correttamente  
- nessuna email duplicata  
- errore gestito  

---

## ⚙️ Fase 7: Aspetti tecnici

---

### Flusso

1. aggiornamento stato ordine  
2. trigger evento  
3. invio email  

---

### Gestione errori

- retry  
- logging  

---

## ⚠️ Fase 8: Rischi

---

### Duplicazione email
→ invii multipli  

---

### Mancato invio
→ perdita comunicazione  

---

### Incoerenza stato
→ email errate  

---

## 🧠 Fase 9: Coinvolgimento stakeholder

---

### Business

- contenuto email  
- momento invio  

---

### IT

- fattibilità  
- integrazione  

---

### QA

- test  

---

## ⚠️ Errori tipici (junior)

---

### Partire subito dalla soluzione
→ “aggiungiamo una mail”  

---

### Non analizzare integrazioni
→ problemi tecnici  

---

### Non considerare errori
→ sistema fragile  

---

## 🧠 Come ragiona un analista senior

Un analista senior:

- parte dal contesto  
- analizza flussi  
- identifica il vero punto di trigger  
- valuta opzioni  
- considera rischi  
- coinvolge stakeholder  

👉 La soluzione è **una conseguenza dell’analisi**

---

## 📌 Lezioni apprese

- anche richieste semplici nascondono complessità  
- il contesto è fondamentale  
- le integrazioni sono critiche  
- i rischi vanno sempre considerati  

---

## 🚀 In sintesi

Una richiesta evolutiva richiede:

- analisi  
- comprensione del sistema  
- valutazione impatti  
- definizione soluzione  

E soprattutto:

> **pensare prima di agire**

---

## ▶️ Prossimo caso

➡️ Vai a: [Caso integrazione sistemi](caso-integrazione-sistemi.md)