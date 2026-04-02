# Dipendenze applicative

> Le dipendenze applicative descrivono come i sistemi sono collegati tra loro: comprenderle è fondamentale per evitare effetti imprevisti e gestire il cambiamento.

---

## 🎯 Obiettivo della pagina

Comprendere:

- cosa sono le dipendenze applicative
- perché sono critiche nei sistemi complessi
- come identificarle
- come gestirle in modo efficace

---

## 🧭 Cos’è una dipendenza applicativa

Una dipendenza applicativa esiste quando:

> **un sistema o componente dipende da un altro per funzionare correttamente**

Esempi:
- un sistema usa dati di un altro  
- un servizio chiama un’API esterna  
- un processo si basa su un flusso precedente  

---

## ⚖️ Principio chiave

> Ogni modifica in un sistema può propagarsi ad altri sistemi

---

## 🧩 Tipologie di dipendenze

---

### 🔗 Dipendenza diretta

- un sistema chiama direttamente un altro  

👉 esempio: API

---

### 🔄 Dipendenza indiretta

- la dipendenza passa attraverso altri sistemi  

👉 effetto a catena  

---

### 📦 Dipendenza sui dati

- un sistema utilizza dati prodotti da un altro  

👉 esempio: anagrafica clienti condivisa  

---

### ⏱️ Dipendenza temporale

- un sistema deve attendere un evento o processo  

👉 esempio: batch notturno  

---

## 📊 Esempio

Sistema A → Sistema B → Sistema C

Una modifica in A può impattare:

- direttamente B  
- indirettamente C  

👉 Anche se C non “vede” A

---

## ⚠️ Perché sono critiche

Le dipendenze:

- aumentano la complessità  
- creano vincoli  
- rendono le modifiche rischiose  

👉 Più dipendenze → più rischio

---

## 🔍 Come identificarle

---

### 1. Analizzare flussi informativi
- chi invia dati  
- chi li riceve  

---

### 2. Analizzare integrazioni
- API  
- file  
- messaggi  

---

### 3. Analizzare processi
- sequenze  
- dipendenze temporali  

---

### 4. Analizzare dati condivisi
- database  
- entità comuni  

---

## ⚠️ Problemi tipici

---

### Dipendenze non documentate
→ rischio elevato  

---

### Effetti a catena
→ problemi imprevisti  

---

### Accoppiamento forte
→ difficoltà di modifica  

---

### Dipendenze nascoste
→ difficili da individuare  

---

## 🧠 Come gestirle

---

### 🔍 Mappare le dipendenze

- identificare sistemi coinvolti  
- rappresentare relazioni  

---

### ⚖️ Valutare impatti

- cosa cambia  
- chi è coinvolto  
- quali rischi  

---

### 🔄 Ridurre accoppiamento

- evitare dipendenze dirette inutili  
- favorire modularità  

---

### 📄 Documentare

- mantenere visibilità  
- aggiornare nel tempo  

---

## 🧠 Come lavora un analista senior

Un analista senior:

- pensa sempre in termini di dipendenze  
- non considera mai una modifica isolata  
- anticipa effetti indiretti  
- identifica sistemi critici  
- usa le dipendenze per guidare le decisioni  

👉 Vede il sistema come una rete, non come parti separate

---

## 📌 Buone pratiche

- non assumere indipendenza  
- verificare sempre impatti  
- mantenere visione end-to-end  
- coinvolgere tutti i sistemi interessati  
- evitare modifiche “locali” senza analisi  

---

## 📊 Esempio pratico

### Modifica richiesta
cambiare struttura dati cliente

### Impatti possibili

- sistema ordini  
- sistema fatturazione  
- sistema CRM  
- report  

👉 Una modifica semplice diventa complessa

---

## ⚖️ Dipendenze vs complessità

| Poche dipendenze | Molte dipendenze |
|-----------------|------------------|
| maggiore autonomia | maggiore rigidità |
| più flessibilità | più rischio |

---

## 🚀 In sintesi

Le dipendenze applicative permettono di:

- comprendere relazioni tra sistemi  
- valutare impatti  
- ridurre rischi  

E soprattutto:

> **capire perché ogni modifica può avere effetti a catena**

---

## ▶️ Prossimo passo

Ora che hai visto come i sistemi sono collegati:

➡️ Vai a: [Requisiti non funzionali](../07-qualita-e-rischi/requisiti-non-funzionali.md)