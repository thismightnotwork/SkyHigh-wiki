# EGLC – London City Airport

!!! warning "SkyHigh Network Use Only"
    This page is for use on the SkyHigh simulation network only and must **never** be used for real-world operations.

## Aerodrome Overview

| Field | Value |
|-------|-------|
| **ICAO** | EGLC |
| **IATA** | LCY |
| **Full Name** | London City Airport |
| **Location** | Newham, Greater London |
| **ARP** | 513030N 0000344E |
| **Elevation** | 19 ft AMSL |
| **Transition Altitude** | 6,000 ft |
| **Division** | SkyHigh UK & Ireland |
| **FIR** | EGTT (London) |

---

## ATC Positions

### Aerodrome Control (ADC)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| ATIS | `EGLC_ATIS` | City Information | 136.350 MHz |
| Ground / Delivery | `EGLC_GND` | City Ground | 121.825 MHz |
| Tower (AIR) | `EGLC_TWR` | City Tower | 118.075 MHz |

### Approach Control (TC Thames)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| Director | `EGLC_APP` | City Director | 132.700 MHz |

!!! info "TC Thames Coverage"
    London City falls within the TC Thames sector. When TC Thames is offline, top-down coverage is provided by TC North East, or the relevant London TC bandbox controller.

---

## Radio Navigation & Landing Aids

| Type | Identifier | Frequency | Runway |
|------|-----------|-----------|--------|
| ILS/DME | I-LCY | 111.550 MHz | 09 |
| ILS/DME | I-LC | 111.550 MHz | 27 |

---

## Runways

| Designator | Length | Notes |
|-----------|--------|-------|
| **09 / 27** | 1,508 m | Single runway |

!!! warning "Steep Approach"
    London City uses a **5.5° glideslope** (vs the standard 3°) due to the obstacle environment in the Thames area. Only aircraft certified for steep approaches may operate into London City. Pilots must be briefed and aircraft must be STOL-capable or certified.

### Preferential Runway

Runway **27** is the preferred runway in westerly / calm conditions. **09** used in easterly winds.

---

## Altimetry

| Reference | Value |
|-----------|-------|
| Transition Altitude | 6,000 ft |
| ASR | Chatham |

---

## Standard Instrument Departures (SIDs)

| Route | RWY 09 | RWY 27 | Initial Climb |
|-------|--------|--------|---------------|
| **CLN** | CLN SIDs | CLN SIDs | 3,000 ft |
| **CPT** | — | CPT SIDs | 3,000 ft |
| **SILVA** | SILVA SIDs | — | 3,000 ft |
| **TIGER** | — | TIGER SIDs | 3,000 ft |

!!! note
    London City SIDs have low initial climb altitudes due to airspace constraints. All departures are coordinated with TC Thames before take-off.

---

## Arrivals

London City uses a continuous descent **steep approach** profile. TC Thames Directors vector aircraft onto the 5.5° glidepath. Due to the tight urban airspace, missed approach procedures are critical — all go-arounds require immediate coordination with TC Thames.

**Missed Approach (RWY 27):** Climb straight ahead to 1,000 ft, then turn left onto heading 180°, climb to 2,000 ft. Contact TC Thames Director.

**Missed Approach (RWY 09):** Climb straight ahead to 1,000 ft, then turn right onto heading 090°, climb to 2,000 ft. Contact TC Thames Director.

---

## Key References

- [UK AIP – EGLC AD2 (NATS eAIP)](https://www.aurora.nats.co.uk/htmlAIP/Publications/2025-08-07-AIRAC/html/eAIP/EG-AD-2.EGLC-en-GB.html)
- [CAP 493 – MATS Part 1](https://www.caa.co.uk/cap493)
