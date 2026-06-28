# EGGW – London Luton Airport

!!! warning "SkyHigh Network Use Only"
    This page is for use on the SkyHigh simulation network only and must **never** be used for real-world operations.

## Aerodrome Overview

| Field | Value |
|-------|-------|
| **ICAO** | EGGW |
| **IATA** | LTN |
| **Full Name** | London Luton Airport |
| **Location** | Luton, Bedfordshire |
| **ARP** | 514233N 0002152W |
| **Elevation** | 526 ft AMSL |
| **Transition Altitude** | 6,000 ft |
| **Division** | SkyHigh UK & Ireland |
| **FIR** | EGTT (London) |

---

## ATC Positions

### Aerodrome Control (ADC)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| ATIS | `EGGW_ATIS` | Luton Information | 120.575 MHz |
| Delivery (GMP) | `EGGW_DEL` | Luton Delivery | 121.750 MHz |
| Ground (GMC) | `EGGW_GND` | Luton Ground | 121.750 MHz |
| Tower (AIR) | `EGGW_TWR` | Luton Tower | 132.550 MHz |

### Approach Control (TC Luton)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| Radar / INT | `EGGW_APP` | Luton Radar | 129.550 MHz |
| Director / FIN | `EGGW_F_APP` | Luton Director | 128.750 MHz |

!!! info "TC Luton Coverage"
    When TC Luton is offline, TC Stansted INT may provide top-down coverage using the `ESSEX_APP` logon. The RT callsign remains "Stansted Radar" for all services.

---

## Radio Navigation & Landing Aids

| Type | Identifier | Frequency | Runway |
|------|-----------|-----------|--------|
| ILS/DME | I-LTN | 110.100 MHz | 07 |
| ILS/DME | I-LL | 109.900 MHz | 25 |
| LUT NDB | LUT | 362 kHz | — |

---

## Runways

| Designator | Length | Cat |
|-----------|--------|-----|
| **07 / 25** | 2,162 m | CAT II |

### Preferential Runway

Runway **25** is preferred in westerly / calm conditions. **07** used for easterly winds. Runway 07/25 is Luton's single runway.

---

## Altimetry

| Reference | Value |
|-----------|-------|
| Transition Altitude | 6,000 ft |
| ASR | Chatham |

Note: Luton is the highest of the London airports at 526 ft AMSL — QFE values differ significantly from nearby Stansted and Heathrow.

---

## Standard Instrument Departures (SIDs)

| Route | RWY 07 | RWY 25 | Initial Climb |
|-------|--------|--------|---------------|
| **BPK** | BPK SIDs | BPK SIDs | 4,000 ft |
| **CPT** | — | CPT SIDs | 4,000 ft |
| **DET** | DET SIDs | DET SIDs | 4,000 ft |
| **LOREL** | LOREL SIDs | LOREL SIDs | 4,000 ft |
| **OCK** | — | OCK SIDs | 4,000 ft |
| **ZAGZO** | ZAGZO SIDs | ZAGZO SIDs | 4,000 ft |

---

## Standard Arrival Routes (STARs)

| Stack | Inbound | Notes |
|-------|---------|-------|
| **ABBOT** | via LAPRA / CLN | Shared with Stansted |
| **ZAGZO** | via OCK / CPT | Luton-specific |

---

## Low Visibility Procedures (LVP)

LVP initiated when:
- IRVR ≤ 600 m, or
- Cloud ceiling ≤ 200 ft

Runway 07/25 equipped for **CAT II** operations.

---

## Key References

- [UK AIP – EGGW AD2 (NATS eAIP)](https://www.aurora.nats.co.uk/htmlAIP/Publications/2025-08-07-AIRAC/html/eAIP/EG-AD-2.EGGW-en-GB.html)
- [CAP 493 – MATS Part 1](https://www.caa.co.uk/cap493)
