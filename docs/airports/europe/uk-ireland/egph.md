# EGPH – Edinburgh Airport

!!! warning "SkyHigh Network Use Only"
    This page is for use on the SkyHigh simulation network only and must **never** be used for real-world operations.

## Aerodrome Overview

| Field | Value |
|-------|-------|
| **ICAO** | EGPH |
| **IATA** | EDI |
| **Full Name** | Edinburgh Airport |
| **Location** | Edinburgh, Scotland |
| **ARP** | 555716N 0031946W |
| **Elevation** | 135 ft AMSL |
| **Transition Altitude** | 6,000 ft |
| **Division** | SkyHigh UK & Ireland |
| **FIR** | EGPX (Scottish) |

---

## ATC Positions

### Aerodrome Control (ADC)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| ATIS | `EGPH_ATIS` | Edinburgh Information | 132.075 MHz |
| Delivery (GMP) | `EGPH_DEL` | Edinburgh Delivery | 121.755 MHz |
| Ground (GMC) | `EGPH_GND` | Edinburgh Ground | 121.755 MHz |
| Tower (AIR) | `EGPH_TWR` | Edinburgh Tower | 118.705 MHz |

### Approach Control

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| Radar | `EGPH_APP` | Edinburgh Radar | 121.200 MHz |
| Director | `EGPH_F_APP` | Edinburgh Director | 128.225 MHz |

---

## Radio Navigation & Landing Aids

| Type | Identifier | Frequency | Runway |
|------|-----------|-----------|--------|
| ILS/DME | I-EDN | 110.100 MHz | 06 |
| ILS/DME | I-EDI | 109.900 MHz | 24 |
| EDN VOR/DME | EDN | 114.200 MHz | — |

---

## Runways

| Designator | Length | Cat |
|-----------|--------|-----|
| **06 / 24** | 2,556 m | CAT III |
| **12 / 30** | 1,800 m | CAT I (crosswind) |

### Preferential Runway

Runway **24** is preferred in westerly conditions (prevailing wind). Runway **06** is used in easterly conditions. Runway **12/30** is the crosswind runway, normally used when the crosswind component exceeds limits on 06/24.

---

## Altimetry

| Reference | Value |
|-----------|-------|
| Transition Altitude | 6,000 ft |
| ASR | Scottish |

---

## Standard Instrument Departures (SIDs)

| Route | RWY 06 | RWY 24 | Initial Climb |
|-------|--------|--------|---------------|
| **GOSAM** | ✅ | ✅ | 6,000 ft |
| **IDRID** | ✅ | ✅ | 6,000 ft |
| **LOMON** | ✅ | ✅ | 6,000 ft |
| **LUSIV** | ✅ | ✅ | 6,000 ft |
| **RIBEL** | ✅ | — | 6,000 ft |
| **TLA** | ✅ | ✅ | 6,000 ft |

All SIDs are RNAV1. Edinburgh SIDs are coordinated with Scottish Control (EGPX).

---

## Standard Arrival Routes (STARs)

| Stack | Inbound |
|-------|---------|
| **TIPOD** | E/SE approaches |
| **TLA** | W/NW approaches |

---

## Low Visibility Procedures (LVP)

LVP initiated when:
- IRVR ≤ 600 m, or
- Cloud ceiling ≤ 200 ft

Runway 06/24 is equipped for **CAT III** operations.

---

## Key References

- [UK AIP – EGPH AD2 (NATS eAIP)](https://www.aurora.nats.co.uk/htmlAIP/Publications/2025-08-07-AIRAC/html/eAIP/EG-AD-2.EGPH-en-GB.html)
- [CAP 493 – MATS Part 1](https://www.caa.co.uk/cap493)
