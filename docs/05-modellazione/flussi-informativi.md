# Flussi informativi

> I flussi informativi descrivono come i dati si muovono tra sistemi, processi e attori: comprenderli è essenziale per analizzare e progettare soluzioni corrette.

---

## 🎯 Obiettivo della pagina

Comprendere:

- cosa sono i flussi informativi
- perché sono fondamentali
- come identificarli e descriverli
- come usarli per analizzare e progettare sistemi

---

## 🧭 Cos’è un flusso informativo

Un flusso informativo descrive:

> **il movimento dei dati da un punto a un altro**

Include:
- origine (chi invia)  
- destinazione (chi riceve)  
- contenuto (cosa viene trasmesso)  
- modalità (come avviene lo scambio)  

---

## 🧩 Elementi fondamentali

---

### 📤 Origine
Chi genera o invia i dati

Esempi:
- utente  
- sistema  
- processo  

---

### 📥 Destinazione
Chi riceve i dati

Esempi:
- altro sistema  
- database  
- servizio  

---

### 📦 Contenuto
Quali dati vengono trasmessi

Esempi:
- dati cliente  
- ordine  
- stato  

---

### 🔄 Modalità
Come avviene lo scambio

Esempi:
- API  
- file  
- messaggi  
- interazione utente  

---

## 📊 Esempio semplice

### Scenario: creazione ordine

1. Utente → Sistema A  
   inserisce dati ordine  

2. Sistema A → Database  
   salva ordine  

3. Sistema A → Sistema B  
   invia dati per fatturazione  

👉 Tre flussi distinti

---

## ⚖️ Perché sono fondamentali

I flussi informativi permettono di:

- comprendere il funzionamento reale  
- identificare dipendenze  
- analizzare impatti  
- progettare integrazioni  

👉 Senza flussi, si vede solo una parte del sistema

---

## 🔄 Tipologie di flussi

---

### 🔁 Sincroni

- richiesta e risposta immediata  
- esempio: API REST  

👉 Pro:
- risposta immediata  

👉 Contro:
- dipendenza diretta  

---

### 📦 Asincroni

- comunicazione differita  
- esempio: code, eventi  

👉 Pro:
- maggiore resilienza  

👉 Contro:
- maggiore complessità  

---

### 📄 Batch

- elaborazione periodica  
- esempio: file giornalieri  

👉 Pro:
- semplice  

👉 Contro:
- non real-time  

---

## 🔍 Come identificare i flussi

---

### 1. Partire dai processi
- cosa succede  
- chi interagisce  

---

### 2. Identificare i dati
- cosa viene creato  
- cosa viene modificato  
- cosa viene trasmesso  

---

### 3. Tracciare il percorso
- da dove parte  
- dove arriva  
- come si muove  

---

## ⚠️ Errori comuni

---

### Ignorare flussi nascosti
- processi manuali  
- integrazioni non documentate  

---

### Non distinguere modalità
- sincrono vs asincrono  

---

### Non considerare errori
- cosa succede se il flusso fallisce?  

---

### Non vedere le dipendenze
→ effetti a catena  

---

## 🧠 Come lavora un analista senior

Un analista senior:

- identifica rapidamente i flussi critici  
- distingue tra flussi principali e secondari  
- considera sempre errori e fallback  
- valuta impatti delle modifiche  
- mantiene una visione end-to-end  

👉 Non vede singoli sistemi, ma **ecosistemi**

---

## 📌 Rappresentazione

I flussi possono essere rappresentati con:

- diagrammi  
- tabelle  
- descrizioni strutturate  

👉 L’importante è la chiarezza, non lo strumento

---

## 📊 Esempio strutturato

| Origine   | Destinazione | Contenuto     | Modalità |
|----------|-------------|--------------|----------|
| Sistema A | Sistema B  | Dati ordine  | API      |
| Sistema B | Database   | Fattura      | Batch    |

---

## 🔄 Relazione con altri elementi

I flussi informativi collegano:

- use case → comportamento  
- architettura → struttura  
- integrazioni → comunicazione  

---

## 🚀 In sintesi

I flussi informativi permettono di:

- capire come circolano i dati  
- identificare dipendenze  
- progettare integrazioni  

E soprattutto:

> **vedere il sistema come un insieme connesso**

---

## ▶️ Prossimo passo

Ora che hai visto come si muovono i dati:

➡️ Vai a: [Modello dati ad alto livello](modello-dati-alto-livello.md)