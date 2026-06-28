# EGPF – Glasgow Airport

!!! warning "SkyHigh Network Use Only"
    This page is for use on the SkyHigh simulation network only and must **never** be used for real-world operations.

## Aerodrome Overview

| Field | Value |
|-------|-------|
| **ICAO** | EGPF |
| **IATA** | GLA |
| **Full Name** | Glasgow Airport |
| **Location** | Renfrewshire, Scotland |
| **ARP** | 554152N 0042534W |
| **Elevation** | 26 ft AMSL |
| **Transition Altitude** | 6,000 ft |
| **Division** | SkyHigh UK & Ireland |
| **FIR** | EGPX (Scottish) |

---

## ATC Positions

### Aerodrome Control (ADC)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| ATIS | `EGPF_ATIS` | Glasgow Information | 135.850 MHz |
| Ground (GMC) | `EGPF_GND` | Glasgow Ground | 121.700 MHz |
| Tower (AIR) | `EGPF_TWR` | Glasgow Tower | 118.805 MHz |

### Approach Control

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| Radar | `EGPF_APP` | Glasgow Radar | 119.100 MHz |
| Director | `EGPF_F_APP` | Glasgow Director | 119.100 MHz |

---

## Radio Navigation & Landing Aids

| Type | Identifier | Frequency | Runway |
|------|-----------|-----------|--------|
| ILS/DME | I-GLA | 110.100 MHz | 05 |
| ILS/DME | I-GL | 108.750 MHz | 23 |
| GOW VOR/DME | GOW | 115.400 MHz | — |

---

## Runways

| Designator | Length | Cat |
|-----------|--------|-----|
| **05 / 23** | 2,658 m | CAT III |
| **09 / 27** | 1,012 m | CAT I (crosswind) |

### Preferential Runway

Runway **23** is preferred in south-westerly conditions (prevailing). Runway **05** is used in north-easterly winds.

---

## Altimetry

| Reference | Value |
|-----------|-------|
| Transition Altitude | 6,000 ft |
| ASR | Scottish |

---

## Standard Instrument Departures (SIDs)

| Route | RWY 05 | RWY 23 | Initial Climb |
|-------|--------|--------|---------------|
| **LUSIV** | ✅ | ✅ | 6,000 ft |
| **NORBO** | ✅ | ✅ | 6,000 ft |
| **PTH** | ✅ | ✅ | 6,000 ft |
| **ROBBO** | ✅ | ✅ | 6,000 ft |
| **TLA** | ✅ | ✅ | 6,000 ft |

All SIDs are RNAV1. Coordinated with Scottish Control (EGPX).

---

## Standard Arrival Routes (STARs)

| Stack | Inbound |
|-------|---------|
| **STIRA** | E/SE approaches |
| **TLA** | N/NW approaches |

---

## Low Visibility Procedures (LVP)

LVP initiated when:
- IRVR ≤ 600 m, or
- Cloud ceiling ≤ 200 ft

Runway 05/23 is equipped for **CAT III** operations.

---

## Key References

- [UK AIP – EGPF AD2 (NATS eAIP)](https://www.aurora.nats.co.uk/htmlAIP/Publications/2025-08-07-AIRAC/html/eAIP/EG-AD-2.EGPF-en-GB.html)
- [CAP 493 – MATS Part 1](https://www.caa.co.uk/cap493)
