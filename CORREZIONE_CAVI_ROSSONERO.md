# CORREZIONE CAVI ROSSO-NERO
## Progetto Cortina 2026 - v1.0.02

**Data correzione:** 15 Gennaio 2026
**Responsabile:** Informa Sistemi

---

## 🚨 ERRORE IDENTIFICATO

### Problema
I cavi rosso-nero (audio per casse passive) erano stati erroneamente assegnati alla tratta del **Ristorante P.-1**.

### Perché era un errore
- Al **Ristorante P.-1** ci sono casse audio **MAUI ATTIVE**
- Le casse MAUI attive ricevono segnale audio tramite:
  - **Cavi XLR** (arrivo dopo il 20 gennaio)
  - **Snake Thoman** (cavo LAN con splitter passivi)
- Le casse attive **NON richiedono** amplificatore esterno
- I cavi rosso-nero servono SOLO per casse **PASSIVE** (collegano amplificatore → casse)

---

## ✅ CORREZIONE APPLICATA

### Destinazione Corretta
I cavi rosso-nero servono per la **Galleria ledwall C** (Lounge area):
- **Destinazione:** Casse passive sopra al ledwall C in Galleria
- **Tipo casse:** Fonestar (rettangolari con staffa OR tonde a incasso)
- **Quantità:** 2 cavi da 25m ciascuno (50m totali)

### Configurazione Amplificatore

**OPZIONE 1 - Amplificatore in Regia P.0:**
```
Regia P.0 (Amplificatore)
    ↓
Cavo rosso-nero: 2x 25m (50m totali)
    ↓
Galleria ledwall C
    ↓
Casse passive Fonestar sopra ledwall C
```
- Lunghezza cavi: 2x 25m = 50m totali
- Da tirare il 20 gennaio con Igor

**OPZIONE 2 - Amplificatore sotto bancone bar:**
```
Regia P.0
    ↓
Segnale audio non amplificato (XLR o altro)
    ↓
Sotto bancone bar accanto a ledwall C
    ↓
Amplificatore
    ↓
Cavo rosso-nero: breve (~5-10m)
    ↓
Casse passive sopra ledwall C
```
- Lunghezza cavi: 2x 5-10m (brevi)
- Da decidere in loco in base a layout Henoto

---

## 📋 FILE AGGIORNATI

### 1. INSTALLAZIONE_IGOR_20GEN.md

**Modifiche effettuate:**

#### Sezione 3 - Tratta Ristorante P.-1
- ❌ **RIMOSSO:** CAV-R04 (cavo rosso-nero 2x 30m)
- ✅ **AGGIORNATO:** Totale da ~210-270m a ~150-210m
- ✅ **AGGIUNTA NOTA:** "Al Ristorante P.-1 ci sono casse MAUI **ATTIVE** (NO cavi rosso-nero necessari)"

#### Nuova Sezione 2bis - Galleria ledwall C
- ✅ **AGGIUNTA:** Tratta audio Galleria ledwall C (casse passive)
- ✅ **CODICE:** CAV-LC01 (cavo rosso-nero 2x 25m = 50m tot)
- ✅ **OPZIONI:** 2 configurazioni amplificatore (Regia OR sotto bancone)
- ✅ **DETTAGLI:** Tipo casse, polarità, scelta finale Henoto

#### Riepilogo Materiali
- ✅ **AGGIORNATO:** Descrizione cavi rosso-nero da "Audio casse passive Ristorante" a "Audio casse passive **Galleria ledwall C** (Regia→Galleria OR Bancone bar→Casse)"

### 2. MESSAGGI_WHATSAPP_IGOR.txt (v1.0.02)

**Nuovo file creato con 5 messaggi:**

#### Messaggio 2 - Cavi Audio e BNC
- ✅ **CORRETTO:** "Da Regia P.0 → Galleria ledwall C"
- ✅ **SPECIFICHE:** Audio amplificatore → Casse passive Fonestar sopra ledwall C
- ✅ **OPZIONE 2:** Da bancone bar → Casse se ampli sotto bancone

#### Messaggio 5 - Priorità Percorsi
- ✅ **AGGIUNTA:** Priorità 3 - GALLERIA LEDWALL C (Audio passive)
- ✅ **DETTAGLI:** 2 cavi rosso-nero (50m), verificare posizione amplificatore in loco

