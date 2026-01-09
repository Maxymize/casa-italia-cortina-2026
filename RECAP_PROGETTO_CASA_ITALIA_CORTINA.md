# CASA ITALIA - CORTINA 2026
## DOCUMENTO DI RECAP GENERALE DEL PROGETTO

**Data documento:** 9 Gennaio 2026
**Project Manager Informa Sistemi:** Maximilian Giurastante (320.02.37.200)
**Referente Henoto Cortina:** Greta Gobbo (g.gobbo@henoto.com - 348.694.7549)
**Coordinamento Generale:** Nicola Furnari (n.furnari@informasistemi.com)

---

## 1. OVERVIEW PROGETTO

### 1.1 Contesto
Casa Italia per le Olimpiadi Invernali Milano-Cortina 2026 sara' distribuita su **3 location**:
- **Milano** - Triennale (coordinamento generale)
- **Cortina** - Galleria Farsetti (Piazza Roma 10, Cortina d'Ampezzo)
- **Livigno** - Centro Sportivo Acquagranda

### 1.2 Scope Informa Sistemi per Cortina
- Installazione LED Wall (4 totali: 3 interni + 1 esterno)
- Impianti audio in tutte le aree
- Passaggio cavi e infrastruttura di rete
- Regia video centralizzata
- Monitor sala stampa
- Connettivita' e telecamere PTZ per collegamenti inter-house

### 1.3 Location Cortina - Galleria Farsetti
Struttura su **due piani** + tensostruttura esterna:
- **Piano 0:** Galleria Lounge, Spazio Regia, Spazio Interviste, Padiglione (Celebration)
- **Piano -1:** Ristorante (ex Esselunga), Casa Giornalisti, Deposito, Locale Preparazione

---

## 2. INSTALLAZIONI LED - DETTAGLIO TECNICO

### 2.1 LED CELEBRATION (Tensostruttura esterna - Padiglione)
| Parametro | Valore |
|-----------|--------|
| **Codice** | LED03 |
| **Tipologia** | COB 1.5 indoor (nuovo ordine lotto 420) |
| **Dimensioni** | 6 x 2.36m |
| **Risoluzione** | 3840 x 1536 px |
| **Controller** | MCTRL4K |
| **Software** | VMIX 1 |
| **Moduli** | 10 colonne da 7 moduli (premontaggio: 10x4 + 10x3) |
| **Alimentazione** | Quadro 32A pentapolare (5x16A) |
| **Audio** | 2x MAUI + casse eventualmente a incasso |
| **Montaggio** | Su parete legno con viti, manutenzione frontale |
| **Altezza da terra** | ~15cm (zoccolo) |

### 2.2 LED LOUNGE - Galleria Piano 0 (Configurazione a C)
| Parametro | Valore |
|-----------|--------|
| **Codice** | LED02 + LED04 |
| **Tipologia** | COB 1.5 con angolari 45 gradi |
| **Dimensioni** | Parete lunga: 2.4 x 2.7m / Lato corto: 1.8 x 2.7m (o 1.2 x 2.7m) |
| **Risoluzione** | LED02: 1152 x 1728 px / LED04: 1536 x 1728 px |
| **Controller** | MCTRL4K |
| **Software** | VMIX 3 |
| **Moduli** | 10 colonne da 8 moduli (premontaggio: 12x4 dritti + 4x4 SX + 4x4 DX) |
| **Alimentazione** | 3x16A (minimo 2 prese) |
| **Partenze** | 10 corrente + 18 LAN |
| **Note** | Necessario vano ispezionabile per PC sending e controller 2U. Moduli tagliati a 45 gradi in arrivo settimana prossima |

### 2.3 LED RISTORANTE Piano -1 (Ex Esselunga)
| Parametro | Valore |
|-----------|--------|
| **Codice** | LED01 - SEGNA |
| **Tipologia** | Passo 2.6 indoor (LED a noleggio Sedico) |
| **Dimensioni** | 6 x 2.5m |
| **Risoluzione** | 2304 x 960 px |
| **Controller** | MCTRL4K |
| **Software** | VMIX 2 |
| **Moduli** | Rental 500x1000mm + 500x500mm |
| **Alimentazione** | 5x16A o 32A pentapolare (~11kW + audio) |
| **Audio** | 2x MAUI |
| **Montaggio** | Su truss o staffe a C su parete (spessore 25-30cm) |
| **Note** | Opzione parete dedicata 7x2.5m con casse incassate ai lati. Ispezione lato cucina o corridoio camerieri |

### 2.4 LED ESTERNO (Piazzale)
| Parametro | Valore |
|-----------|--------|
| **Codice** | LED06 |
| **Tipologia** | AMIL BLUE passo 3.9 outdoor (sostituzione BLADE) |
| **Dimensioni** | 3 x 2m |
| **Risoluzione** | 768 x 512 px |
| **Controller** | MTCRL300 |
| **Moduli** | Rental 500x1000mm |
| **Alimentazione** | 2x16A (~4kW) |
| **Audio** | 2x Fonestar + Amplificatore Monacor |
| **Montaggio** | Su truss/layher (struttura condivisa con Pascucci per luci) |
| **Altezza da terra** | ~1m |
| **Hardware** | Connessioni aliscaf e tubolari 2" (fornitura IS) |

**Materiale struttura LED esterno da preparare:**
- 4 pali da 2m
- 3 pali da 3m
- 6 pali da 1m
- 10 aliscaf singoli
- 16 aliscaf doppi

### 2.5 SALA STAMPA (Casa Giornalisti Piano -1)
| Parametro | Valore |
|-----------|--------|
| **Codice** | LED05 |
| **Tipologia** | 2x Monitor TV 55" su stand da tavolo |
| **Contenuti** | RAI Sport e RAI 2 (fissi) |
| **Note** | Verificare presenza presa internet e antenna TV nella stanza |

---

## 3. SCHEMA REGIA VIDEO

### 3.1 Configurazione Hardware Regia
La regia e' posizionata al **Piano 0 - Spazio Regia (C.PT.17)**, nell'area esterna dopo lo Studio TV.

**Postazioni VMIX (PC con software VMIX per regia video e gestione contenuti):**
| Postazione | LED Gestiti | Monitor | Uscita Video | Sending Card |
|------------|-------------|---------|--------------|--------------|
| VMIX 1 | LED03 (Celebration) | MON1 27" | HDMI -> MCTRL4K | MCTRL4K (3840x1536px) |
| VMIX 2 | LED01 (Ristorante -1) | MON2 27" | HDMI -> MCTRL4K | MCTRL4K (2304x960px) |
| VMIX 3 | LED02/LED04 (Galleria) | MON3 | HDMI -> MCTRL4K | MCTRL4K (2688x1728px tot) |

**MiniPC Windows (WIN1-WIN4) - Streaming Gare:**
- 4x MiniPC per trasmettere canali gare (Discovery/RAI) sugli schermi
- 4x Encoder Kiloview per codifica video HDMI/SDI -> IP (NDI, SRT, RTMP, H.264/H.265)
- Supporto 4K, streaming su rete IP/WiFi/4G-5G

**Sending Card (Controller LED):**
| Controller | LED | Risoluzione | Cavi LAN Main | Cavi LAN Backup |
|------------|-----|-------------|---------------|-----------------|
| MCTRL4K #1 | LED03 Celebration | 3840x1536px | 10 (frecce verdi) | 10 (frecce arancio) |
| MCTRL4K #2 | LED01 Ristorante | 2304x960px | 5 | 5 |
| MCTRL4K #3 | LED02+LED04 Lounge | 1152+1536x1728px | 12 | 12 |
| MTCRL300 | LED06 Esterno | 768x512px | 1 | 1 |

*Nota: Le sending card MCTRL convertono segnale HDMI in uscita LAN Cat.5 per i moduli LED. Il backup garantisce continuita' del segnale in caso di guasto linea principale.*

**Telecamere PTZ:**
- 3x PTZ 4K per comunicazione inter-house (collegamento con Milano e Livigno)
- Collegamento: Cavo BNC -> Schede acquisizione video PC VMIX
- Posizionamento: davanti Celebration e/o Lounge
- Il segnale BNC viene acquisito dalle schede video dei PC VMIX

**Extender Video per lunghe distanze:**
- Extender HDMI/LAN (trasmitter + receiver) per tratte lunghe
- Bobine fibra ottica con connettori HDMI per segnali ad alta qualita'

### 3.2 Flusso Segnali Audio
```
MIXER BEHRINGER (centrale in regia)
    |
    +-- LR (Main Out) --> Cavo XLR --> MAUI 28G Celebration (casse attive a colonna)
    +-- AUX 1 --> Cavo XLR --> Speaker SSSNAKE Galleria
    +-- AUX 2 --> Cavo XLR --> MAUI 28G Lounge (casse attive a colonna)
```

**Tipologie Audio:**
- **MAUI 28G (LD Systems)**: Casse attive a colonna, segnale via cavo XLR
- **Fonestar**: Speaker passivi a parete, richiedono amplificatore (Monacor per LED esterno)
- **Schede Audio USB**: 3x collegate ai PC VMIX per gestione audio software

### 3.3 Flusso Segnali Video Completo
```
SORGENTI VIDEO
    |
    +-- MiniPC WIN1-4 (streaming gare) --> Encoder Kiloview --> Rete IP --> Switch
    +-- Telecamere PTZ --> BNC --> Schede acquisizione --> PC VMIX
    |
PC VMIX (regia e gestione contenuti)
    |
    +-- HDMI Out --> MCTRL4K (Sending Card)
                        |
                        +-- LAN Cat.5 Main (frecce verdi) --> Moduli LED
                        +-- LAN Cat.5 Backup (frecce arancio) --> Moduli LED
```

**Rete Intranet Allestimento:**
- Switch 24 porte centrale in regia
- Convoglia tutta la rete interna (VMIX, MiniPC, Encoder, Controller)
- Uscita internet: connessione dedicata (Eolo/Starlink) + esistente location

---

## 4. CRITICITA' IDENTIFICATE

### 4.1 Passaggi Cavi (URGENTE - da risolvere con Henoto)
| Tratta | Problematica | Soluzione proposta |
|--------|--------------|-------------------|
| Regia --> Piano -1 | Porta a vetro potrebbe essere murata. Come portare segnali giu'? | Verificare con impianti aria/aerazione. Passaggio finestra o aperture cucina/cappa |
| Regia --> LED a C (Piano 0) | Percorso da definire | Passaggio battiscopa/galleria (gia' cablata) |
| Regia --> LED Celebration | Struttura esterna | Treccia 12/14 cavi Nitto per cavo singolo, 20m |
| Sotto moquette | Tempistiche critiche | Coordinare PRIMA della posa moquette (2 febbraio) |

### 4.2 Tempistiche Critiche
- **Ingresso cantiere previsto da Henoto:** 29 Gennaio (TROPPO TARDI)
- **Ingresso richiesto IS:** 25-26 Gennaio
- **Tempo stimato per LED:** 1.5-2 giorni ciascuno
- **Deadline installazioni:** 4 Marzo sera (tutto testato per servizio fotografico)
- **Cerimonia apertura:** 6 Marzo pomeriggio

### 4.3 Criticita' da Smarcare con Greta (Henoto)
1. Passaggio cavi tra regia e piano -1 (ex esselunga)
2. Passaggio cavi tra regia e LED a C piano 0
3. Verifica presa internet/antenna TV in sala giornalisti
4. Passaggio cavi tra regia e LED celebration
5. Posizionamento quadri elettrici (16A singole vs 32A pentapolare)
6. Mensola/vano per tecnica LED a C (ripiano bancone bar o vano dedicato)
7. Decisione casse: tipo Ara Pacis o incasso (disponibili 10-15cm)
8. Verifica cronoprogramma e consegna strutture
9. **Richiesta call congiunta per allineamento**

### 4.4 Connettivita' (Criticita' Rete)
- Rete Galleria Farsetti insufficiente (~100 Mbps)
- **Opzioni valutate:**
  - Ponte radio dedicato: 500 Mbps simmetrici (difficile, realisticamente 200 Mbps)
  - Eolo: ~500 euro/mese per 200 Mbps
  - Starlink residenziale: 40 euro/mese (aziendale 300-400 euro/mese)
- **Decisione:** Procedere con scouting Eolo/Starlink come backup
- Setup: WiFi in Lounge, VLAN/Firewall per gestione banda

### 4.5 LED Esterno
- Rischio neve durante installazione
- Manca nel cronoprogramma Henoto
- Da schedulare con priorita' weather-dependent

---

## 5. CRONOPROGRAMMA

### 5.1 Timeline Generale
| Data | Milestone |
|------|-----------|
| 15-16 Gennaio | Inizio lavori strutture Cortina |
| 22-23 Gennaio | Inizio montaggi generali |
| **25-26 Gennaio** | **Ingresso IS in cantiere (richiesto)** |
| 29 Gennaio | Ingresso IS previsto da Henoto (da anticipare) |
| 2 Febbraio | Posa moquette Celebration |
| 4 Marzo sera | **DEADLINE: tutto testato e funzionante** |
| 5 Marzo | Setup finale |
| **6 Marzo PM** | **Cerimonia di apertura - tutti schermi su Discovery** |

### 5.2 Fasi Lavoro IS (da schedulare nel dettaglio)
1. **Passaggio cavi** (prima della moquette - entro 1 febbraio)
2. **Installazione LED Esterno** (weather-dependent, priorita' alta)
3. **Installazione LED Celebration** (~1.5-2 giorni)
4. **Installazione LED Lounge/Galleria** (~1.5-2 giorni)
5. **Installazione LED Ristorante -1** (~1.5-2 giorni)
6. **Setup Regia** (~1 giorno)
7. **Cablaggio e test audio** (~1 giorno)
8. **Test completo sistema** (~1 giorno)

---

## 6. TEAM E CONTATTI

### 6.1 Team Informa Sistemi Cortina
| Ruolo | Nome | Contatto |
|-------|------|----------|
| Project Manager | Maximilian Giurastante | 320.02.37.200 / m.giurastante@informasistemi.com |
| Tecnico Senior | Flavia Falanga | - |
| Tecnico | Igor | - |
| Coordinamento | Nicola Furnari | n.furnari@informasistemi.com |

### 6.2 Team Henoto
| Ruolo | Nome | Contatto |
|-------|------|----------|
| PM Cortina | Greta Gobbo | 348.694.7549 / g.gobbo@henoto.com |
| PM Milano | Alberto Guglielmo | - |
| PM Livigno | Claudio Rigoletto | - |

### 6.3 Altri Riferimenti
| Azienda/Ruolo | Nome | Note |
|---------------|------|------|
| Committente | CONI | Piazza Lauro de Bosis 15, Roma |
| Progettazione Architettonica | IT'S | Via Ignazio Pettinengo 72, Roma |
| Luci Outdoor | Pascucci | Struttura condivisa LED esterno |

---

## 7. MATERIALI E FORNITURE

### 7.1 LED e Controller
- LED COB 1.5: nuovo ordine lotto 420 (Celebration)
- LED COB 1.5 con angolari 45: in arrivo settimana prossima
- LED AMIL BLUE: sostituzione BLADE (flight case con bollino fucsia da CTV)
- LED SEGNA 2.6: noleggio da Sedico
- Controller: 3x MCTRL4K + 1x MTCRL300

### 7.2 Audio
- Casse MAUI (multiple postazioni)
- Casse Fonestar (LED esterno)
- Amplificatore Monacor (LED esterno)
- Mixer Behringer centrale
- Opzione casse a incasso (da decidere)

### 7.3 Cavi e Connessioni (da quantificare)
- Cavi BNC per telecamere
- Rulli cavo di rete
- Treccia Nitto 12/14 cavi (20m per Celebration)
- Fibre ottiche
- Prolunghe elettriche
- Switch di rete

### 7.4 Hardware Regia
- 3x VMIX (XL per gestione LED con skin Excel real-time)
- 4x MiniPC Windows
- 4x Encoder
- 3x Monitor 27"
- 3x Schede Audio
- Switch di rete

### 7.5 Connettivita'
- Account Discovery Plus (~30 da Matteo Pacor)
- Segnale 4K: 2x DriveSign da Discovery
- Firewall disponibile per gestione banda
- PTZ 4K: 3-5 unita' (verificare inventario)

---

## 8. ACTION ITEMS IMMEDIATI

### Alta Priorita' (entro 10 Gennaio)
- [ ] Schedulare call con Greta Gobbo per criticita' Cortina
- [ ] Creare cronoprogramma interno IS colorato
- [ ] Verificare disponibilita' materiali LED (soprattutto angolari COB)
- [ ] Confermare ingresso cantiere anticipato (25-26 gennaio)

### Media Priorita' (entro 15 Gennaio)
- [ ] Definire percorsi cavi con piantine dettagliate
- [ ] Quantificare esattamente cavi necessari
- [ ] Verificare con Nicola se monitor/audio arrivano gia' cablati
- [ ] Contattare Eolo per preventivo connettivita'
- [ ] Verificare Starlink come backup

### Da Monitorare
- [ ] Arrivo moduli COB tagliati a 45 gradi
- [ ] Conferma LED a noleggio Sedico (2.6 ristorante)
- [ ] Test flight case AMIL BLUE (bollino fucsia)
- [ ] Meteo Cortina per pianificazione LED esterno

---

## 9. LISTA MATERIALI DETTAGLIATA PER AMBIENTE

### 9.1 REGIA (Piano 0 - Spazio C.PT.17)

#### PC VMIX (Regia Video e Gestione Contenuti)
| Materiale | Quantita' | Flight Case | Funzione | Stato |
|-----------|-----------|-------------|----------|-------|
| PC VMIX 1 | 1 | CORT12 | Regia LED03 Celebration | Confermato |
| PC VMIX 2 | 1 | CORT12 | Regia LED01 Ristorante | Confermato |
| PC VMIX 3 | 1 | - | Regia LED02+LED04 Lounge | Confermato |
| Schede video acquisizione (BNC/HDMI) | 3 | CORT12 | Ingressi telecamere PTZ | Confermato |
| Monitor 27" (MON1, MON2, MON3) | 3 | - | Preview/Program per operatore | Confermato |

*I PC VMIX hanno schede video con ingressi BNC/HDMI per acquisire segnali telecamere e uscite HDMI verso le sending card*

#### MiniPC Windows (Streaming Gare)
| Materiale | Quantita' | Flight Case | Funzione | Stato |
|-----------|-----------|-------------|----------|-------|
| MiniPC Windows (WIN1-WIN4) | 4 | CORT12 | Streaming canali Discovery/RAI | Confermato |
| Encoder Kiloview | 4 | CORT12 | Codifica HDMI/SDI->IP (NDI/SRT/RTMP) | Confermato |

*Gli encoder trasformano segnali video in flussi IP per streaming su rete, supporto 4K e H.265*

#### Sending Card (Controller LED)
| Materiale | Quantita' | LED Gestito | Ingresso | Uscita | Stato |
|-----------|-----------|-------------|----------|--------|-------|
| MCTRL4K #1 | 1 | LED03 Celebration | HDMI da VMIX1 | 10+10 LAN Cat.5 | Confermato |
| MCTRL4K #2 | 1 | LED01 Ristorante | HDMI da VMIX2 | 5+5 LAN Cat.5 | Confermato |
| MCTRL4K #3 | 1 | LED02+04 Lounge | HDMI da VMIX3 | 12+12 LAN Cat.5 | Confermato |
| MTCRL300 | 1 | LED06 Esterno | HDMI/EDV | 1+1 LAN Cat.5 | Confermato |

*Le sending card convertono HDMI in segnale LAN Cat.5 per i moduli LED. Linee backup (arancio) per continuita'*

#### Hardware Audio
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Mixer Behringer | 1 | Centrale - LR/AUX1/AUX2 | Confermato |
| Schede Audio USB | 3 | Una per ogni PC VMIX | Confermato |
| Ricevitore Microfoni JTS | 1 | CORT12 - wireless | Confermato |

#### Rete e Connessioni
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Switch 24 porte | 1 | Hub centrale intranet allestimento | Confermato |
| Mensole rack | 2 | Per apparati | Confermato |
| Prese 220V rack | 2 | - | Confermato |

#### Telecamere PTZ (Inter-house Milano/Livigno)
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| PTZ 4K | 3 | Collegamento BNC -> schede acquisizione VMIX | Confermato |
| Cavi BNC (telecamere) | 3 | ~20m ciascuno (PTZ->Regia) | **DA QUANTIFICARE lunghezza** |

#### Cavi e Collegamenti REGIA
| Tipo Cavo | Quantita' | Tratta | Stato |
|-----------|-----------|--------|-------|
| Cavo HDMI | 3 | VMIX -> MCTRL4K (sending) | **DA VERIFICARE** |
| Cavo HDMI | 3 | VMIX -> Monitor 27" | **DA VERIFICARE** |
| Cavo BNC | 3 | PTZ -> Schede acquisizione VMIX | **DA QUANTIFICARE** |
| Cavo XLR | 3 | Schede Audio -> Mixer Behringer | **DA VERIFICARE** |
| Cavo LAN Cat.6 | ~10 | MiniPC/Encoder -> Switch | **DA QUANTIFICARE** |
| Extender HDMI/LAN | 2-4 set | Trasmitter+Receiver per tratte lunghe | **DA VERIFICARE necessita'** |
| Bobine fibra ottica HDMI | - | Per segnali alta qualita' lunghe distanze | **DA VERIFICARE necessita'** |

#### ⚠️ MATERIALI MANCANTI/DA VERIFICARE - REGIA
- [ ] Quantita' e lunghezza esatta cavi BNC per telecamere PTZ
- [ ] Cavi HDMI corti per VMIX->Sending e VMIX->Monitor
- [ ] Cavi XLR per collegamento schede audio-mixer
- [ ] Cavi LAN per MiniPC/Encoder verso Switch
- [ ] Necessita' extender HDMI/LAN per tratte lunghe
- [ ] Necessita' fibra ottica HDMI
- [ ] Alimentatori/ciabatte per tutti i dispositivi
- [ ] Rack o struttura per alloggiamento apparati (2U per controller)

---

### 9.2 TENSOSTRUTTURA CELEBRATION (LED03 - Piano 0)

#### LED Wall (3840x1536px)
| Materiale | Quantita' | Flight Case | Stato |
|-----------|-----------|-------------|-------|
| Moduli COB 1.5 (600x337.5mm) | 70 | Bancale COB1.5 | Nuovo lotto 420 |
| - Premontaggio 10 colonne x 4 moduli | 40 | - | Da premontare |
| - Premontaggio 10 colonne x 3 moduli | 30 | - | Da premontare |
| Tail A (cavi alimentazione moduli) | 320+spare | 5 pezzi x flight case | Confermato |
| Partenze corrente | 10 | - | Confermato |

#### Segnale Video (da Regia)
| Materiale | Quantita' | Tratta | Stato |
|-----------|-----------|--------|-------|
| Cavi LAN Cat.5 Main | 10 | MCTRL4K (Regia) -> Moduli LED | ~20m ciascuno |
| Cavi LAN Cat.5 Backup | 10 | MCTRL4K (Regia) -> Moduli LED | ~20m ciascuno |
| Treccia Nitto 12/14 cavi | 1 | Fascio unico per passaggio battiscopa | 20m - Confermato |
| Extender HDMI/LAN (opzionale) | 1 set | Se distanza >30m | **DA VERIFICARE** |

*La sending card MCTRL4K in regia converte HDMI->LAN. I cavi arrivano ai moduli lungo battiscopa*

#### Audio
| Materiale | Quantita' | Flight Case | Collegamento | Stato |
|-----------|-----------|-------------|--------------|-------|
| MAUI 28G (LD Systems) | 2 | CORT11 | Cavo XLR da Mixer LR | Confermato |
| Casse a incasso (opzionali) | 2 | - | XLR | **DA DECIDERE** (10-15cm disp.) |

#### Cablaggio Audio
| Materiale | Quantita' | Tratta | Stato |
|-----------|-----------|--------|-------|
| Cavo XLR | 2 | Mixer Behringer (LR) -> MAUI 28G | ~20m - **DA QUANTIFICARE** |

#### Alimentazione
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Quadro 32A pentapolare | 1 | Oppure 5x16A (~7kW LED + audio) | **DA CONFERMARE posizione** |

#### ⚠️ MATERIALI MANCANTI/DA VERIFICARE - CELEBRATION
- [ ] Lunghezza esatta 20 cavi LAN Cat.5 (10 main + 10 backup)
- [ ] 2x Cavi XLR ~20m per MAUI (da mixer LR)
- [ ] Viti/tasselli per montaggio su parete legno
- [ ] Zoccolo 15cm per rialzo da terra
- [ ] Staffaggio/supporti per moduli LED
- [ ] Canaline passacavi per percorso battiscopa
- [ ] Verifica necessita' extender HDMI/LAN

---

### 9.3 GALLERIA LOUNGE (LED02 + LED04 - Piano 0)

#### LED Wall Configurazione a C (LED02: 1152x1728px + LED04: 1536x1728px)
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Moduli COB 1.5 dritti (600x337.5mm) | 48 | 12 colonne x 4 moduli | Confermato |
| Moduli COB 1.5 angolo 45° SX | 16 | 4 colonne x 4 moduli | **IN ARRIVO settimana prossima** |
| Moduli COB 1.5 angolo 45° DX | 16 | 4 colonne x 4 moduli | **IN ARRIVO settimana prossima** |
| Tail A (cavi alimentazione moduli) | 320+spare | - | Confermato |
| Partenze corrente | 10 | - | Confermato |

#### Segnale Video (da Regia)
| Materiale | Quantita' | Tratta | Stato |
|-----------|-----------|--------|-------|
| Cavi LAN Cat.5 Main | 12 | MCTRL4K (Regia) -> Moduli LED | ~15m ciascuno |
| Cavi LAN Cat.5 Backup | 12 | MCTRL4K (Regia) -> Moduli LED | ~15m ciascuno |
| Extender HDMI/LAN (opzionale) | 1 set | Se necessario | **DA VERIFICARE** |

*La sending card MCTRL4K gestisce entrambi LED02 e LED04. Totale 24 cavi LAN (12 main + 12 backup)*

#### Controller e Sending (in loco)
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| MCTRL4K | 1 | In vano tecnico locale | Confermato |
| PC Sending | 1 | In vano ispezionabile | Confermato |
| Cavo HDMI | 1 | PC Sending -> MCTRL4K | **DA VERIFICARE** |

#### Audio
| Materiale | Quantita' | Collegamento | Stato |
|-----------|-----------|--------------|-------|
| MAUI 28G LOUNGE (LD Systems) | 2 | Cavo XLR da Mixer AUX2 | Confermato |
| Speaker SSSNAKE Galleria | 1 | Cavo XLR da Mixer AUX1 | Confermato |
| Casse Sonos (opzionali) | 8 | ~1KW totale | **DA CONFERMARE** |

#### Cablaggio Audio
| Materiale | Quantita' | Tratta | Stato |
|-----------|-----------|--------|-------|
| Cavo XLR | 2 | Mixer Behringer (AUX2) -> MAUI 28G | ~15m - **DA QUANTIFICARE** |
| Cavo XLR | 1 | Mixer Behringer (AUX1) -> Speaker SSSNAKE | ~15m - **DA QUANTIFICARE** |

#### Alimentazione
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Prese 16A | 3 | Minimo 2 (~4.3kW LED + audio) | **DA CONFERMARE posizione** |
| Quadro 32A | 1 | Alternativa | - |

#### Vano Tecnico (per PC Sending + MCTRL4K)
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Vano ispezionabile/mensola | 1 | Per PC sending + controller 2U | **DA DEFINIRE con Henoto** |
| Ripiano bancone bar | 1 | Alternativa | **DA CONFERMARE** |

*Il controller MCTRL4K e' formato 2U rack. Necessita alimentazione e ventilazione*

#### ⚠️ MATERIALI MANCANTI/DA VERIFICARE - LOUNGE
- [ ] Conferma arrivo moduli 45° (SX e DX)
- [ ] Vano/mensola per tecnica (decisione con Greta)
- [ ] 24 cavi LAN Cat.5 ~15m (12 main + 12 backup)
- [ ] 3x Cavi XLR ~15m per MAUI e Speaker (da mixer AUX1/AUX2)
- [ ] Cavo HDMI corto PC Sending->MCTRL4K
- [ ] Staffaggio per montaggio su parete
- [ ] Tipo casse definitivo (Sonos vs altro)

---

### 9.4 RISTORANTE PIANO -1 (LED01 - Ex Esselunga)

#### LED Wall (2304x960px)
| Materiale | Quantita' | Flight Case | Stato |
|-----------|-----------|-------------|-------|
| LED SEGNA 2.6 (500x1000mm) | 24 | CORT01-CORT05 | **NOLEGGIO SEDICO** |
| LED SEGNA 2.6 (500x500mm) | 12 | CORT01-CORT05 | **NOLEGGIO SEDICO** |

*LED a noleggio da Sedico - verificare disponibilita' e date consegna*

#### Segnale Video (da Regia - **PERCORSO CRITICO**)
| Materiale | Quantita' | Tratta | Stato |
|-----------|-----------|--------|-------|
| Cavi LAN Cat.5 Main | 5 | MCTRL4K (Regia P.0) -> Moduli LED (P.-1) | ~30m - **PERCORSO DA DEFINIRE** |
| Cavi LAN Cat.5 Backup | 5 | MCTRL4K (Regia P.0) -> Moduli LED (P.-1) | ~30m - **PERCORSO DA DEFINIRE** |
| Extender HDMI/LAN | 1 set | Trasmitter (Regia) + Receiver (Rist.) | **CONSIGLIATO per distanza** |
| Fibra ottica HDMI | 1 | Alternativa per qualita' segnale | **DA VALUTARE** |

*⚠️ CRITICITA': Porta vetro tra piani potrebbe essere murata. Verificare passaggio via cappa/aerazione cucina*

#### Controller e Sending
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| MCTRL4K | 1 | In regia P.0 - riceve HDMI da VMIX2 | Confermato |
| VX1000 (Sending) | 1 | Backup/alternativa | Confermato |
| Scheda Audio USB | 1 | Collegata a VMIX2 | Confermato |

#### Audio
| Materiale | Quantita' | Collegamento | Stato |
|-----------|-----------|--------------|-------|
| MAUI 28G (LD Systems) | 2 | Cavo XLR da Mixer o locale | Confermato |
| Casse incasso (opzionali) | 2 | Se parete 7x2.5m | **DA DECIDERE** |

#### Cablaggio Audio
| Materiale | Quantita' | Tratta | Stato |
|-----------|-----------|--------|-------|
| Cavo XLR | 2 | Per MAUI 28G (locale o da regia) | ~30m - **DA QUANTIFICARE** |

*Se audio gestito localmente, servono cavi XLR corti. Se da regia, ~30m per piano*

#### Alimentazione
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Quadro 32A pentapolare | 1 | Oppure 5x16A (~11kW LED + audio) | **DA CONFERMARE posizione** |

#### Montaggio
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Truss | - | Oppure staffe a C | **DA DEFINIRE** |
| Staffe a C | - | Spessore 25-30cm dietro LED | **DA DEFINIRE** |
| Parete dedicata 7x2.5m | 1 | Opzione con casse incassate ai lati | **DA DECIDERE** |
| Pannello ispezionabile | 1 | Lato cucina o corridoio camerieri | **DA DEFINIRE** |

#### ⚠️ MATERIALI MANCANTI/DA VERIFICARE - RISTORANTE
- [ ] **CRITICO**: Percorso cavi regia P.0 -> ristorante P.-1 (porta vetro murata?)
- [ ] Soluzione passaggio: cappa/aerazione cucina o finestra
- [ ] Conferma noleggio LED Sedico (date e condizioni)
- [ ] 10 cavi LAN Cat.5 ~30m (5 main + 5 backup)
- [ ] Extender HDMI/LAN consigliato per distanza
- [ ] Decisione truss vs staffe a C
- [ ] Decisione parete dedicata 7x2.5m per casse incasso
- [ ] Posizione pannello ispezionabile
- [ ] 2x Cavi XLR per MAUI (lunghezza da definire)

---

### 9.5 LED ESTERNO PIAZZALE (LED06)

#### LED Wall (768x512px)
| Materiale | Quantita' | Flight Case | Stato |
|-----------|-----------|-------------|-------|
| AMIL BLUE 3.9 outdoor (500x1000mm) | 12 | CORT14, CORT15, CORT16 | Bollino fucsia - testare 3 case |
| Spare modules | - | CORT16 | Confermato |

*LED outdoor sostituzione BLADE - verificare 3 case con bollino fucsia prima dell'installazione*

#### Segnale Video (da Regia)
| Materiale | Quantita' | Tratta | Stato |
|-----------|-----------|--------|-------|
| Cavi LAN Cat.5 Main | 1 | MTCRL300 (case esterno) -> Moduli LED | ~5m locale |
| Cavi LAN Cat.5 Backup | 1 | MTCRL300 (case esterno) -> Moduli LED | ~5m locale |
| Cavo LAN segnale regia | 1 | Regia -> Case esterno | ~25m - **DA QUANTIFICARE** |
| Cavo HDMI (o extender) | 1 | Per segnale video al MTCRL300 | **DA VERIFICARE** |

*Il controller MTCRL300 e' posizionato in case leggero vicino al LED, riceve segnale dalla regia*

#### Controller e Sending (in case locale)
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| MTCRL300 (Sending 300) | 1 | In case leggero outdoor | Confermato |
| EDV | 1 | Collegamento a MTCRL300 | Confermato |
| Scheda Audio | 1 | Per audio locale | Confermato |
| Presa 220V | 1 | In case | Confermato |

#### Audio (Speaker Passivi + Amplificatore)
| Materiale | Quantita' | Collegamento | Stato |
|-----------|-----------|--------------|-------|
| Fonestar (speaker passivi a parete) | 2 | Cavo speaker da Amplificatore | Confermato |
| Amplificatore Monacor | 1 | Alimenta Fonestar, ingresso audio da scheda | Confermato |

*I Fonestar sono speaker passivi, necessitano amplificatore Monacor per funzionare*

#### Cablaggio Audio
| Materiale | Quantita' | Tratta | Stato |
|-----------|-----------|--------|-------|
| Cavo speaker | 2 | Amplificatore Monacor -> Fonestar | ~5m - **DA QUANTIFICARE** |
| Cavo audio (jack/XLR) | 1 | Scheda Audio -> Amplificatore | ~1m locale |

#### Struttura Montaggio
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Pali 2m | 4 | Tubolari 2" | Da preparare |
| Pali 3m | 3 | Tubolari 2" | Da preparare |
| Pali 1m | 6 | Tubolari 2" | Da preparare |
| Aliscaf singoli | 10 | Connessioni tubolari | Da preparare |
| Aliscaf doppi | 16 | Connessioni tubolari | Da preparare |
| Truss/Layher | - | Struttura condivisa con Pascucci (luci) | **DA COORDINARE** |
| Canaline carrabili | 10 | CORT17 - protezione cavi a terra | Confermato |

#### Alimentazione
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Prese 16A | 2 | ~4kW totale | Confermato |
| Partenze corrente | 2 | - | Confermato |

#### ⚠️ MATERIALI MANCANTI/DA VERIFICARE - ESTERNO
- [ ] Test 3 case AMIL BLUE (bollino fucsia) prima di partire
- [ ] Coordinamento struttura con Pascucci (luci outdoor)
- [ ] Cavo segnale regia->case esterno (~25m)
- [ ] Extender HDMI/LAN se necessario per distanza
- [ ] Protezione meteo per case tecnico (pioggia/neve)
- [ ] Cavi speaker per Fonestar (~5m x2)
- [ ] **MANCA NEL CRONOPROGRAMMA HENOTO** - da aggiungere
- [ ] Rischio neve - schedulare weather-dependent, priorita' alta

---

### 9.6 SALA STAMPA / CASA GIORNALISTI (Piano -1)

#### Monitor
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Monitor TV 55" | 2 | LED05 | Confermato |
| Stand da tavolo | 2 | - | Confermato |

#### Contenuti
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Segnale RAI Sport | 1 | Fisso | Da verificare antenna |
| Segnale RAI 2 | 1 | Fisso | Da verificare antenna |

#### Connettivita'
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Presa Internet | 1 | - | **DA VERIFICARE** |
| Presa Antenna TV | 1 | SAT/TV trovata in camera | **DA VERIFICARE** |

#### ⚠️ MATERIALI MANCANTI/DA VERIFICARE - SALA STAMPA
- [ ] Verifica presa internet nella stanza
- [ ] Verifica antenna TV (SAT/TV)
- [ ] Cavi HDMI per monitor
- [ ] Decoder/ricevitore TV se necessario
- [ ] Ciabatte/alimentazione

---

### 9.7 SPAZIO INTERVISTE (Piano 0 - C.PT.14)

#### Monitor
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Monitor TV 55" | 2 | LED05 - Area interviste | Confermato |
| Stand da terra | 2 | - | Confermato |

#### ⚠️ MATERIALI MANCANTI/DA VERIFICARE - INTERVISTE
- [ ] Alimentazione monitor
- [ ] Segnale video (da regia o autonomo?)
- [ ] Cavi HDMI
- [ ] Eventuale audio per monitor

---

### 9.8 RIEPILOGO FLIGHT CASE CORTINA

| Codice | Contenuto | Destinazione |
|--------|-----------|--------------|
| CORT01 | LED noleggio Sedico | Ristorante -1 |
| CORT02 | LED noleggio Sedico | Ristorante -1 |
| CORT03 | LED noleggio Sedico | Ristorante -1 |
| CORT04 | LED noleggio Sedico | Ristorante -1 |
| CORT05 | LED noleggio Sedico | Ristorante -1 |
| CORT11 | Coppia casse MAUI | Celebration |
| CORT12 | VMIX1, VMIX2, Microfoni JTS, MiniPC, Encoder | Regia |
| CORT14 | AMIL BLUE fucsia | LED Esterno |
| CORT15 | AMIL BLUE fucsia | LED Esterno |
| CORT16 | AMIL BLUE fucsia (spare) | LED Esterno |
| CORT17 | Canaline carrabili (10 pz) | LED Esterno |
| Bancale COB1.5 | 80 moduli dritti/sx/dx | Celebration + Lounge |

---

### 9.9 CABLAGGIO GENERALE - DA QUANTIFICARE

| Tratta | Tipo Cavo | Lunghezza Stimata | Stato |
|--------|-----------|-------------------|-------|
| Regia -> Celebration | Treccia Nitto 12/14 cavi | 20m | Confermato |
| Regia -> Celebration | Cavi LAN | ~20m x 10 | **DA QUANTIFICARE** |
| Regia -> Lounge | Cavi LAN | ~15m x 18 | **DA QUANTIFICARE** |
| Regia -> Ristorante -1 | Cavi LAN | ~30m x 10 | **CRITICO - percorso da definire** |
| Regia -> LED Esterno | Cavi LAN | ~25m x 2 | **DA QUANTIFICARE** |
| Regia -> Telecamere PTZ | Cavi BNC | ~20m x 2 | **DA QUANTIFICARE** |
| Sotto moquette | Cavi vari | - | **PRIMA del 2 febbraio** |

#### Materiali Cablaggio Generici
| Materiale | Quantita' | Note | Stato |
|-----------|-----------|------|-------|
| Rulli cavo di rete Cat6 | - | - | **DA QUANTIFICARE** |
| Cavi BNC | - | Per telecamere | **DA QUANTIFICARE** |
| Fibre ottiche | - | Se necessarie | **DA VERIFICARE** |
| Prolunghe elettriche | - | Per ogni area | **DA QUANTIFICARE** |
| Canaline/passacavi | - | Per percorsi | **DA QUANTIFICARE** |
| Fascette/velcro | - | Per fissaggio | **DA QUANTIFICARE** |
| Nastro Nitto | - | Per trecce | Confermato |

---

### ⚠️ 9.10 RIEPILOGO CRITICITA' MATERIALI

#### URGENTE - Da risolvere immediatamente
1. **Percorso cavi Regia -> Piano -1**: Porta vetro potrebbe essere murata
2. **Moduli COB 45°**: In arrivo settimana prossima - verificare consegna
3. **LED Sedico noleggio**: Confermare disponibilita' e date
4. **Test AMIL BLUE**: Verificare 3 case con bollino fucsia

#### DA DEFINIRE con Henoto/Greta
1. Posizionamento quadri elettrici (16A vs 32A)
2. Vano tecnico per LED Lounge
3. Tipo casse (incasso vs self-standing)
4. Struttura LED esterno (coordinamento Pascucci)
5. Passaggi cavi sotto moquette (prima del 2 febbraio)

#### DA QUANTIFICARE
1. Lunghezze esatte tutti i cavi
2. Numero cavi BNC per PTZ
3. Cavi audio per tutte le tratte
4. Prolunghe elettriche per ogni area
5. Materiale di consumo (fascette, velcro, nastro)

---

## 10. CRONOPROGRAMMA INSTALLAZIONE INFORMA SISTEMI

### 10.1 Premesse e Vincoli

**Data inaugurazione Casa Italia:** 6 Febbraio 2026
**Deadline installazioni complete:** 5 Febbraio 2026 (collaudo finale)
**Vincolo moquette:** Passaggio cavi PRIMA della posa (prevista 2 Febbraio)
**Ingresso cantiere richiesto:** 25-26 Gennaio 2026

**Team Informa Sistemi - 5 persone totali:**

| Ruolo | Nome | Competenze |
|-------|------|------------|
| **PM Cortina + Tecnico Regia** | Maximilian Giurastante | Project Management, VMIX, Regia live |
| **Tecnico Regia** | Flavia Falanga | VMIX, Audio, Coordination |
| **Installatore Principale** | Igor Matiuzzi | LED, Cablaggio, Sistemi |
| **Installatore Supporto 1** | *Da definire* | LED, Cablaggio |
| **Installatore Supporto 2** | *Da definire* | LED, Cablaggio |

**Composizione squadre:**
- **Squadra LED (3 persone):** Igor Matiuzzi (capo), + 2 installatori supporto
- **Squadra Regia (2 persone):** Maximilian Giurastante, Flavia Falanga

**Tempistiche base per LED:**
- LED semplice (montaggio parete): ~2 giorni
- LED complesso (struttura/angoli): ~2.5 giorni
- Cablaggio per tratta: ~0.5 giorni

---

### 10.2 Cronoprogramma Dettagliato

#### FASE 0: PRE-CANTIERE (20-24 Gennaio)
| Data | Attivita' | Responsabile | Note |
|------|-----------|--------------|------|
| 20-21 Gen | Test 3 case AMIL BLUE (bollino fucsia) | Magazzino IS | Prima di caricare |
| 20-21 Gen | Premontaggio colonne LED Celebration (10x4 + 10x3) | Magazzino IS | 70 moduli totali |
| 20-21 Gen | Premontaggio colonne LED Lounge (12x4 dritti + 4x4 SX + 4x4 DX) | Magazzino IS | Attesa moduli 45° |
| 22 Gen | Verifica arrivo moduli COB 45° | Acquisti IS | **CRITICO** |
| 22-23 Gen | Preparazione flight case CORT01-17 | Magazzino IS | Lista completa |
| 23 Gen | Carico mezzi (furgone + bilico LED) | Logistica IS | Partenza h.18:00 |
| 24 Gen | Viaggio + Arrivo Cortina | Logistica IS | ~6h viaggio |

---

#### FASE 1: CABLAGGIO PRINCIPALE (25-27 Gennaio)
*Priorita' MASSIMA: Cavi sotto moquette prima della posa*

| Data | Giorno | Attivita' | Team | Ore | Note |
|------|--------|-----------|------|-----|------|
| **25 Gen** | Sab | Scarico materiali + Sopralluogo percorsi cavi | 2 tecnici | 8h | Verifica percorso P.0->P.-1 |
| **25 Gen** | Sab | Posa treccia Nitto 20m (Regia->Celebration) | 2 tecnici | 4h | Sotto battiscopa |
| **26 Gen** | Dom | Cablaggio LAN Regia->Lounge (~15m x 24 cavi) | 2 tecnici | 8h | Main + Backup |
| **26 Gen** | Dom | Cablaggio LAN Regia->Celebration (~20m x 20 cavi) | 2 tecnici | 6h | Via treccia Nitto |
| **27 Gen** | Lun | Cablaggio LAN Regia->Ristorante P.-1 (~30m x 10 cavi) | 2 tecnici | 8h | **PERCORSO CRITICO** |
| **27 Gen** | Lun | Cablaggio audio XLR (tutte le tratte) | 1 tecnico | 6h | Mixer->MAUI/Speaker |
| **27 Gen** | Lun | Cablaggio BNC telecamere PTZ | 1 tecnico | 4h | 3x PTZ->Regia |

**⚠️ CHECKPOINT 27 Gen sera:** Tutti i cavi sotto moquette devono essere posati

---

#### FASE 2: LED CELEBRATION (28-29 Gennaio)
*LED03 - Tensostruttura Padiglione - 6x2.36m*

| Data | Giorno | Attivita' | Team | Ore | Note |
|------|--------|-----------|------|-----|------|
| **28 Gen** | Mar | Montaggio struttura/supporti parete legno | 3 installatori | 4h | Viti + zoccolo 15cm |
| **28 Gen** | Mar | Installazione colonne LED (10 col x 7 moduli) | 3 installatori | 8h | 70 moduli |
| **29 Gen** | Mer | Collegamento cavi LAN (10 main + 10 backup) | 3 installatori | 4h | Da treccia Nitto |
| **29 Gen** | Mer | Collegamento alimentazione + Tail A | 3 installatori | 3h | Quadro 32A |
| **29 Gen** | Mer | Test e calibrazione MCTRL4K | 1 tecnico regia | 3h | Con VMIX1 |
| **29 Gen** | Mer | Installazione audio MAUI 28G (2x) | 2 installatori | 2h | XLR da Mixer LR |

**Durata totale LED Celebration:** 2 giorni

---

#### FASE 3: LED LOUNGE (30-31 Gennaio + 1 Feb mattina)
*LED02+LED04 - Configurazione a C - Piano Galleria*

| Data | Giorno | Attivita' | Team | Ore | Note |
|------|--------|-----------|------|-----|------|
| **30 Gen** | Gio | Preparazione vano tecnico (mensola/ripiano) | 2 installatori | 3h | Accordo con Henoto |
| **30 Gen** | Gio | Montaggio supporti parete (configurazione C) | 3 installatori | 5h | Struttura angolare |
| **30 Gen** | Gio | Installazione colonne dritte (12 col x 4 moduli) | 3 installatori | 6h | 48 moduli |
| **31 Gen** | Ven | Installazione colonne angolari SX (4 col x 4 moduli) | 3 installatori | 4h | 16 moduli 45° |
| **31 Gen** | Ven | Installazione colonne angolari DX (4 col x 4 moduli) | 3 installatori | 4h | 16 moduli 45° |
| **31 Gen** | Ven | Collegamento cavi LAN (12 main + 12 backup) | 3 installatori | 3h | Totale 24 cavi |
| **1 Feb** | Sab | Collegamento alimentazione + Tail A | 2 installatori | 2h | 3x16A |
| **1 Feb** | Sab | Posizionamento PC Sending + MCTRL4K in vano | 1 tecnico regia | 2h | Controller 2U |
| **1 Feb** | Sab | Test e calibrazione MCTRL4K | 1 tecnico regia | 3h | Con VMIX3 |
| **1 Feb** | Sab | Installazione audio MAUI + Speaker | 2 installatori | 3h | XLR da Mixer AUX1/2 |

**Durata totale LED Lounge:** 2.5 giorni (complessita' angoli 45°)

---

#### FASE 4: LED RISTORANTE P.-1 (1-2 Febbraio)
*LED01 SEGNA - Ex Esselunga - 6x2.5m - Noleggio Sedico*

| Data | Giorno | Attivita' | Team | Ore | Note |
|------|--------|-----------|------|-----|------|
| **1 Feb** | Sab | Montaggio truss/staffe a C | 3 installatori | 5h | Spessore 25-30cm |
| **1 Feb** | Sab | Ritiro LED noleggio Sedico | 1 autista | 4h | CORT01-05 |
| **2 Feb** | Dom | Installazione moduli LED SEGNA | 3 installatori | 8h | 500x1000 + 500x500 |
| **2 Feb** | Dom | Collegamento cavi LAN (5 main + 5 backup) | 2 installatori | 3h | Percorso da P.0 |
| **2 Feb** | Dom | Collegamento alimentazione | 2 installatori | 2h | Quadro 32A |
| **2 Feb** | Dom | Test e calibrazione MCTRL4K | 1 tecnico regia | 3h | Con VMIX2 |
| **2 Feb** | Dom | Installazione audio MAUI (2x) | 2 installatori | 2h | - |

**Durata totale LED Ristorante:** 2 giorni

**⚠️ ATTENZIONE:** Posa moquette prevista 2 Febbraio - coordinare con Henoto

---

#### FASE 5: REGIA VIDEO (1-3 Febbraio)
*Parallelo alle installazioni LED - Piano 0 Spazio C.PT.17*

| Data | Giorno | Attivita' | Team | Ore | Note |
|------|--------|-----------|------|-----|------|
| **1 Feb** | Sab | Posizionamento rack/tavoli regia | 2 tecnici | 3h | Mensole + prese 220V |
| **1 Feb** | Sab | Installazione Switch 24 porte | 1 tecnico | 2h | Hub centrale |
| **1 Feb** | Sab | Setup PC VMIX 1, 2, 3 | 2 tecnici | 4h | Monitor 27" |
| **2 Feb** | Dom | Setup MiniPC WIN1-4 + Encoder Kiloview | 2 tecnici | 4h | Streaming gare |
| **2 Feb** | Dom | Collegamento Sending Cards MCTRL4K (3x) + MTCRL300 | 2 tecnici | 3h | HDMI da VMIX |
| **2 Feb** | Dom | Setup Mixer Behringer + Schede Audio USB | 1 tecnico | 3h | LR/AUX1/AUX2 |
| **3 Feb** | Lun | Installazione telecamere PTZ (3x) | 2 tecnici | 4h | BNC->Schede acquisizione |
| **3 Feb** | Lun | Configurazione rete intranet | 1 tecnico | 4h | Switch + routing |
| **3 Feb** | Lun | Test collegamenti inter-house | 2 tecnici | 4h | Milano/Livigno |

**Durata totale Regia:** 3 giorni (in parallelo)

---

#### FASE 6: LED ESTERNO (3-4 Febbraio)
*LED06 AMIL BLUE - Piazzale - 3x2m - Weather dependent*

| Data | Giorno | Attivita' | Team | Ore | Note |
|------|--------|-----------|------|-----|------|
| **3 Feb** | Lun | Montaggio struttura pali + aliscaf | 3 installatori | 6h | Coord. Pascucci luci |
| **3 Feb** | Lun | Posizionamento case MTCRL300 | 1 tecnico | 2h | Case leggero outdoor |
| **4 Feb** | Mar | Installazione moduli AMIL BLUE | 3 installatori | 6h | 12 moduli outdoor |
| **4 Feb** | Mar | Cablaggio LAN esterno (1 main + 1 backup) | 2 installatori | 2h | Con canaline carrabili |
| **4 Feb** | Mar | Collegamento audio Fonestar + Monacor | 1 tecnico | 2h | Speaker passivi |
| **4 Feb** | Mar | Test e calibrazione MTCRL300 | 1 tecnico regia | 2h | - |

**Durata totale LED Esterno:** 2 giorni

**⚠️ RISCHIO METEO:** Prevedere giorno buffer in caso neve/maltempo

---

#### FASE 7: MONITOR E FINITURE (4 Febbraio)
*Sala Stampa + Spazio Interviste*

| Data | Giorno | Attivita' | Team | Ore | Note |
|------|--------|-----------|------|-----|------|
| **4 Feb** | Mar | Installazione Monitor 55" Sala Stampa (2x) | 2 installatori | 2h | Stand tavolo |
| **4 Feb** | Mar | Collegamento segnale RAI Sport/RAI 2 | 1 tecnico | 2h | Verifica antenna |
| **4 Feb** | Mar | Installazione Monitor 55" Interviste (2x) | 2 installatori | 2h | Stand terra |
| **4 Feb** | Mar | Finiture cablaggio (fascette, canaline) | 2 tecnici | 4h | Ordine generale |

---

#### FASE 8: COLLAUDO FINALE (5 Febbraio)
*Test completo di tutti i sistemi*

| Data | Giorno | Attivita' | Team | Ore | Note |
|------|--------|-----------|------|-----|------|
| **5 Feb** | Mer | Test tutti i LED (contenuti, colori, luminosita') | 2 tecnici | 4h | Tutti i VMIX |
| **5 Feb** | Mer | Test audio tutte le zone | 1 tecnico | 3h | Livelli, routing |
| **5 Feb** | Mer | Test streaming gare (MiniPC + Encoder) | 1 tecnico | 2h | Discovery/RAI |
| **5 Feb** | Mer | Test collegamenti PTZ inter-house | 2 tecnici | 3h | Milano/Livigno |
| **5 Feb** | Mer | Test generale con cliente | Team completo | 2h | Demo funzionalita' |
| **5 Feb** | Mer | Correzioni/regolazioni finali | Team completo | 2h | Buffer |

---

### 10.3 Riepilogo Grafico (Gantt Semplificato)

```
GENNAIO 2026                           FEBBRAIO 2026
20  21  22  23  24  25  26  27  28  29  30  31  01  02  03  04  05  06
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
[PRE-CANTIERE (test+premontaggio)]
                    [VIAGGIO]
                        [====CABLAGGIO PRINCIPALE====]
                                    [CELEBRATION]
                                                [===LOUNGE===]
                                                    [RISTORANTE]
                                                [======REGIA======]
                                                            [ESTERNO]
                                                                [MON]
                                                                    [OK]
                                                                        *INAUG*

Legenda:
[====] = Attivita' in corso
*INAUG* = Inaugurazione 6 Febbraio
```

---

### 10.4 Risorse per Giorno

**Legenda Team:**
- **Igor** = Igor Matiuzzi (Installatore Principale)
- **Supp1/Supp2** = Installatori Supporto (nomi da definire)
- **Max** = Maximilian Giurastante (PM + Tecnico Regia)
- **Flavia** = Flavia Falanga (Tecnico Regia)

| Data | Squadra LED (Igor + Supporto) | Squadra Regia (Max + Flavia) | Totale | Note |
|------|------------------------------|------------------------------|--------|------|
| 25 Gen | - | Max, Flavia | 2 | Scarico + Sopralluogo cavi |
| 26 Gen | - | Max, Flavia | 2 | Cablaggio LAN principale |
| 27 Gen | - | Max, Flavia | 2 | Cablaggio P.-1 + Audio |
| 28 Gen | Igor, Supp1, Supp2 | Max | 4 | LED Celebration D1 |
| 29 Gen | Igor, Supp1, Supp2 | Max | 4 | LED Celebration D2 |
| 30 Gen | Igor, Supp1, Supp2 | Flavia | 4 | LED Lounge D1 |
| 31 Gen | Igor, Supp1, Supp2 | Flavia | 4 | LED Lounge D2 + Ristorante |
| 1 Feb | Igor, Supp1, Supp2 | Max, Flavia | 5 | Ristorante + Regia |
| 2 Feb | Igor, Supp1, Supp2 | Max, Flavia | 5 | Regia setup completo |
| 3 Feb | Igor, Supp1, Supp2 | Max, Flavia | 5 | LED Esterno D1 |
| 4 Feb | Igor, Supp1, Supp2 | Max, Flavia | 5 | LED Esterno D2 + Monitor |
| 5 Feb | Igor, Supp1 | Max, Flavia | 4 | Collaudo generale |

**Totale giornate uomo:** ~50 gg/uomo (5 persone x 10 giorni medi)

---

### 10.5 CONFRONTO CRONOPROGRAMMI: HENOTO vs INFORMA SISTEMI

#### Cronoprogramma HENOTO (Attuale)
```
GENNAIO 2026                           FEBBRAIO 2026
15  16  17  18  19  20  21  22  23  24  25  26  27  28  29  30  31  01  02  03  04  05  06
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
[===STRUTTURE HENOTO (15-16 Gen)===]
                        [====MONTAGGI GENERALI (22-23 Gen)====]
                                                        [INGRESSO IS (29 Gen)]------>
                                                                            [MOQUETTE]
                                                                                        [INAUG]
```

**Problemi del cronoprogramma Henoto:**
- Ingresso IS previsto: **29 Gennaio** (troppo tardi!)
- Posa moquette: **2 Febbraio** (i cavi devono passare PRIMA)
- Non include: LED Esterno, dettaglio fasi installazione LED, regia, cablaggio
- Gap di 4 giorni tra fine montaggi (23 Gen) e ingresso IS (29 Gen) - tempo perso!

---

#### Cronoprogramma INFORMA SISTEMI (Richiesto)
```
GENNAIO 2026                           FEBBRAIO 2026
15  16  17  18  19  20  21  22  23  24  25  26  27  28  29  30  31  01  02  03  04  05  06
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
[===STRUTTURE HENOTO===]
                    [PRE-CANTIERE IS (test, premontaggio)]
                                    [VIAG]
                                        [==CABLAGGIO (25-27)==]
                                                    [CELEBRATION]
                                                                [===LOUNGE===]
                                                                    [RISTORANTE]
                                                                [======REGIA======]
                                                                            [ESTERNO]
                                                                                [MON][OK]
                                                                                        [INAUG]
```

**Vantaggi del cronoprogramma IS:**
- Ingresso IS anticipato: **25-26 Gennaio** (+4 giorni di lavoro!)
- Cablaggio completato PRIMA della moquette (27 Gen sera)
- LED Esterno schedulato (weather-dependent con buffer)
- Regia in parallelo ai LED (ottimizzazione risorse)
- 1 giorno buffer per collaudo finale

---

#### TABELLA CONFRONTO DETTAGLIATO

| Attivita' | HENOTO (Attuale) | INFORMA SISTEMI (Richiesto) | Delta | Impatto |
|-----------|------------------|-----------------------------| ------|---------|
| **Ingresso cantiere IS** | 29 Gennaio | 25-26 Gennaio | **-4 giorni** | CRITICO - necessario per completare |
| **Inizio cablaggio** | Non previsto | 25 Gennaio | - | Deve essere PRIMA moquette |
| **Fine cablaggio sotto moquette** | Non previsto | 27 Gennaio sera | - | OBBLIGATORIO prima 2 Feb |
| **LED Celebration** | Non dettagliato | 28-29 Gennaio | - | 2 giorni con 3 installatori |
| **LED Lounge** | Non dettagliato | 30 Gen - 1 Feb | - | 2.5 giorni (angoli 45°) |
| **LED Ristorante** | Non dettagliato | 1-2 Febbraio | - | 2 giorni + noleggio Sedico |
| **Regia Video** | Non prevista | 1-3 Febbraio | - | In parallelo ai LED |
| **LED Esterno** | **NON PREVISTO** | 3-4 Febbraio | - | MANCA nel crono Henoto! |
| **Posa moquette** | 2 Febbraio | 2 Febbraio | = | Vincolo fisso |
| **Collaudo finale** | Non previsto | 5 Febbraio | - | 1 giorno buffer |
| **Inaugurazione** | 6 Febbraio | 6 Febbraio | = | Deadline fissa |

---

#### GRAFICO COMPARATIVO VISIVO

```
                    HENOTO                          vs                    INFORMA SISTEMI

        |------ 29 Gen ------|                              |------ 25 Gen ------|
        |    INGRESSO IS     |                              |    INGRESSO IS     |
        |____________________|                              |____________________|
                 |                                                   |
                 v                                                   v
        Solo 8 GIORNI                                        12 GIORNI COMPLETI
        per completare tutto!                                per lavorare con calma
                 |                                                   |
                 v                                                   v
        ❌ Cavi dopo moquette?                               ✅ Cavi PRIMA moquette
        ❌ LED Esterno non schedulato                        ✅ LED Esterno con buffer meteo
        ❌ Nessun buffer collaudo                            ✅ 1 giorno collaudo finale
        ❌ Rischio ritardi                                   ✅ Margine di sicurezza
```

---

#### ⚠️ RICHIESTA FORMALE A HENOTO

**Data richiesta:** Anticipare ingresso Informa Sistemi dal **29 Gennaio** al **25-26 Gennaio**

**Motivazioni tecniche:**
1. **Cablaggio sotto moquette**: I cavi LAN, XLR e BNC devono essere posati PRIMA del 2 Febbraio
2. **4 LED Wall da installare**: Servono almeno 8-10 giorni lavorativi, non 8
3. **LED Esterno mancante**: Non e' nel cronoprogramma Henoto ma e' previsto da contratto
4. **Regia complessa**: 3 PC VMIX, 4 MiniPC, 4 Encoder, 3 PTZ richiedono tempo
5. **Test inter-house**: Collegamento con Milano/Livigno richiede giornata dedicata

**Conseguenze se non anticipato:**
- Rischio di non completare entro il 6 Febbraio
- Cavi a vista sopra moquette (impresentabile)
- LED Esterno non installato
- Nessun tempo per collaudo e correzioni

---

### 10.6 Criticita' Cronoprogramma

#### ⚠️ PUNTI CRITICI

1. **Percorso cavi P.0 -> P.-1 (27 Gen)**
   - Porta vetro potrebbe essere murata
   - **Azione:** Verificare PRIMA del 25 Gen con Henoto
   - **Piano B:** Passaggio via cappa/aerazione cucina

2. **Arrivo moduli COB 45° (22 Gen)**
   - Necessari per LED Lounge
   - **Azione:** Confermare consegna entro 21 Gen
   - **Piano B:** Iniziare con moduli dritti, completare angoli dopo

3. **Posa moquette (2 Feb)**
   - Tutti i cavi sotto moquette devono essere posati PRIMA
   - **Azione:** Completare cablaggio principale entro 27 Gen sera
   - **Piano B:** Chiedere proroga posa moquette

4. **LED Esterno - Meteo**
   - Rischio neve/maltempo a Cortina
   - **Azione:** Monitorare meteo, prevedere giorno buffer
   - **Piano B:** Posticipare a 5 Feb mattina se necessario

5. **Noleggio LED Sedico**
   - Confermare disponibilita' e date ritiro
   - **Azione:** Confermare entro 20 Gen
   - **Piano B:** Nessuno - attivita' critica

---

### 10.6 Checklist Pre-Partenza (24 Gennaio)

- [ ] Test completato AMIL BLUE (3 case fucsia)
- [ ] Premontaggio completato colonne Celebration
- [ ] Premontaggio completato colonne Lounge (inclusi 45°)
- [ ] Conferma noleggio LED Sedico
- [ ] Flight case CORT01-17 preparati
- [ ] Percorso cavi P.0->P.-1 definito con Henoto
- [ ] Quadri elettrici confermati (posizione)
- [ ] Vano tecnico Lounge confermato
- [ ] Coordinamento Pascucci per struttura esterna
- [ ] Previsioni meteo verificate

---

## 11. ALLEGATI E RIFERIMENTI

### Documenti Disponibili
1. `Crono Casa Italia_Cortina.xlsx` - Cronoprogramma Henoto
2. `Dettaglio installazioni Cortina.xlsx` - Specifiche tecniche
3. `Cortina ABACO DISPOSITIVI.pdf` - Piante con legenda dispositivi
4. `Schema dettagliato regia cortina-drawio.pdf` - Schema regia v1.2
5. `Piantina Cortina piano 0.png` - Layout piano terra
6. `Piantina Cortina piano -1.png` - Layout piano interrato

### Link Utili
- Matterport location: [link nel file Excel Dettaglio installazioni]

---

**Documento redatto da:** Assistente PM
**Prossimo aggiornamento:** Post call con Henoto

---
*Versione 1.0 - 9 Gennaio 2026*
