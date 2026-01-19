# ANALISI CALL CON NICOLA FURNARI - 10 Gennaio 2026
## Aggiornamento Stato Progetto Casa Italia Cortina

**Data call:** 10 Gennaio 2026
**Partecipanti:** Maximilian Giurastante, Nicola Furnari (Eventi Streaming 1)
**Documento di riferimento:** RECAP_PROGETTO_CASA_ITALIA_CORTINA.md

---

## 1. AGGIORNAMENTI TECNICI EMERSI DALLA CALL

### 1.1 LED CELEBRATION - BACKUP CONFERMATO NON PRESENTE

| Parametro | Stato Precedente | Aggiornamento Call |
|-----------|------------------|-------------------|
| Cavi LAN Backup | 10 (ipotizzati) | **0 - NESSUN BACKUP** |
| Motivazione | - | MCTRL4K ha solo 16 porte, non 20 |
| Rischio | Basso | LED nuovo (lotto 420), usato una sola volta |
| Mitigazione | - | Tenere sending card di backup pronta dietro il LED |

**Nicola conferma:** "Non abbiamo schede che hanno 20 porte. Il LED e' nuovo, quello con cui faremo la Celebration. Usato una volta. Mettere 2 sending mi sembra eccessivo."

**Decisione:** Si lasciano cavi di backup pronti dietro al LED, collegabili in caso di emergenza.

---

### 1.2 LED LOUNGE - VANO TECNICO E PASSAGGIO CAVI

| Problema | Soluzione Discussa |
|----------|-------------------|
| VMIX e' un PC Tower, non entra in spazi ristretti | Ripiano/mensola sotto il bancone bar |
| Passaggio cavi Regia->Galleria | Sotto moquette (SE presente) oppure extender 4K via rete esistente |
| Spazio tecnico | Unico posto disponibile e' sotto il bancone bar |

**Criticita' emersa:** La Galleria Farsetti ha un IT locale poco affidabile ("un negozietto di montagna che ripara computer"). Non conviene affidarsi all'infrastruttura esistente.

**Soluzione proposta:**
- Verificare con Greta se c'e' moquette in Galleria
- Se si', passare cavi PRIMA della posa (sotto moquette)
- Utilizzare extender 4K per la tratta lunga
- Chiedere a Henoto mensola/vano sotto bancone per PC sending + MCTRL4K

---

### 1.3 STREAMING GARE - ARCHITETTURA CHIARITA

Il sistema di streaming gare funziona cosi':

```
MiniPC Windows (WIN1-4)
    |
    +-- Browser (Discovery Plus / RAI)
    |
    +-- Fullscreen sul canale
    |
    v
Encoder Kiloview
    |
    +-- Trasforma HDMI in link locale IP
    |
    v
Switch 24 porte (rete locale)
    |
    +-- Link accessibile da tutti i VMIX
    |
    v
VMIX 1/2/3
    |
    +-- Mettono il link come sorgente
```

**Vantaggio:** Verso internet si usano pochi mega per canale. Internamente si puo' saturare fino a 1 Gbps.

**Costi banda:**
- Internet: ~5-10 Mbps per canale (streaming Discovery/RAI)
- Rete locale: fino a 1 Gbps disponibile per distribuzione interna

---

### 1.4 PASSAGGIO CAVI PIANO 0 -> PIANO -1 (CRITICITA' PRINCIPALE)

| Opzione | Fattibilita' | Note |
|---------|--------------|------|
| Porta vetro | RISCHIO MURATA | Da verificare con Henoto |
| Finestra | Possibile | Ma rimane aperta col freddo? |
| Cappa cucina | **PROPOSTA** | Da verificare con HENOTO - lavori NON ancora iniziati |

**Proposta d'azione (DA CONFERMARE):**
1. Verificare con HENOTO se/quando bucheranno per la cappa
2. Se confermato, sfruttare lo stesso passaggio per i nostri cavi
3. Mandare Igor quando iniziano l'impianto elettrico con bobine di rete

**⚠️ STATO: PROPOSTA - Da verificare nella call con HENOTO Lunedi' 13/01 ore 12:00**

**Nicola:** "Io vorrei, siccome loro dovranno bucare per la cappa, usare lo spazio che dovranno fare per uscire con la cappa."

---

## 2. LOGISTICA E MATERIALI

### 2.1 Arrivo Materiali

