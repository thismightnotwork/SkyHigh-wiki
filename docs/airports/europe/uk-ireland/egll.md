# EGLL – London Heathrow

!!! warning "SkyHigh Network Use Only"
    This page is for use on the SkyHigh simulation network only and must **never** be used for real-world operations.

## Aerodrome Overview

| Field | Value |
|-------|-------|
| **ICAO** | EGLL |
| **IATA** | LHR |
| **Full Name** | London Heathrow Airport |
| **Location** | Hillingdon, Greater London |
| **ARP** | 513028N 0002729W |
| **Elevation** | 83 ft AMSL |
| **Transition Altitude** | 6,000 ft |
| **Safety Altitude** | 2,500 ft |
| **Division** | SkyHigh UK & Ireland |
| **FIR** | EGTT (London) |

---

## ATC Positions

### Aerodrome Control (ADC)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| ATIS | `EGLL_ATIS` | Heathrow Information | 128.075 MHz |
| Delivery (GMP) | `EGLL_DEL` | Heathrow Delivery | 121.970 MHz |
| Ground North (GMC) | `EGLL_N_GND` | Heathrow Ground | 121.900 MHz |
| Ground South (GMC) | `EGLL_S_GND` | Heathrow Ground | 121.700 MHz |
| Tower 1 (AIR) | `EGLL_1_TWR` | Heathrow Tower | 118.705 MHz |
| Tower 2 (AIR) | `EGLL_2_TWR` | Heathrow Tower | 124.475 MHz |

### Approach Control (TC Heathrow)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| INT North | `EGLL_N_APP` | Heathrow Radar | 119.725 MHz |
| INT South | `EGLL_S_APP` | Heathrow Radar | 134.975 MHz |
| Final North | `EGLL_NF_APP` | Heathrow Director | 120.400 MHz |
| Final South | `EGLL_SF_APP` | Heathrow Director | 126.725 MHz |

---

## Radio Navigation & Landing Aids

| Type | Identifier | Frequency | Runway |
|------|-----------|-----------|--------|
| ILS/DME | I-LL | 109.500 MHz | 09L |
| ILS/DME | I-LW | 110.300 MHz | 09R |
| ILS/DME | I-LL | 109.500 MHz | 27R |
| ILS/DME | I-LW | 110.300 MHz | 27L |
| ATIS | — | 128.075 MHz | — |

---

## Runways

| Designator | Length | Cat |
|-----------|--------|-----|
| **09L / 27R** | 3,902 m | CAT III |
| **09R / 27L** | 3,660 m | CAT III |

### Runway Usage

Heathrow operates **segregated mode** — one runway is dedicated to arrivals, one to departures. The standard configuration is:

- **Easterly operations (09s):** 09L arrivals, 09R departures
- **Westerly operations (27s):** 27R arrivals, 27L departures

Runway alternation takes place at **1500 local** during westerly operations (noise abatement). Simultaneous use of both runways for the same purpose requires coordination with London TC.

---

## Altimetry

| Reference | Value |
|-----------|-------|
| Transition Altitude | 6,000 ft |
| ASR | Chatham |

The Heathrow QNH is the reference for the London TMA Transition Level / Minimum Stack Level table used across the entire LTMA. Arriving aircraft below the Transition Altitude are issued the Heathrow QNH.

---

## Standard Instrument Departures (SIDs)

Heathrow uses **RNAV1 SIDs** from all runways. The primary departure routes and their initial climb altitudes are:

| SID Route | 09L / 09R | 27R / 27L | Initial Climb |
|-----------|-----------|-----------|---------------|
| CPT (Compton) | CPT SIDs | CPT SIDs | 6,000 ft |
| DET (Detling) | DET SIDs | DET SIDs | 6,000 ft |
| LAM (Lambourne) | LAM SIDs | — | 6,000 ft |
| LOREL | LOREL SIDs | — | 6,000 ft |
| MID (Midhurst) | — | MID SIDs | 6,000 ft |
| OCK (Ockham) | OCK SIDs | OCK SIDs | 6,000 ft |
| SAM (Southampton) | — | SAM SIDs | 6,000 ft |
| WOD (Woodley) | WOD SIDs | WOD SIDs | 6,000 ft |

All departures are subject to Noise Preferential Routings (NPR) as published in UK AIP EGLL AD 2.21.

---

## Standard Arrival Routes (STARs)

Heathrow uses four holding stacks:

| Stack | Direction | Inbound | From |
|-------|-----------|---------|------|
| **LAMBOURNE (LAM)** | NE | R/H | 8,000–15,000 ft |
| **BIGGIN (BIG)** | SE | L/H | 7,000–15,000 ft |
| **OCKHAM (OCK)** | SW | R/H | 7,000–15,000 ft |
| **BOVINGDON (BNN)** | NW | L/H | 7,000–15,000 ft |

Aircraft are released from the stacks by London TC (TC North, TC South etc.) to TC Heathrow for sequencing to final approach.

---

## Holding Procedures

| Hold | Speed | Levels |
|------|-------|--------|
| LAM | 220 kt | FL80–FL150 |
| BIG | 220 kt | FL70–FL150 |
| OCK | 220 kt | FL70–FL150 |
| BNN | 220 kt | FL80–FL150 |

---

## Low Visibility Procedures (LVP)

LVP are initiated when:
- IRVR ≤ 600 m, or
- Cloud ceiling ≤ 200 ft

Heathrow is equipped for **CAT III** operations on all four runway ends. During LVP, mandatory CAT II/III holding points are used and runway occupancy is strictly one aircraft at a time.

---

## Noise Abatement

- **Daytime curfew exemptions:** Limited night movements between 2330–0600 local
- Noise preferential routes mandatory for all jet aircraft and all aircraft >5,700 kg MTOW
- NPR terminate at 4,000 ft or as published per SID

---

## Key References

- [UK AIP – EGLL AD2 (NATS eAIP)](https://www.aurora.nats.co.uk/htmlAIP/Publications/2025-08-07-AIRAC/html/eAIP/EG-AD-2.EGLL-en-GB.html)
- [CAP 493 – MATS Part 1](https://www.caa.co.uk/cap493)
- [CAP 413 – Radiotelephony Manual](https://www.caa.co.uk/cap413)
