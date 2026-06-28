# EGKK – London Gatwick

!!! warning "SkyHigh Network Use Only"
    This page is for use on the SkyHigh simulation network only and must **never** be used for real-world operations.

## Aerodrome Overview

| Field | Value |
|-------|-------|
| **ICAO** | EGKK |
| **IATA** | LGW |
| **Full Name** | London Gatwick Airport |
| **Location** | Crawley, West Sussex |
| **ARP** | 510845N 0000938W |
| **Elevation** | 202 ft AMSL |
| **Transition Altitude** | 6,000 ft |
| **Division** | SkyHigh UK & Ireland |
| **FIR** | EGTT (London) |

---

## ATC Positions

### Aerodrome Control (ADC)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| ATIS | `EGKK_ATIS` | Gatwick Information | 136.525 MHz |
| Delivery (GMP) | `EGKK_DEL` | Gatwick Delivery | 121.955 MHz |
| Ground (GMC) | `EGKK_GND` | Gatwick Ground | 121.800 MHz |
| Tower (AIR) | `EGKK_TWR` | Gatwick Tower | 124.225 MHz |

### Approach Control (TC Gatwick)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| Radar / INT | `EGKK_APP` | Gatwick Approach | 126.825 MHz |
| Director / FIN | `EGKK_F_APP` | Gatwick Director | 124.525 MHz |

---

## Radio Navigation & Landing Aids

| Type | Identifier | Frequency | Runway |
|------|-----------|-----------|--------|
| ILS/DME | I-GG | 110.900 MHz | 08L |
| ILS/DME | I-GLL | 109.900 MHz | 26R |
| ILS/DME | I-GR | 110.900 MHz | 08R |
| ILS/DME | I-GLR | 109.900 MHz | 26L |

---

## Runways

| Designator | Length | Cat |
|-----------|--------|-----|
| **08L / 26R** | 3,316 m | CAT III |
| **08R / 26L** | 2,565 m | CAT I |

!!! info "Single Runway Operations"
    Gatwick normally operates as a **single runway** airport. The northern runway (08R/26L) is used for emergency diversions and during maintenance. Normal operations use 08L/26R exclusively.

### Preferential Runway

Runway **26R** is preferred in calm/westerly wind conditions. **08L** is used in easterly conditions. Runway selection is primarily wind-driven with noise abatement considerations.

---

## Altimetry

| Reference | Value |
|-----------|-------|
| Transition Altitude | 6,000 ft |
| ASR | Chatham |
| QFE offset | Approx QNH − 7 hPa |

---

## Standard Instrument Departures (SIDs)

| SID Route | 08L | 26R | Initial Climb |
|-----------|-----|-----|---------------|
| **BOGNA** | BOGNA SIDs | BOGNA SIDs | 6,000 ft |
| **CLN** (Clacton) | CLN SIDs | CLN SIDs | 6,000 ft |
| **FRANE** | — | FRANE SIDs | 6,000 ft |
| **LAM** | LAM SIDs | LAM SIDs | 6,000 ft |
| **MIMKU** | MIMKU SIDs | — | 6,000 ft |
| **NOVMA** | NOVMA SIDs | NOVMA SIDs | 6,000 ft |
| **SFD** (Seaford) | — | SFD SIDs | 6,000 ft |
| **TIMBA** | TIMBA SIDs | TIMBA SIDs | 6,000 ft |

All SIDs are RNAV1. Conventional alternatives available where published.

---

## Standard Arrival Routes (STARs)

Gatwick uses two holding stacks:

| Stack | Location | Inbound Course | Direction |
|-------|----------|---------------|----------|
| **TIMBA** | East/NE approach | — | R/H |
| **WILLO** | West/SW approach | — | L/H |

Aircraft are transferred by London TC South to TC Gatwick at the relevant stack.

---

## Departure Separation

Gatwick uses a **time-based separation** system similar to Stansted, with route groups:

| Leading \ Following | TIMBA/CLN | SFD/NOVMA | LAM/BOGNA |
|--------------------|-----------|-----------|----------|
| **TIMBA/CLN** | 2 min | 1 min | 1 min |
| **SFD/NOVMA** | 1 min | 2 min | 2 min |
| **LAM/BOGNA** | 1 min | 2 min | 2 min |

---

## Low Visibility Procedures (LVP)

LVP initiated when:
- IRVR ≤ 600 m, or
- Cloud ceiling ≤ 200 ft

Gatwick is equipped for **CAT III** operations on Runway 08L/26R.

---

## Key References

- [UK AIP – EGKK AD2 (NATS eAIP)](https://www.aurora.nats.co.uk/htmlAIP/Publications/2025-08-07-AIRAC/html/eAIP/EG-AD-2.EGKK-en-GB.html)
- [CAP 493 – MATS Part 1](https://www.caa.co.uk/cap493)
