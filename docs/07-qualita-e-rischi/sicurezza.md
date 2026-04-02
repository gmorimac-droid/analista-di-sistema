# Sicurezza

> La sicurezza è un requisito trasversale che protegge dati, sistemi e processi: non è un’aggiunta, ma una parte integrante dell’analisi.

---

## 🎯 Obiettivo della pagina

Comprendere:

- cosa significa sicurezza nei sistemi informativi
- quali aspetti considerare
- come integrare la sicurezza nell’analisi
- quali errori evitare

---

## 🧭 Cos’è la sicurezza

La sicurezza informatica riguarda:

> **protezione di dati, accessi e operazioni da utilizzi non autorizzati o dannosi**

---

## ⚖️ Principio chiave

> La sicurezza deve essere progettata, non aggiunta dopo

---

## 🧩 Pilastri della sicurezza

---

### 🔐 Autenticazione

#### Cos’è
Verifica dell’identità

#### Esempi
- username/password  
- autenticazione a due fattori  

---

### 🔑 Autorizzazione

#### Cos’è
Definisce cosa può fare un utente

#### Esempi
- accesso in lettura  
- accesso in modifica  

---

### 🛡️ Protezione dei dati

#### Include
- dati sensibili  
- crittografia  
- protezione in transito e a riposo  

---

### 📄 Audit e tracciabilità

#### Cos’è
Registrazione delle operazioni

#### Serve per
- controlli  
- analisi problemi  
- compliance  

---

## 🔍 Aree da considerare

---

### 👤 Accessi

- chi può accedere  
- da dove  
- con quali modalità  

---

### 📦 Dati

- quali dati sono sensibili  
- dove vengono memorizzati  
- come vengono trasmessi  

---

### 🔄 Flussi

- dove passano i dati  
- quali sistemi coinvolti  

---

### ⚠️ Errori

- gestione accessi non validi  
- tentativi di accesso non autorizzati  

---

## ⚠️ Problemi tipici

---

### Accessi troppo permissivi
→ rischio di abuso  

---

### Mancanza di controlli
→ vulnerabilità  

---

### Dati non protetti
→ esposizione  

---

### Logging insufficiente
→ difficile analisi  

---

## 🧠 Ruolo dell’analista

L’Analista di Sistema:

- identifica requisiti di sicurezza  
- integra la sicurezza nei requisiti  
- verifica impatti  
- collabora con specialisti  

👉 Non implementa, ma **garantisce che sia considerata**

---

## 🔄 Sicurezza e requisiti

La sicurezza deve essere:

- esplicita  
- documentata  
- verificabile  

---

### Esempio

Requisito:
> accesso al sistema

Requisiti di sicurezza:
- autenticazione obbligatoria  
- autorizzazione per ruolo  
- tracciamento accessi  

---

## 📊 Esempio pratico

### Scenario
accesso dati cliente

### Analisi

- chi può accedere?  
- quali dati sono visibili?  
- serve tracciamento?  

👉 La sicurezza modifica il comportamento del sistema

---

## ⚠️ Errori comuni

---

### Considerarla alla fine
→ costi elevati  

---

### Essere troppo generici
→ “il sistema deve essere sicuro”  

---

### Non coinvolgere esperti
→ soluzioni incomplete  

---

### Non testarla
→ vulnerabilità  

---

## 🧠 Come lavora un analista senior

Un analista senior:

- integra la sicurezza fin dall’inizio  
- identifica dati sensibili  
- considera sempre accessi e autorizzazioni  
- anticipa rischi  
- collabora con team sicurezza  

👉 Non vede la sicurezza come un extra, ma come parte del sistema

---

## 📌 Buone pratiche

- definire requisiti chiari  
- proteggere dati sensibili  
- gestire accessi correttamente  
- tracciare operazioni  
- verificare nei test  

---

## 🔄 Relazione con altri elementi

La sicurezza impatta:

- requisiti  
- architettura  
- integrazioni  
- flussi  

👉 È trasversale a tutto

---

## 🚀 In sintesi

La sicurezza permette di:

- proteggere dati  
- prevenire accessi non autorizzati  
- garantire affidabilità  

E soprattutto:

> **evitare problemi critici e spesso irreversibili**

---

## ▶️ Prossimo passo

Ora che hai visto la sicurezza:

➡️ Vai a: [Performance e scalabilità](performance-scalabilita.md)