---

## 🔧 SISTEMA AUDIO COMPLETO - RIEPILOGO

### Casse ATTIVE (MAUI 28G)
**Locations:** Celebration, Lounge, Ristorante P.-1

**Collegamento:**
- Segnale dal mixer (Regia P.0)
- Tramite cavi **XLR** (arrivo dopo 20 gen)
- Oppure tramite **Snake Thoman** (cavo LAN + splitter passivi)
- **NON richiedono amplificatore esterno**
- **NON richiedono cavi rosso-nero**

### Casse PASSIVE (Fonestar)
**Locations:** Galleria ledwall C, LED Esterno

**Collegamento:**
- Richiedono **amplificatore esterno**
- Amplificatore → Casse tramite **cavi rosso-nero**
- Polarità: nero = -, rosso = +

**Galleria ledwall C:**
- 2 cavi rosso-nero da 25m (se ampli in Regia)
- 2 cavi rosso-nero da 5-10m (se ampli sotto bancone bar)

**LED Esterno:**
- Audio da PC EDV esterno → Amplificatore locale → 2 casse Fonestar

---

## 📊 QUANTITÀ CAVI ROSSO-NERO

### Prima (ERRATO)
- Ristorante P.-1: 2x 30m = 60m
- **TOTALE:** 60m

### Dopo (CORRETTO)
- Galleria ledwall C: 2x 25m = 50m
- **TOTALE:** 50m

**Differenza:** -10m (risparmio)

---

## ✅ CHECKLIST VERIFICA

- [x] Rimosso cavi rosso-nero da tratta Ristorante P.-1
- [x] Aggiunta nota casse MAUI attive al Ristorante
- [x] Creata nuova sezione Galleria ledwall C
- [x] Specificate 2 opzioni posizione amplificatore
- [x] Aggiornato riepilogo materiali
- [x] Creati messaggi WhatsApp corretti (v1.0.02)
- [x] Aggiornate priorità percorsi
- [x] Documentato sistema audio completo (attive vs passive)

---

## 🎯 PROSSIMI PASSI

### Fase 1: Conferma Posizione Amplificatore (Pre-20 Gen)
- [ ] Ricevere layout definitivo da allestitore Henoto
- [ ] Confermare posizione amplificatore:
  - Opzione A: In Regia P.0 (tirare cavi 2x 25m)
  - Opzione B: Sotto bancone bar (tirare cavi brevi 2x 5-10m)

### Fase 2: Installazione 20 Gennaio
- [ ] Igor porta cavi rosso-nero: 2x 25m (50m tot)
- [ ] Passaggio cavi verso Galleria ledwall C
- [ ] Verifica percorso ottimale in loco

### Fase 3: Post-Installazione (Dopo 25 Gen)
- [ ] Arrivo amplificatore
- [ ] Arrivo casse passive Fonestar (scelta modello con Henoto)
- [ ] Montaggio casse sopra ledwall C
- [ ] Collegamento finale amplificatore → casse
- [ ] Test audio sistema completo

---

## 📞 RIFERIMENTI

**Sistema Audio Locations:**
- **Celebration P.0:** MAUI attive (XLR/Snake)
- **Lounge P.0:** MAUI attive (XLR/Snake)
- **Ristorante P.-1:** MAUI attive (XLR/Snake) ← NO cavi rosso-nero
- **Galleria ledwall C:** Fonestar passive (cavi rosso-nero) ← CORREZIONE
- **LED Esterno:** Fonestar passive (locale)

**Cavi Audio:**
- **XLR:** Solo casse attive (arrivo dopo 20 gen)
- **Snake Thoman:** Solo casse attive (LAN + splitter)
- **Rosso-nero:** Solo casse passive (polarità +/-)

---

**Documento di correzione**
**Versione:** 1.0.02
**Data:** 15 Gennaio 2026, ore 10:30
**Responsabile:** Informa Sistemi

---

## 📌 NOTA FINALE

L'errore è stato identificato e corretto prima dell'installazione del 20 gennaio. La documentazione è ora coerente e corretta:

✅ Ristorante P.-1 = Casse MAUI ATTIVE (NO cavi rosso-nero)
✅ Galleria ledwall C = Casse Fonestar PASSIVE (SÌ cavi rosso-nero)

Igor porterà i materiali corretti il 20 gennaio.
