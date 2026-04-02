# Specifica tecnica

> La specifica tecnica descrive come la soluzione viene implementata: rappresenta il ponte tra analisi e sviluppo.

---

## 🎯 Obiettivo della pagina

Comprendere:

- cos’è una specifica tecnica
- in cosa differisce dalla specifica funzionale
- qual è il ruolo dell’analista
- come strutturarla in modo efficace

---

## 🧭 Cos’è una specifica tecnica

La specifica tecnica è:

> **un documento che descrive come realizzare tecnicamente una soluzione**

Include:
- architettura  
- componenti  
- integrazioni  
- flussi tecnici  
- strutture dati  

---

## ⚖️ Principio chiave

> La specifica tecnica traduce il “cosa” in “come”

---

## 🔄 Differenza con la specifica funzionale

| Specifica funzionale | Specifica tecnica |
|---------------------|------------------|
| cosa deve fare | come viene implementato |
| orientata al business | orientata all’IT |
| descrittiva | progettuale |

👉 Sono complementari, non alternative

---

## 🧩 A cosa serve

La specifica tecnica serve a:

- guidare lo sviluppo  
- definire l’architettura  
- chiarire integrazioni  
- ridurre incertezze tecniche  

---

## 🧱 Struttura tipica

---

### 🧭 1. Overview

- contesto tecnico  
- obiettivi  

---

### 🧱 2. Architettura

- componenti coinvolti  
- relazioni  

---

### 🔗 3. Integrazioni

- sistemi coinvolti  
- modalità di comunicazione  

---

### 🔄 4. Flussi tecnici

- sequenza operazioni  
- gestione errori  

---

### 📦 5. Dati

- strutture dati  
- mapping  

---

### ⚠️ 6. Vincoli tecnici

- limiti  
- scelte tecnologiche  

---

## 📊 Esempio sintetico

### Funzionalità: Creazione ordine

**Architettura**
- frontend → backend → database  

**Flusso**
1. richiesta API  
2. validazione  
3. salvataggio  

**Integrazione**
- sistema pagamenti  

**Gestione errori**
- risposta errore standard  

---

## 🧠 Ruolo dell’analista

Dipende dal contesto:

---

### 🔹 Analista funzionale

- contribuisce  
- verifica coerenza  
- non entra nei dettagli tecnici  

---

### 🔹 Analista di sistema

- partecipa attivamente  
- definisce flussi  
- contribuisce alle integrazioni  

---

### 🔹 Architetto / sviluppatore

- definisce dettagli tecnici  
- implementa  

---

👉 L’analista di sistema sta **a metà tra funzionale e tecnico**

---

## ⚠️ Dove arriva l’analista

L’analista di sistema:

✔ definisce:
- flussi  
- integrazioni  
- dati ad alto livello  

❌ non definisce:
- codice  
- dettagli implementativi  
- configurazioni tecniche specifiche  

---

## ⚠️ Errori comuni

---

### Andare troppo nel tecnico
→ invade il ruolo dello sviluppatore  

---

### Restare troppo alto livello
→ documento inutile  

---

### Non allineare con funzionale
→ incoerenza  

---

### Non coinvolgere sviluppo
→ problemi implementativi  

---

## 🧠 Come lavora un analista senior

Un analista senior:

- mantiene equilibrio tra funzionale e tecnico  
- chiarisce flussi e integrazioni  
- anticipa problemi tecnici  
- collabora con sviluppatori  
- non entra nei dettagli inutili  

👉 Non scrive codice, ma **rende lo sviluppo possibile**

---

## 📌 Buone pratiche

- mantenere chiarezza  
- definire responsabilità  
- usare diagrammi se utile  
- validare con team tecnico  
- mantenere allineamento con funzionale  

---

## 🔄 Relazione con altri deliverable

La specifica tecnica si collega a:

- specifica funzionale → base  
- architettura → struttura  
- flussi → comportamento  
- integrazioni → comunicazione  

---

## 🚀 In sintesi

La specifica tecnica permette di:

- tradurre requisiti in implementazione  
- guidare sviluppo  
- ridurre incertezze  

E soprattutto:

> **collegare analisi e realizzazione tecnica**

---

## ▶️ Prossimo passo

Ora che hai visto la specifica tecnica:

➡️ Vai a: [Tracciabilità](tracciabilita.md)