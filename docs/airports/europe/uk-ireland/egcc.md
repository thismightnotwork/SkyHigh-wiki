# EGCC – Manchester Airport

!!! warning "SkyHigh Network Use Only"
    This page is for use on the SkyHigh simulation network only and must **never** be used for real-world operations.

## Aerodrome Overview

| Field | Value |
|-------|-------|
| **ICAO** | EGCC |
| **IATA** | MAN |
| **Full Name** | Manchester Airport |
| **Location** | Manchester, Greater Manchester |
| **ARP** | 532128N 0021619W |
| **Elevation** | 257 ft AMSL |
| **Transition Altitude** | 6,000 ft |
| **Division** | SkyHigh UK & Ireland |
| **FIR** | EGTT (London) |

---

## ATC Positions

### Aerodrome Control (ADC)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| ATIS | `EGCC_ATIS` | Manchester Information | 128.175 MHz |
| Delivery (GMP) | `EGCC_DEL` | Manchester Delivery | 121.855 MHz |
| Ground (GMC) | `EGCC_GND` | Manchester Ground | 121.700 MHz |
| Tower (AIR) | `EGCC_TWR` | Manchester Tower | 118.625 MHz |
| Tower 2 | `EGCC_2_TWR` | Manchester Tower | 119.400 MHz |

### Approach Control

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| Radar / INT | `EGCC_APP` | Manchester Radar | 119.725 MHz |
| Director / FIN | `EGCC_F_APP` | Manchester Director | 121.350 MHz |

---

## Radio Navigation & Landing Aids

| Type | Identifier | Frequency | Runway |
|------|-----------|-----------|--------|
| ILS/DME | I-MAN | 110.500 MHz | 05L |
| ILS/DME | I-MRS | 109.500 MHz | 05R |
| ILS/DME | I-MAN | 110.500 MHz | 23R |
| ILS/DME | I-MRS | 109.500 MHz | 23L |
| MAN VOR/DME | MAN | 113.550 MHz | — |

---

## Runways

| Designator | Length | Cat |
|-----------|--------|-----|
| **05L / 23R** | 3,048 m | CAT III |
| **05R / 23L** | 3,048 m | CAT III |

### Runway Usage

Manchester operates in **independent parallel** mode or **segregated mode** depending on traffic levels and ATC staffing:

- **Segregated:** One runway arrivals only, one departures only
- **Independent parallel:** Both runways simultaneously for arrivals or departures
- The **southerly runway (05R/23L)** is normally preferred for operations when single runway is in use

---

## Altimetry

| Reference | Value |
|-----------|-------|
| Transition Altitude | 6,000 ft |
| ASR | Manchester |

---

## Standard Instrument Departures (SIDs)

| Route | 05L | 05R | 23R | 23L | Notes |
|-------|-----|-----|-----|-----|-------|
| **DESIG** | ✅ | ✅ | ✅ | ✅ | North-eastern departures |
| **LISTO** | ✅ | ✅ | ✅ | ✅ | Southern / SW departures |
| **MONTY** | ✅ | ✅ | ✅ | ✅ | Western departures |
| **POL** | ✅ | ✅ | ✅ | ✅ | Northern departures |
| **SANBA** | ✅ | ✅ | ✅ | ✅ | SE departures |
| **UPTON** | ✅ | ✅ | ✅ | ✅ | SW/western |

All SIDs are RNAV1. Initial climb is typically **5,000 ft** for standard jet departures.

---

## Standard Arrival Routes (STARs)

Manchester uses **two holding stacks**:

| Stack | Location | Inbound | Levels |
|-------|----------|---------|--------|
| **DAYNE** | NE (via Pole Hill) | NE approaches | FL70–FL130 |
| **MIRSI** | SE (via Wallasey) | SW/W approaches | FL70–FL130 |

---

## Low Visibility Procedures (LVP)

LVP initiated when:
- IRVR ≤ 600 m, or
- Cloud ceiling ≤ 200 ft

Both runways are equipped for CAT III operations.

---

## Noise Abatement

All jet aircraft and aircraft exceeding 5,700 kg MTOW must comply with the published NPR. NPR are mandatory from take-off to 4,000 ft. Preferential arrival routings avoid residential areas south and southwest of the airport.

---

## Key References

- [UK AIP – EGCC AD2 (NATS eAIP)](https://www.aurora.nats.co.uk/htmlAIP/Publications/2025-08-07-AIRAC/html/eAIP/EG-AD-2.EGCC-en-GB.html)
- [CAP 493 – MATS Part 1](https://www.caa.co.uk/cap493)
