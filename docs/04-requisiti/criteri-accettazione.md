# Criteri di accettazione

> I criteri di accettazione definiscono quando un requisito può essere considerato soddisfatto: senza di essi, non esiste una vera verifica.

---

## 🎯 Obiettivo della pagina

Comprendere:

- cosa sono i criteri di accettazione
- perché sono essenziali
- come scriverli in modo efficace
- come collegano analisi, sviluppo e test

---

## 🧭 Cos’è un criterio di accettazione

Un criterio di accettazione è:

> una condizione chiara e verificabile che determina se una funzionalità è corretta

Risponde alla domanda:

👉 **“Come sappiamo che funziona davvero?”**

---

## ⚖️ Principio chiave

> Se non è verificabile, non è un buon requisito

---

## 🧩 A cosa servono

I criteri di accettazione:

- chiariscono il comportamento atteso  
- riducono ambiguità  
- guidano lo sviluppo  
- supportano il testing  
- allineano stakeholder  

👉 Sono il ponte tra **analisi e validazione**

---

## 🧠 Struttura di base

Un criterio di accettazione deve essere:

- chiaro  
- specifico  
- verificabile  
- non ambiguo  

---

## 🧾 Formati comuni

---

### 🔹 Forma descrittiva

Esempio:

> Il sistema deve permettere la creazione di un ordine solo se il cliente è attivo.

---

### 🔹 Forma strutturata (Given / When / Then)

Formato molto efficace:

- **Given** → contesto iniziale  
- **When** → azione  
- **Then** → risultato atteso  

#### Esempio

- Given: cliente attivo  
- When: viene creato un ordine  
- Then: l’ordine viene salvato correttamente  

---

## 🔍 Tipologie di criteri

---

### ⚙️ Funzionali

Verificano comportamento del sistema

Esempio:
- inserimento dati corretto
- esecuzione di un’azione

---

### ⚠️ Negativi / di errore

Verificano cosa succede in caso di errore

Esempio:
- input non valido
- dati mancanti

---

### 🔒 Non funzionali

Verificano qualità del sistema

Esempio:
- tempo di risposta
- sicurezza
- disponibilità

---

### 🔄 Edge case

Verificano casi limite

Esempio:
- valori estremi
- condizioni rare

---

## 📊 Esempio completo

### Requisito
> Il sistema deve permettere la creazione di un ordine

### Criteri di accettazione

1. Cliente attivo → ordine creato con successo  
2. Cliente inattivo → errore e blocco operazione  
3. Dati mancanti → messaggio di errore  
4. Tempo di risposta < 2 secondi  

👉 Il requisito diventa testabile

---

## ⚠️ Errori comuni

---

### Essere vaghi
> “Il sistema deve funzionare correttamente”

→ non verificabile

---

### Essere incompleti
- mancano casi negativi
- mancano condizioni

---

### Essere troppo dettagliati
- livello eccessivo
- perdita di leggibilità

---

### Non coprire edge case
→ problemi in produzione

---

## 🔄 Relazione con altri elementi

I criteri di accettazione collegano:

- requisiti → cosa fare  
- sviluppo → come implementare  
- test → come verificare  

👉 Sono il punto di convergenza

---

## 🧠 Come lavora un analista senior

Un analista senior:

- scrive criteri mentre definisce i requisiti  
- pensa già in termini di testabilità  
- anticipa casi limite  
- coinvolge QA nella definizione  
- usa criteri per chiarire ambiguità  

👉 Non aggiunge criteri dopo: **li integra nel pensiero**

---

## 📌 Buone pratiche

- usare linguaggio semplice  
- evitare ambiguità  
- coprire casi positivi e negativi  
- includere edge case  
- mantenere equilibrio tra dettaglio e chiarezza  

---

## 🧩 Checklist

Un buon criterio è:

- ✔ chiaro  
- ✔ verificabile  
- ✔ completo  
- ✔ coerente con il requisito  

---

## 🚀 In sintesi

I criteri di accettazione permettono di:

- rendere i requisiti testabili  
- ridurre incomprensioni  
- migliorare qualità  

E soprattutto:

> **definire in modo oggettivo quando qualcosa è fatto bene**

---

## ▶️ Prossimo passo

Ora che sai rendere verificabili i requisiti:

➡️ Vai a: [Gestione ambiguità](gestione-ambiguita.md)