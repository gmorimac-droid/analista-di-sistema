# Modello dati ad alto livello

> Il modello dati ad alto livello descrive cosa rappresentano i dati e come sono collegati: è la base per comprendere il significato del sistema.

---

## 🎯 Obiettivo della pagina

Comprendere:

- cos’è un modello dati ad alto livello
- perché è fondamentale per l’analisi
- come costruirlo in modo efficace
- come usarlo per migliorare comprensione e coerenza

---

## 🧭 Cos’è un modello dati ad alto livello

Un modello dati ad alto livello descrive:

> **le entità principali del sistema e le relazioni tra loro**

Non entra nei dettagli tecnici (tabelle, tipi, indici), ma si concentra su:

- cosa rappresentano i dati  
- come sono collegati  
- quali sono i concetti chiave  

---

## ⚖️ Principio chiave

> Prima di capire dove stanno i dati, bisogna capire cosa sono

---

## 🧩 Elementi fondamentali

---

### 📦 Entità

Oggetti principali del dominio

#### Esempi
- Cliente  
- Ordine  
- Prodotto  
- Fattura  

👉 Rappresentano “cose” rilevanti

---

### 🧾 Attributi

Informazioni associate a un’entità

#### Esempi (Cliente)
- nome  
- email  
- stato  

👉 Descrivono l’entità

---

### 🔗 Relazioni

Collegamenti tra entità

#### Esempi
- Cliente → Ordine  
- Ordine → Prodotto  

👉 Mostrano come le entità interagiscono

---

## 📊 Esempio semplice

### Entità
- Cliente  
- Ordine  

### Relazione
- un cliente può avere più ordini  

### Attributi (ordine)
- data  
- importo  
- stato  

👉 Modello semplice ma chiaro

---

## 🧠 Perché è fondamentale

Il modello dati permette di:

- comprendere il dominio  
- evitare incomprensioni  
- identificare incoerenze  
- supportare analisi e progettazione  

👉 Senza modello dati, si lavora “a intuizione”

---

## 🔄 Relazione con altri elementi

Il modello dati collega:

- requisiti → cosa serve  
- use case → come si usa  
- flussi → dove vanno i dati  

👉 È il livello semantico del sistema

---

## 🔍 Come costruirlo

---

### 1. Identificare le entità
- cosa è rilevante nel dominio  
- cosa viene gestito dal sistema  

---

### 2. Definire attributi principali
- informazioni essenziali  
- evitare dettagli tecnici  

---

### 3. Identificare relazioni
- come le entità sono collegate  
- cardinalità (uno-a-molti, molti-a-molti)  

---

### 4. Validare
- con business  
- con team tecnico  

---

## ⚠️ Errori comuni

---

### Essere troppo tecnici
- pensare in termini di database  
→ perde valore analitico  

---

### Essere troppo generici
- entità vaghe  
→ poca utilità  

---

### Ignorare relazioni
→ visione incompleta  

---

### Non aggiornare il modello
→ incoerenza nel tempo  

---

## ⚖️ Livello di dettaglio

Il modello ad alto livello deve:

- essere comprensibile  
- essere sintetico  
- rappresentare ciò che conta  

👉 Non serve dettagliare tutto

---

## 🧠 Come lavora un analista senior

Un analista senior:

- identifica rapidamente le entità chiave  
- semplifica il dominio  
- evita ridondanze  
- mantiene coerenza tra modello e realtà  
- usa il modello per guidare le decisioni  

👉 Non descrive dati, ma **struttura il significato**

---

## 📌 Buone pratiche

- usare nomi chiari  
- mantenere consistenza  
- evitare duplicazioni  
- rappresentare relazioni esplicite  
- aggiornare nel tempo  

---

## 📊 Esempio evoluto

### Entità
- Cliente  
- Ordine  
- Prodotto  
- Pagamento  

### Relazioni
- Cliente → Ordine  
- Ordine → Prodotto  
- Ordine → Pagamento  

👉 Visione completa del dominio

---

## 🚀 In sintesi

Il modello dati ad alto livello permette di:

- comprendere il significato dei dati  
- strutturare il dominio  
- migliorare coerenza  

E soprattutto:

> **trasformare dati in conoscenza**

---

## ▶️ Prossimo passo

Ora che hai visto come rappresentare i dati:

➡️ Vai a: [Architettura logica](../06-architettura/architettura-logica.md)