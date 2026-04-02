# Classificazione requisiti

> Classificare i requisiti significa dare struttura a ciò che è stato raccolto, rendendo le informazioni comprensibili, gestibili e utilizzabili.

---

## 🎯 Obiettivo della pagina

Comprendere:

- perché è importante classificare i requisiti
- quali categorie utilizzare
- come organizzare le informazioni
- come evitare confusione e sovrapposizioni

---

## 🧭 Perché classificare

Dopo la raccolta, i requisiti sono spesso:

- disordinati  
- incompleti  
- mescolati tra loro  

Senza classificazione:

- è difficile analizzare  
- è difficile comunicare  
- è difficile implementare  

👉 La classificazione porta **ordine e chiarezza**

---

## ⚖️ Principio chiave

> Ogni requisito deve avere una natura chiara

---

## 🧩 Le principali categorie

---

### ⚙️ 1. Requisiti funzionali

#### Definizione
Descrivono cosa deve fare il sistema.

#### Esempi
- creare un ordine  
- aggiornare un cliente  
- inviare una notifica  

#### Caratteristiche
- osservabili
- verificabili
- legati a comportamenti

---

### 📊 2. Requisiti non funzionali

#### Definizione
Descrivono come il sistema deve funzionare.

#### Esempi
- performance (tempo di risposta)
- sicurezza
- disponibilità
- scalabilità

#### Attenzione
Spesso vengono dimenticati, ma sono critici

---

### 🔒 3. Vincoli

#### Definizione
Limiti entro cui la soluzione deve operare.

#### Tipologie
- tecnici (tecnologie, sistemi esistenti)
- normativi (compliance)
- organizzativi (processi, ruoli)

#### Esempio
> “Deve integrarsi con il sistema legacy X”

---

### 🧩 4. Regole di business

#### Definizione
Logiche specifiche del dominio.

#### Esempi
- calcoli
- condizioni
- validazioni

#### Importanza
- spesso implicite
- fondamentali per il corretto funzionamento

---

### 👤 5. Requisiti utente

#### Definizione
Bisogni espressi dal punto di vista dell’utente.

#### Esempio
> “Voglio poter visualizzare lo stato dell’ordine”

👉 Spesso punto di partenza per requisiti funzionali

---

### 🔗 6. Requisiti di integrazione

#### Definizione
Descrivono interazioni con altri sistemi.

#### Esempi
- API
- scambio file
- sincronizzazione dati

---

## 📊 Strutturazione dei requisiti

Una volta classificati, vanno organizzati.

---

### 📌 Per categoria

- funzionali
- non funzionali
- vincoli
- ecc.

👉 utile per visione globale

---

### 📌 Per funzionalità

- modulo cliente
- modulo ordini
- modulo pagamenti

👉 utile per sviluppo

---

### 📌 Per priorità

- alta
- media
- bassa

👉 utile per pianificazione

---

## ⚖️ Granularità

Un requisito deve essere:

- abbastanza dettagliato da essere chiaro  
- abbastanza sintetico da essere gestibile  

⚠️ Errori:

- troppo generico → ambiguo  
- troppo dettagliato → ingestibile  

---

## 🔄 Relazioni tra requisiti

I requisiti non sono isolati.

Esistono relazioni:

- dipendenze  
- inclusioni  
- derivazioni  

👉 Comprendere le relazioni evita incoerenze

---

## ⚠️ Problemi tipici

---

### Mescolare tipi diversi
- funzionale + non funzionale nello stesso requisito

---

### Mancanza di classificazione
- tutto nello stesso elenco

---

### Requisiti duplicati
- stessa cosa descritta più volte

---

### Requisiti contraddittori
- logiche incoerenti

---

## 🧠 Come lavora un analista senior

Un analista senior:

- classifica già durante la raccolta
- riconosce subito il tipo di requisito
- mantiene ordine continuo
- evita duplicazioni
- evidenzia relazioni

👉 Non organizza dopo, **organizza mentre analizza**

---

## 📌 Buone pratiche

- separare chiaramente le categorie
- usare naming coerente
- mantenere struttura semplice
- aggiornare continuamente
- evitare ridondanze

---

## 📊 Esempio

### Input (grezzo)
> “Il sistema deve essere veloce e permettere di creare ordini e rispettare le regole aziendali”

### Output classificato

- Funzionale → creare ordine  
- Non funzionale → tempo di risposta < 2 secondi  
- Regola di business → validazione ordine secondo regole X  

---

## 🚀 In sintesi

La classificazione dei requisiti permette di:

- dare ordine  
- migliorare chiarezza  
- facilitare sviluppo e test  

E soprattutto:

> **trasformare informazioni disordinate in struttura utilizzabile**

---

## ▶️ Prossimo passo

Ora che hai classificato i requisiti:

➡️ Vai a: [Criteri di accettazione](criteri-accettazione.md)