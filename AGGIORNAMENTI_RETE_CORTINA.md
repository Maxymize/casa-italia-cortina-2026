# AGGIORNAMENTI LISTA MATERIALI - APPARATI DI RETE
## Progetto Cortina 2026

**Data aggiornamento:** 14 Gennaio 2026
**Versione:** 1.2.10
**Fonte dati:** Lista Ip e apparati di rete - Cortina.xlsx

---

## MODIFICHE APPORTATE

### 1. Switch di Rete

**PRIMA:**
- Switch Manager generico (3-4 unità)
- Nessun IP assegnato
- Nessun modello specificato

**DOPO:**
- 4x Netgear GS110 (Switch managed 24 porte)
- IP Statici assegnati:
  - SW-01: 10.122.0.30 (LED03 Celebration)
  - SW-02: 10.122.0.31 (LED02/04 Lounge)
  - SW-03: 10.122.0.32 (LED01 Ristorante P.-1)
  - SW-04: 10.122.0.33 (LED06 Esterno)

---

### 2. Router e Firewall

**PRIMA:**
- 1x Router con Firewall integrato
- Nessun IP assegnato

**DOPO:**
- 3 unità con IP Statici:
  - RTR-01: 10.122.0.254 (Firewall/Router - Gateway principale)
  - RTR-02: 10.122.0.1 (Boxino Gestione Monitoraggio - Monitoraggio rete locale)
  - RTR-03: 10.122.0.2 (Boxino Gestione Antenne - Gestione antenne WiFi)

---

### 3. Access Point WiFi

**PRIMA:**
- 4x Access Point WiFi
- Nessun IP assegnato

**DOPO:**
- 4x Access Point WiFi con IP Statici:
  - WIFI-01: 10.122.0.10 (LED03 Celebration)
  - WIFI-02: 10.122.0.11 (LED02/04 Lounge)
  - WIFI-03: 10.122.0.12 (LED01 Ristorante P.-1)
  - WIFI-04: 10.122.0.13 (LED06 Esterno)
- Modalità: Cablata (NO mesh) per performance streaming ottimali

---

### 4. Nuova Sezione: Configurazione di Rete

**AGGIUNTO:**
- Subnet: 10.122.0.0/24
- Gateway: 10.122.0.254 (Firewall)
- DNS: Da configurare

**Range IP Statici Assegnati:**
- Router/Firewall: 10.122.0.1, 10.122.0.2, 10.122.0.254
- Access Point WiFi: 10.122.0.10-13
- Switch: 10.122.0.30-33
- Encoder Kiloview: 10.122.0.50-53
- MiniPC Streaming: 10.122.0.60-63

**Range DHCP:** 10.122.0.100-200 (per dispositivi temporanei)

---

## MATERIALI DI RETE DISPONIBILI

Secondo il foglio "materiale" del file Excel:
- ✓ 4 switch Netgear GS110 (CONFERMATI)
- ✓ 6 WiFi Access Point (4 utilizzati, 2 di riserva)
- ✓ 2 firewall (CONFERMATI)
- 5 switch unmanaged (NON utilizzati nel progetto principale)
- ✓ 2 boxini gestione (1 utilizzato come RTR-02)

---

## DISPOSITIVI CON IP ASSEGNATI (da Excel)

### Apparati di Rete Principali
1. **boxino gestione monitoraggio** - 10.122.0.1
2. **boxino gestione antenne** - 10.122.0.2
3. **firewall** - 10.122.0.254
4. **wifi celebration** - 10.122.0.10
5. **wifi lounge** - 10.122.0.11
6. **wifi ristorante** - 10.122.0.12
7. **wifi esterno** - 10.122.0.13
8. **switch celebration** - 10.122.0.30
9. **switch lounge** - 10.122.0.31
10. **switch ristorante** - 10.122.0.32
11. **switch esterno** - 10.122.0.33

### Encoder Video (già presenti nel documento)
12. **KILOVIEW1** - 10.122.0.50
13. **KILOVIEW2** - 10.122.0.51
14. **KILOVIEW3** - 10.122.0.52
15. **KILOVIEW4** - 10.122.0.53

### MiniPC Streaming (già presenti nel documento)
16. **windows stream 1** - 10.122.0.60
17. **windows stream 2** - 10.122.0.61
18. **windows stream 3** - 10.122.0.62
19. **windows stream 4** - 10.122.0.63

**TOTALE: 19 dispositivi con IP statico assegnato**

---

## FILE AGGIORNATI

1. ✓ **LISTA_MATERIALI_COMPLETA_CORTINA.md** - File markdown sorgente
2. ✓ **LISTA_MATERIALI_COMPLETA_CORTINA.docx** - Documento Word rigenerato
3. ✓ **Sezione 3. DISPOSITIVI DI RETE** - Completamente riscritta con:
   - Tabelle aggiornate con IP statici
   - Modelli specifici (Netgear GS110)
   - Nuova sottosezione 3.4 "Configurazione di Rete"
4. ✓ **Sezione 9.3 Dispositivi Rete** - Riepilogo aggiornato

---

## NOTE TECNICHE

- **IP esclusi:** Tutti gli IP con flag DHCP e quelli non assegnati a nessun apparato sono stati esclusi dall'analisi
- **Subnet utilizzata:** 10.122.0.0/24 (come da file Excel)
- **Gateway:** 10.122.0.254 è configurato come gateway di rete principale
- **WiFi:** Configurati in modalità cablata (NO mesh) per garantire performance ottimali per lo streaming
- **Switch:** Netgear GS110 managed a 24 porte, permettono gestione e monitoring della rete

---

## PROSSIMI PASSI

1. Verificare disponibilità fisica dei 4 switch Netgear GS110 in magazzino
2. Configurare gli IP statici su tutti i dispositivi prima del montaggio
3. Predisporre la configurazione del Firewall (RTR-01) con le regole di sicurezza
4. Testare la connettività tra tutti i dispositivi di rete
5. Configurare il range DHCP 10.122.0.100-200 per dispositivi temporanei

---

**Documento generato automaticamente dall'analisi del file Excel**
**File sorgente:** Lista Ip e apparati di rete - Cortina.xlsx
**Data:** 14 Gennaio 2026
