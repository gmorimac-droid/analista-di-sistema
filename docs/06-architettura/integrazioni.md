# Integrazioni

> Le integrazioni sono il modo in cui i sistemi collaborano tra loro: comprenderle è fondamentale per progettare soluzioni coerenti e affidabili.

---

## 🎯 Obiettivo della pagina

Comprendere:

- cosa sono le integrazioni
- perché sono critiche nei sistemi moderni
- quali tipi di integrazione esistono
- come analizzarle e progettarle correttamente

---

## 🧭 Cos’è un’integrazione

Un’integrazione è:

> **uno scambio strutturato di dati tra sistemi diversi**

Serve a:

- condividere informazioni  
- coordinare processi  
- mantenere coerenza  

---

## ⚖️ Principio chiave

> Più sistemi ci sono, più le integrazioni diventano il punto critico

---

## 🧩 Perché sono fondamentali

Le integrazioni permettono di:

- evitare duplicazione dei dati  
- collegare processi diversi  
- automatizzare flussi  
- costruire ecosistemi  

👉 Senza integrazioni, i sistemi sono isolati

---

## 🔄 Tipologie di integrazione

---

### 🔁 Sincrona (real-time)

- richiesta e risposta immediata  
- esempio: API REST  

#### Pro
- risposta immediata  

#### Contro
- forte dipendenza tra sistemi  

---

### 📦 Asincrona

- comunicazione differita  
- esempio: code, eventi  

#### Pro
- maggiore resilienza  

#### Contro
- maggiore complessità  

---

### 📄 Batch

- elaborazione periodica  
- esempio: file notturni  

#### Pro
- semplice da implementare  

#### Contro
- dati non aggiornati in tempo reale  

---

## 🔗 Pattern comuni

---

### Point-to-point

- collegamento diretto tra due sistemi  

👉 semplice, ma poco scalabile  

---

### Hub / middleware

- sistema centrale che gestisce integrazioni  

👉 più strutturato  

---

### Event-driven

- sistemi reagiscono a eventi  

👉 flessibile e moderno  

---

## 🔍 Elementi di un’integrazione

---

### 📤 Origine
chi invia i dati  

---

### 📥 Destinazione
chi riceve i dati  

---

### 📦 Payload
cosa viene trasmesso  

---

### 🔄 Modalità
come avviene lo scambio  

---

### ⚠️ Gestione errori
cosa succede se qualcosa fallisce  

---

## ⚠️ Problemi tipici

---

### Dipendenze forti
- un sistema blocca l’altro  

---

### Incoerenza dati
- dati diversi tra sistemi  

---

### Errori non gestiti
- perdita di informazioni  

---

### Mancanza di tracciabilità
- difficile capire cosa è successo  

---

## 🧠 Come analizzare un’integrazione

---

### 1. Capire il contesto
- perché serve  
- quali sistemi coinvolge  

---

### 2. Analizzare i dati
- cosa viene scambiato  
- formato  
- frequenza  

---

### 3. Valutare modalità
- sincrona / asincrona / batch  

---

### 4. Considerare errori
- fallback  
- retry  
- logging  

---

### 5. Valutare impatti
- dipendenze  
- performance  
- sicurezza  

---

## 📊 Esempio

### Scenario
Sistema Ordini → Sistema Pagamenti

### Integrazione
- invio richiesta pagamento  
- ricezione esito  

### Problemi possibili
- timeout  
- pagamento fallito  
- risposta non ricevuta  

👉 Serve gestione completa

---

## 🧠 Come lavora un analista senior

Un analista senior:

- identifica integrazioni critiche  
- valuta sempre resilienza  
- considera errori come parte del flusso  
- evita dipendenze inutili  
- mantiene visione end-to-end  

👉 Non vede solo “connessioni”, ma **comportamenti tra sistemi**

---

## 📌 Buone pratiche

- definire chiaramente responsabilità  
- documentare integrazioni  
- gestire errori esplicitamente  
- mantenere tracciabilità  
- evitare accoppiamenti troppo stretti  

---

## 🔄 Relazione con altri elementi

Le integrazioni collegano:

- architettura → struttura  
- flussi → movimento dati  
- requisiti → comportamento  

---

## 🚀 In sintesi

Le integrazioni permettono di:

- collegare sistemi  
- automatizzare processi  
- mantenere coerenza  

E soprattutto:

> **trasformare sistemi isolati in un ecosistema**

---

## ▶️ Prossimo passo

Ora che hai visto come i sistemi collaborano:

➡️ Vai a: [Sistemi legacy](sistemi-legacy.md)