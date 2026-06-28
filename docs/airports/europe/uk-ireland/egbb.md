# EGBB – Birmingham Airport

!!! warning "SkyHigh Network Use Only"
    This page is for use on the SkyHigh simulation network only and must **never** be used for real-world operations.

## Aerodrome Overview

| Field | Value |
|-------|-------|
| **ICAO** | EGBB |
| **IATA** | BHX |
| **Full Name** | Birmingham Airport |
| **Location** | Solihull, West Midlands |
| **ARP** | 522718N 0014448W |
| **Elevation** | 325 ft AMSL |
| **Transition Altitude** | 6,000 ft |
| **Division** | SkyHigh UK & Ireland |
| **FIR** | EGTT (London) |

---

## ATC Positions

### Aerodrome Control (ADC)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| ATIS | `EGBB_ATIS` | Birmingham Information | 126.025 MHz |
| Delivery (GMP) | `EGBB_DEL` | Birmingham Delivery | 121.805 MHz |
| Ground (GMC) | `EGBB_GND` | Birmingham Ground | 121.805 MHz |
| Tower (AIR) | `EGBB_TWR` | Birmingham Tower | 118.305 MHz |

### Approach Control

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| Radar | `EGBB_APP` | Birmingham Radar | 118.050 MHz |
| Director | `EGBB_F_APP` | Birmingham Director | 131.325 MHz |

---

## Radio Navigation & Landing Aids

| Type | Identifier | Frequency | Runway |
|------|-----------|-----------|--------|
| ILS/DME | I-BHX | 110.900 MHz | 15 |
| ILS/DME | I-BB | 108.750 MHz | 33 |
| BHX VOR/DME | BHX | 113.050 MHz | — |

---

## Runways

| Designator | Length | Cat |
|-----------|--------|-----|
| **15 / 33** | 3,052 m | CAT II |

### Preferential Runway

Runway **15** is the preferred runway for departures in calm conditions due to noise abatement considerations (avoids the city centre). The active runway selection is wind-driven; runway **33** is used in northerly winds.

---

## Altimetry

| Reference | Value |
|-----------|-------|
| Transition Altitude | 6,000 ft |
| ASR | Barnsley |

---

## Standard Instrument Departures (SIDs)

| Route | RWY 15 | RWY 33 | Initial Climb |
|-------|--------|--------|---------------|
| **CPT** | CPT SIDs | CPT SIDs | 4,000 ft |
| **COWLY** | COWLY SIDs | COWLY SIDs | 4,000 ft |
| **LISTO** | LISTO SIDs | — | 4,000 ft |
| **TNT** | TNT SIDs | TNT SIDs | 4,000 ft |
| **UPTON** | UPTON SIDs | UPTON SIDs | 4,000 ft |

All SIDs are RNAV1 with conventional alternatives.

---

## Standard Arrival Routes (STARs)

| Stack | Inbound | Notes |
|-------|---------|-------|
| **CHASE** | From the south/SE | Typical for east/south-bound inbounds |
| **TAMOP** | From the north/NW | Typical for north-bound inbounds |

---

## Low Visibility Procedures (LVP)

LVP initiated when:
- IRVR ≤ 600 m, or
- Cloud ceiling ≤ 200 ft

Birmingham is equipped for **CAT II** operations.

---

## Key References

- [UK AIP – EGBB AD2 (NATS eAIP)](https://www.aurora.nats.co.uk/htmlAIP/Publications/2025-08-07-AIRAC/html/eAIP/EG-AD-2.EGBB-en-GB.html)
- [CAP 493 – MATS Part 1](https://www.caa.co.uk/cap493)
