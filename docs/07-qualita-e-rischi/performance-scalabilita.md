# Performance e scalabilità

> Performance e scalabilità determinano se un sistema è utilizzabile nel mondo reale: non basta che funzioni, deve funzionare bene anche sotto carico.

---

## 🎯 Obiettivo della pagina

Comprendere:

- cosa sono performance e scalabilità
- perché sono critiche
- come analizzarle e definirle
- come evitare problemi nel tempo

---

## 🧭 Definizioni

---

### ⚡ Performance

Descrive:

> **quanto velocemente il sistema risponde**

Esempi:
- tempo di risposta  
- tempo di elaborazione  

---

### 📈 Scalabilità

Descrive:

> **quanto il sistema riesce a gestire l’aumento del carico**

Esempi:
- numero di utenti  
- volume dati  
- richieste simultanee  

---

## ⚖️ Principio chiave

> Un sistema che funziona con pochi utenti può fallire con molti utenti

---

## 🧩 Perché sono fondamentali

Performance e scalabilità influenzano:

- esperienza utente  
- stabilità  
- costi  
- affidabilità  

👉 Spesso i problemi emergono solo in produzione

---

## 🔍 Cosa analizzare

---

### ⏱️ Tempi di risposta

- quanto tempo impiega una funzione  
- in quali condizioni  

---

### 👥 Numero di utenti

- utenti simultanei  
- picchi di utilizzo  

---

### 📦 Volume dati

- quantità di dati gestiti  
- crescita nel tempo  

---

### 🔄 Frequenza operazioni

- quante richieste al secondo  
- operazioni ripetitive  

---

## 📊 Esempio

### Scenario
creazione ordine

### Performance
- tempo di risposta < 2 secondi  

### Scalabilità
- supportare 1.000 utenti contemporanei  

---

## ⚠️ Problemi tipici

---

### Sistema lento
→ cattiva esperienza utente  

---

### Collasso sotto carico
→ sistema non disponibile  

---

### Degrado progressivo
→ peggioramento nel tempo  

---

### Picchi non gestiti
→ problemi improvvisi  

---

## 🧠 Ruolo dell’analista

L’Analista di Sistema:

- identifica requisiti di performance  
- valuta carichi attesi  
- considera scenari di crescita  
- collabora con team tecnico  

👉 Non misura, ma **definisce cosa deve essere misurato**

---

## 🔄 Come definire i requisiti

---

### ✔ Misurabili

❌ “Il sistema deve essere veloce”  
✔ “Tempo di risposta < 2 secondi”  

---

### ✔ Contestualizzati

- per quale operazione  
- in quali condizioni  

---

### ✔ Realistici

- coerenti con contesto  
- tecnicamente sostenibili  

---

## 📊 Esempio strutturato

| Requisito | Valore |
|----------|--------|
| Tempo risposta ordine | < 2 secondi |
| Utenti simultanei | 1.000 |
| Richieste/sec | 100 |

---

## ⚠️ Errori comuni

---

### Non definirli
→ problemi in produzione  

---

### Definirli troppo tardi
→ costi elevati  

---

### Essere vaghi
→ inutili  

---

### Ignorare picchi
→ fallimenti improvvisi  

---

## 🧠 Come lavora un analista senior

Un analista senior:

- pensa in termini di carico  
- considera scenari reali  
- identifica punti critici  
- anticipa problemi  
- collabora con architetti  

👉 Non si chiede “funziona?”, ma “funziona sempre?”

---

## 📌 Buone pratiche

- definire requisiti misurabili  
- considerare picchi  
- includere crescita futura  
- testare condizioni reali  
- monitorare nel tempo  

---

## 🔄 Relazione con altri elementi

Performance e scalabilità influenzano:

- architettura  
- integrazioni  
- flussi  
- requisiti  

👉 Sono trasversali

---

## ⚖️ Performance vs scalabilità

| Performance | Scalabilità |
|------------|-------------|
| velocità | capacità |
| breve termine | lungo termine |
| risposta | crescita |

---

## 🚀 In sintesi

Performance e scalabilità permettono di:

- garantire velocità  
- gestire crescita  
- evitare problemi  

E soprattutto:

> **assicurare che il sistema funzioni anche nelle condizioni reali**

---

## ▶️ Prossimo passo

Ora che hai visto come il sistema si comporta sotto carico:

➡️ Vai a: [Analisi del rischio](analisi-rischio.md)