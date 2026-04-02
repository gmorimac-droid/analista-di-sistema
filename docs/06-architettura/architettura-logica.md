# Architettura logica

> L’architettura logica rappresenta la struttura del sistema a livello concettuale: mostra componenti, relazioni e flussi senza entrare nei dettagli tecnici.

---

## 🎯 Obiettivo della pagina

Comprendere:

- cos’è un’architettura logica
- perché è fondamentale per l’analisi
- come costruirla
- come usarla per prendere decisioni

---

## 🧭 Cos’è l’architettura logica

L’architettura logica descrive:

> **come è organizzato il sistema e come interagiscono i suoi componenti**

Include:
- sistemi e componenti  
- relazioni tra sistemi  
- flussi informativi  
- responsabilità  

👉 Non descrive *come è implementato*, ma *come è strutturato*

---

## ⚖️ Principio chiave

> L’architettura logica deve essere comprensibile sia al business che all’IT

---

## 🧩 Elementi fondamentali

---

### 🧱 Componenti

Unità logiche del sistema

#### Esempi
- sistema ordini  
- sistema clienti  
- sistema pagamenti  

---

### 🔗 Relazioni

Collegamenti tra componenti

#### Esempi
- integrazione tra sistemi  
- dipendenze  

---

### 🔄 Flussi

Movimento dei dati tra componenti

👉 già visti nei flussi informativi, qui vengono integrati

---

### 🎯 Responsabilità

Cosa fa ogni componente

#### Esempio
- sistema A → gestione clienti  
- sistema B → gestione ordini  

---

## 📊 Esempio semplice

### Componenti
- Sistema Clienti  
- Sistema Ordini  
- Sistema Pagamenti  

### Relazioni
- Clienti → Ordini  
- Ordini → Pagamenti  

### Flussi
- dati cliente  
- dati ordine  
- stato pagamento  

👉 Visione completa e sintetica

---

## 🧠 Perché è fondamentale

L’architettura logica permette di:

- avere una visione d’insieme  
- comprendere dipendenze  
- analizzare impatti  
- progettare soluzioni coerenti  

👉 Senza architettura, si lavora “a pezzi”

---

## 🔄 Relazione con altri elementi

L’architettura logica integra:

- AS-IS / TO-BE → stato attuale e futuro  
- use case → comportamento  
- flussi → movimento dati  
- modello dati → significato  

👉 È il punto di convergenza

---

## 🔍 Come costruirla

---

### 1. Identificare i componenti
- sistemi esistenti  
- nuovi elementi  

---

### 2. Definire responsabilità
- cosa fa ogni componente  
- cosa NON fa  

---

### 3. Tracciare relazioni
- integrazioni  
- dipendenze  

---

### 4. Integrare flussi
- cosa passa tra i componenti  
- come  

---

### 5. Validare
- con IT  
- con business  

---

## ⚠️ Errori comuni

---

### Essere troppo tecnici
→ difficile da capire  

---

### Essere troppo generici
→ poco utile  

---

### Non definire responsabilità
→ sovrapposizioni  

---

### Ignorare flussi
→ visione incompleta  

---

## ⚖️ Architettura logica vs tecnica

| Architettura logica | Architettura tecnica |
|--------------------|---------------------|
| cosa e come a livello concettuale | come è implementato |
| comprensibile a tutti | più tecnica |
| indipendente dalla tecnologia | legata alla tecnologia |

👉 L’analista lavora principalmente sulla logica

---

## 🧠 Come lavora un analista senior

Un analista senior:

- costruisce una visione chiara e sintetica  
- identifica rapidamente componenti critici  
- evidenzia dipendenze  
- anticipa impatti  
- usa l’architettura per guidare decisioni  

👉 Non descrive sistemi, ma **li organizza mentalmente**

---

## 📌 Buone pratiche

- mantenere semplicità  
- usare naming coerente  
- separare responsabilità  
- aggiornare nel tempo  
- validare con gli stakeholder  

---

## 📊 Livello di dettaglio

Dipende dal contesto:

- overview → pochi componenti  
- dettaglio → più livelli  

👉 L’obiettivo è chiarezza, non completezza assoluta

---

## 🚀 In sintesi

L’architettura logica permette di:

- unire sistemi, dati e flussi  
- avere una visione d’insieme  
- progettare soluzioni coerenti  

E soprattutto:

> **trasformare analisi frammentate in una struttura unica**

---

## ▶️ Prossimo passo

Ora che hai una visione completa del sistema:

➡️ Vai a: [Integrazioni](integrazioni.md)