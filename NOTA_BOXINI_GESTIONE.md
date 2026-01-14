# NOTA TECNICA - BOXINI DI GESTIONE
## Progetto Cortina 2026

**Data:** 14 Gennaio 2026
**Versione:** 1.2.11
**Oggetto:** Specifica funzionale dei 2 boxini di gestione

---

## BOXINI DI GESTIONE - DETTAGLIO FUNZIONALE

### RTR-02: Boxino Gestione Monitoraggio
**IP Statico:** 10.122.0.1
**Posizione:** Regia P.0

**Funzione Principale:**
Monitoraggio della rete locale e supervisione dello stato degli apparati.

**Compiti Specifici:**
- Monitoraggio real-time dello stato di tutti i dispositivi di rete
- Controllo del traffico di rete e delle performance
- Rilevamento anomalie e alert
- Dashboard di supervisione per la regia
- Logging centralizzato degli eventi di rete
- SNMP monitoring degli switch managed
- Verifica connettività dispositivi critici (LED, encoder, streaming)

**Dispositivi Monitorati:**
- 4x Switch Netgear GS110 (10.122.0.30-33)
- 4x Access Point WiFi (10.122.0.10-13)
- 4x Encoder Kiloview (10.122.0.50-53)
- 4x MiniPC Windows (10.122.0.60-63)
- Firewall/Router (10.122.0.254)

---

### RTR-03: Boxino Gestione Antenne
**IP Statico:** 10.122.0.2
**Posizione:** Regia P.0

**Funzione Principale:**
Gestione centralizzata delle antenne WiFi e ottimizzazione della copertura wireless.

**Compiti Specifici:**
- Gestione configurazione 4 Access Point WiFi
- Controllo canali WiFi per evitare interferenze
- Ottimizzazione potenza trasmissione
- Gestione SSID e credenziali
- Monitoraggio dispositivi connessi
- Roaming management tra AP
- Troubleshooting connessioni wireless
- Quality of Service (QoS) per traffico streaming

**Access Point Gestiti:**
- WIFI-01: 10.122.0.10 (LED03 Celebration)
- WIFI-02: 10.122.0.11 (LED02/04 Lounge)
- WIFI-03: 10.122.0.12 (LED01 Ristorante P.-1)
- WIFI-04: 10.122.0.13 (LED06 Esterno)

---

## ARCHITETTURA DI GESTIONE

```
┌─────────────────────────────────────────────────────┐
│              REGIA P.0 - SALA CONTROLLO             │
├─────────────────────────────────────────────────────┤
│                                                     │
│  ┌──────────────────┐      ┌──────────────────┐   │
│  │  RTR-02          │      │  RTR-03          │   │
│  │  Boxino Monitor  │      │  Boxino Antenne  │   │
│  │  10.122.0.1      │      │  10.122.0.2      │   │
│  └────────┬─────────┘      └────────┬─────────┘   │
│           │                         │             │
│           └──────────┬──────────────┘             │
│                      │                            │
│           ┌──────────┴──────────┐                 │
│           │  RTR-01             │                 │
│           │  Firewall/Router    │                 │
│           │  10.122.0.254       │                 │
│           │  (Gateway)          │                 │
│           └──────────┬──────────┘                 │
└──────────────────────┼─────────────────────────────┘
                       │
                       ▼
              RETE DISTRIBUZIONE
         (Switch, WiFi, Dispositivi)
```

---

## VANTAGGI DELL'ARCHITETTURA

### 1. Separazione dei Compiti
- **Monitoraggio** e **Gestione WiFi** sono funzioni indipendenti
- Fault tolerance: guasto di un boxino non impatta l'altro
- Performance: carichi distribuiti su 2 dispositivi dedicati

### 2. Gestione Centralizzata
- Punto unico di controllo per monitoraggio rete (RTR-02)
- Punto unico di controllo per WiFi (RTR-03)
- Interfacce dedicate per operatori in regia

### 3. Scalabilità
- Aggiunta futuri AP WiFi gestita da RTR-03
- Aggiunta futuri dispositivi monitorati da RTR-02
- Range IP riservati (.3-.9) per ulteriori boxini se necessario

### 4. Troubleshooting
- Diagnosi rapida problemi WiFi tramite RTR-03
- Analisi traffico e performance tramite RTR-02
- Isolamento problemi per dominio (rete vs wireless)

---

## CONFIGURAZIONE CONSIGLIATA

### RTR-02 (Monitoraggio)
```
IP: 10.122.0.1
Netmask: 255.255.255.0
Gateway: 10.122.0.254
DNS: Da configurare

Software Consigliato:
- Nagios/Zabbix per monitoring
- Grafana per dashboard visuali
- SNMP trap receiver
- Syslog server
```

### RTR-03 (Antenne)
```
IP: 10.122.0.2
Netmask: 255.255.255.0
Gateway: 10.122.0.254
DNS: Da configurare

Software Consigliato:
- Controller WiFi unificato
- Heatmap WiFi coverage
- Spectrum analyzer
- Client connection manager
```

---

## INTEGRAZIONE CON INFRASTRUTTURA

### Dipendenze
- **Firewall (RTR-01):** Gateway primario, entrambi i boxini passano per il firewall
- **Switch managed:** RTR-02 monitora via SNMP
- **Access Point:** RTR-03 configura e gestisce

### Comunicazione
- RTR-02 ↔ Tutti i dispositivi (polling monitoring)
- RTR-03 ↔ Access Point WiFi (configurazione)
- RTR-02 ↔ RTR-03 (scambio dati per correlazione eventi)

### Backup e Ridondanza
- Configurazioni salvate su RTR-01 (firewall)
- Failover automatico se disponibile
- Log remoti su storage NAS se disponibile

---

## MATERIALE DISPONIBILE

Secondo il foglio "materiale" del file Excel:
- ✅ **2 boxini gestione** disponibili in magazzino
- ✅ **2 firewall** disponibili (1 utilizzato come RTR-01)
- ✅ Configurazione completa possibile con materiale esistente

---

## CHECKLIST PRE-INSTALLAZIONE

- [ ] Verificare presenza fisica 2 boxini in magazzino
- [ ] Configurare IP statici (10.122.0.1 e 10.122.0.2)
- [ ] Installare software monitoring su RTR-02
- [ ] Installare controller WiFi su RTR-03
- [ ] Testare connettività con firewall RTR-01
- [ ] Configurare accesso SNMP agli switch
- [ ] Configurare accesso management agli AP WiFi
- [ ] Testare dashboard monitoring
- [ ] Documentare credenziali di accesso
- [ ] Backup configurazioni

---

**Documento generato per chiarire le funzioni specifiche dei boxini**
**Data:** 14 Gennaio 2026
**Versione:** 1.2.11
