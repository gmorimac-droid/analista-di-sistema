# Requisiti non funzionali

> I requisiti non funzionali definiscono come il sistema deve comportarsi: sono fondamentali per qualità, affidabilità e sostenibilità.

---

## 🎯 Obiettivo della pagina

Comprendere:

- cosa sono i requisiti non funzionali
- perché sono critici
- quali categorie esistono
- come definirli correttamente

---

## 🧭 Cos’è un requisito non funzionale

Un requisito non funzionale descrive:

> **le caratteristiche qualitative del sistema**

Non definisce cosa fa, ma:

👉 **come lo fa**

---

## ⚖️ Principio chiave

> Un sistema può essere funzionalmente corretto ma inutilizzabile se i requisiti non funzionali non sono soddisfatti

---

## 🧩 Differenza con i requisiti funzionali

| Funzionali | Non funzionali |
|-----------|----------------|
| cosa fa il sistema | come si comporta |
| azioni | qualità |
| es. creare ordine | es. tempo di risposta |

---

## 🔍 Principali categorie

---

### ⚡ Performance

#### Descrive
- velocità  
- tempi di risposta  

#### Esempio
> tempo di risposta < 2 secondi  

---

### 🔒 Sicurezza

#### Descrive
- accessi  
- protezione dati  
- autorizzazioni  

#### Esempio
> accesso consentito solo a utenti autenticati  

---

### 📈 Scalabilità

#### Descrive
- capacità di gestire crescita  

#### Esempio
> supportare 10.000 utenti contemporanei  

---

### 🟢 Disponibilità

#### Descrive
- continuità del servizio  

#### Esempio
> sistema disponibile 99.9%  

---

### 🔄 Affidabilità

#### Descrive
- stabilità  
- gestione errori  

---

### 🧾 Auditabilità

#### Descrive
- tracciabilità delle operazioni  

---

### 👤 Usabilità

#### Descrive
- facilità d’uso  

---

## ⚠️ Perché sono spesso trascurati

- meno visibili  
- più difficili da definire  
- percepiti come secondari  

👉 Ma spesso sono la causa principale dei problemi

---

## 🔄 Quando definirli

I requisiti non funzionali devono essere:

- identificati durante l’analisi  
- non aggiunti alla fine  

👉 Devono influenzare la soluzione fin dall’inizio

---

## 📊 Esempio

### Requisito funzionale
> creare ordine  

### Non funzionali associati
- tempo di risposta < 2 secondi  
- accesso autenticato  
- tracciamento operazione  

👉 Senza questi, il requisito è incompleto

---

## ⚠️ Errori comuni

---

### Essere vaghi
> “il sistema deve essere veloce”

---

### Non definirli
→ problemi in produzione  

---

### Definirli troppo tardi
→ costi elevati  

---

### Non verificarli
→ inutili  

---

## 🧠 Come scriverli correttamente

Un buon requisito non funzionale è:

- misurabile  
- verificabile  
- specifico  

---

### Esempio

❌ Non corretto  
> il sistema deve essere veloce  

✔ Corretto  
> tempo di risposta < 2 secondi per operazione X  

---

## 🔄 Relazione con altri elementi

I requisiti non funzionali influenzano:

- architettura  
- integrazioni  
- flussi  
- sicurezza  

👉 Sono trasversali

---

## 🧠 Come lavora un analista senior

Un analista senior:

- identifica NFR fin dall’inizio  
- li rende misurabili  
- li collega ai requisiti funzionali  
- considera impatti su architettura  
- coinvolge team tecnico  

👉 Non li aggiunge, li **integra**

---

## 📌 Buone pratiche

- definire sempre  
- renderli misurabili  
- collegarli ai requisiti  
- validarli con stakeholder  
- verificarli nei test  

---

## 📊 Checklist

Un buon NFR è:

- ✔ chiaro  
- ✔ misurabile  
- ✔ verificabile  
- ✔ rilevante  

---

## 🚀 In sintesi

I requisiti non funzionali permettono di:

- garantire qualità  
- ridurre rischi  
- migliorare affidabilità  

E soprattutto:

> **trasformare un sistema funzionante in un sistema utilizzabile**

---

## ▶️ Prossimo passo

Ora che hai visto la qualità del sistema:

➡️ Vai a: [Sicurezza](sicurezza.md)