| Materiale | Origine | Destinazione | Data |
|-----------|---------|--------------|------|
| Moduli COB 45 gradi | Vixel (sdoganamento Milano) | Cortina via HHENOTO | ~15 Gennaio |
| LED SEGNA noleggio | Sedico | Magazzino IS | 15 Gennaio |
| AMIL BLUE 3.9 | CTV (gia' in magazzino) | Cortina | Col resto |

**Spedizione generale:** Tutto viene mandato a HHENOTO (Padova), che poi porta a Cortina secondo cronoprogramma.

### 2.2 Rack Pre-assemblati

**CONFERMATO:** Nicola preparera' i rack gia' questa settimana con tutti i collegamenti interni. In cantiere si dovranno solo fare i collegamenti esterni.

**Nicola:** "Cercherò di preparare i rack già pronti. Non deve installare il rack, li deve solo aprire e fare i collegamenti esterni."

### 2.3 Sala Stampa - Opzioni TV

| Opzione | Pro | Contro |
|---------|-----|--------|
| Monitor IS + Decoder Edison | Gia' in magazzino | Da verificare disponibilita' |
| Acquisto 2 TV | Decoder interno | Costo aggiuntivo |

**Azione:** Nicola verifica se ci sono televisori in magazzino. Se no, si valuta acquisto.

### 2.4 PTZ - Correzione Quantita'

| Stato precedente | Aggiornamento |
|------------------|---------------|
| 3x PTZ ZTA | **1x PTZ ZTA confermata** (da recuperare ad Assisi) |

---

## 3. TEMPISTICHE E CANTIERE

### 3.1 Date Chiave Confermate/Aggiornate

| Data | Attivita' | Note |
|------|-----------|------|
| **15 Gennaio** | LED SEGNA arriva in magazzino | Da Sedico |
| **Settimana 20-24 Gen** | Igor fa sopralluogo con bobine rete | Quando inizia impianto elettrico |
| **25 Gennaio** | Inizio cantiere IS | Confermato obiettivo |
| **26 Gennaio** | Igor sale con 2 persone | Per iniziare installazione |
| **4 Febbraio PM** | DEADLINE - Servizio fotografico | Tutto deve essere pronto |
| **5 Febbraio** | Ultimi settaggi possibili | - |
| **6 Febbraio AM** | Ultimi ritocchi | - |
| **6 Febbraio PM** | Cerimonia apertura - LIVE | Deadline assoluta |

### 3.2 Alloggio Team

| Dettaglio | Valore |
|-----------|--------|
| Casa | Andrea Marini (architetto, amico di Andrea) |
| Posizione | 300m dopo la Galleria Farsetti |
| Posti letto | 6 |
| Garage | Si' (utile per furgone Igor) |

**Nota:** Maximilian conosce personalmente Andrea Marini.

### 3.3 Viaggio Maximilian

- **23 Gennaio:** Salita a Cortina (treno fino a Mestre + Cortina Express)
- **24-25 Gennaio:** Da Mestre a Cortina con Igor o Cortina Express
- Possibilita' ospitare anche Paola se vuole salire dopo Carnevale (20+)

---

## 4. STAKEHOLDER E RUOLI

### 4.1 Mappa Attori Chiarita

```
CONI (Committente)
    |
    v
IT'S (Studio Progettazione)
    |-- Render
    |-- Capitolato di gara
    |
    v
HENOTO (General Contractor)
    |-- Strutture
    |-- Direzione cantieri
    |-- Parte elettrica
    |-- Falegnameria (zoccoli LED)
    |
    v
HENOTO (Coordinamento)
    |-- Greta Gobbo (PM Cortina)
    |
    v
INFORMA SISTEMI (AV/LED/Streaming)
    |-- Nicola Furnari (Coord.)
    |-- Maximilian Giurastante (PM)
    |-- Igor Matiuzzi (Installatore)
    |-- Flavia Falanga (Tecnico regia)
```

### 4.2 Video Riprese

| Fornitore | Copertura |
|-----------|-----------|
| NEXTHING | 50% (amici di Tommaso Palmieri) |
| STAND BY ME | 50% (stessi del Rio) |

### 4.3 Contatti da Richiedere

Nicola scrivera' una mail stasera con:
- Contatti delle varie ditte nei cantieri
- Informazioni sui referenti di ogni area
- Aggiornamenti su Maglione Elettronica (predisposizioni dietro LED)

---

## 5. CRITICITA' E AZIONI

### 5.1 Criticita' Aperte

| # | Criticita' | Owner | Priorita' | Azione |
|---|------------|-------|-----------|--------|
| 1 | HHENOTO non ha mai confermato per iscritto | Nicola | ALTA | Ottenere conferma scritta |
| 2 | Passaggio cavi P.0->P.-1 | Nicola/Greta | ALTA | **PROPOSTA:** cappa cucina - DA VERIFICARE call 13/01 |
| 3 | Connettivita' ADSL insufficiente | Nicola | MEDIA | Sollecitare risposta |
| 4 | Moquette Galleria da confermare | Greta | MEDIA | Verificare lunedi' |
| 5 | PTZ ZTA ad Assisi | Nicola | BASSA | Recuperare o far spedire |

### 5.2 Preoccupazione Principale di Nicola

**Rassicurazioni verbali da HHENOTO:** Nicola e' preoccupato perche' ha sempre parlato con HHENOTO al telefono ma non ha mai ricevuto conferme scritte via mail sugli accordi presi.

**Nicola:** "Ho sempre avuto delle rassicurazioni verbali, capito? E li' sto un po'... sono un po' preoccupato."

**Azione:** Mandare mail riepilogativa a HHENOTO chiedendo conferma scritta di tutti gli accordi.

---

## 6. ACTION ITEMS POST-CALL

### 6.1 Azioni Nicola (Eventi Streaming)

- [x] Aggiornare documento con info garante (fatto prima della call)
- [ ] Rivedere Gantt finale con Greta entro lunedi'
- [ ] Verificare televisori in magazzino per sala stampa
- [ ] Preparare rack questa settimana con tutti i collegamenti
- [ ] Recuperare PTZ ZTA da Assisi
- [ ] Aggiornare quantita' cavi e lunghezze nell'Excel
- [ ] Completare liste materiali per preparazione
- [ ] Scrivere mail stasera con contatti ditte cantieri
- [ ] Mandare Igor a Cortina con bobine rete quando inizia impianto elettrico
- [ ] Far salire Igor con 2 persone dal 26 per iniziare installazione
- [ ] Organizzare logistica per far arrivare Flavia a Mestre
- [ ] Verificare con Maglione Elettronica predisposizioni dietro ogni LED
- [ ] Coordinare con HHENOTO per conferma scritta accordi verbali

### 6.2 Azioni Maximilian

- [ ] Salire a Cortina il 23, essere a Mestre il 24 o 25
- [ ] Verificare con HHENOTO l'inizio lavori dal 25
- [ ] Condividere cronoprogramma dettagliato con HHENOTO
- [ ] Verificare questione connettivita'/ADSL con tempi necessari

### 6.3 Azioni Congiunte

- [ ] Verificare passaggio cavi con Greta (moquette Galleria?)
- [ ] Verificare possibilita' passaggio cavi via cappa cucina

---

## 7. CONFRONTO STATO PROGETTO

### 7.1 Cosa e' Cambiato

| Aspetto | Prima della Call | Dopo la Call |
|---------|------------------|--------------|
| Backup LED Celebration | 10 cavi previsti | 0 cavi (non necessario) |
| PTZ ZTA | 3 unita' | 1 unita' confermata |
| Vano tecnico Lounge | Da definire | Sotto bancone bar |
| Architettura streaming | Generica | Chiarita (MiniPC->Kiloview->Rete) |
| Passaggio cavi P.-1 | Problema aperto | Soluzione: cappa cucina |
| Alloggio team | Da trovare | Casa Andrea Marini (6 posti) |
| Data inizio cantiere | Richiesto 25/1 | Confermato obiettivo 25/1 |

### 7.2 Cosa Rimane Invariato

- Deadline 4 Febbraio (foto) / 6 Febbraio (apertura)
- 4 LED Wall totali (3 interni + 1 esterno)
- Configurazione VMIX (3 postazioni)
- Sending card (3x MCTRL4K + 1x MTCRL300)
- Team (Max, Flavia, Igor + 2 supporto)

### 7.3 Nuovi Rischi Identificati

| Rischio | Probabilita' | Impatto | Mitigazione |
|---------|--------------|---------|-------------|
| HHENOTO non conferma per iscritto | Media | Alto | Sollecitare mail di conferma |
| IT Galleria inaffidabile | Alta | Medio | Non usare infrastruttura esistente |
| Connettivita' ADSL | Alta | Alto | Verificare tempi attivazione alternative |

---

## 8. PROSSIMI PASSI

1. **Lunedi' 13 Gennaio:** Call con Greta per rivedere Gantt e confermare moquette
2. **Questa settimana:** Nicola prepara rack e aggiorna Excel
3. **Settimana prossima (20-24 Gen):** Igor sopralluogo con bobine
4. **23 Gennaio:** Maximilian parte per Mestre
5. **25-26 Gennaio:** Inizio cantiere IS

---

**Documento redatto da:** AI Assistant
**Data:** 10 Gennaio 2026
**Versione:** 1.0

---

*Questo documento integra le informazioni emerse dalla call del 10 gennaio 2026 con lo stato progetto documentato in RECAP_PROGETTO_CASA_ITALIA_CORTINA.md*
