# EGSS – London Stansted

!!! warning "SkyHigh Network Use Only"
    This page is for use on the SkyHigh simulation network only and must **never** be used for real-world operations. All procedures are adapted from the UK AIP and CAP 493 (MATS Part 1) for simulation purposes.

## Aerodrome Overview

| Field | Value |
|-------|-------|
| **ICAO** | EGSS |
| **IATA** | STN |
| **Full Name** | London Stansted Airport |
| **Location** | Essex, England |
| **ARP** | 515306N 0001406E |
| **Elevation** | 348 ft AMSL |
| **Transition Altitude** | 6,000 ft |
| **Safety Altitude (MSA)** | 2,100 ft |
| **Magnetic Variation** | ~2°W |
| **Division** | SkyHigh UK & Ireland |
| **FIR** | EGTT (London) |

---

## ATC Positions

### Aerodrome Control (ADC)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| ATIS | `EGSS_ATIS` | Stansted Information | 127.180 MHz |
| Delivery (GMP) | `EGSS_DEL` | Stansted Delivery | 121.955 MHz |
| Ground (GMC) | `EGSS_GND` | Stansted Ground | 121.730 MHz |
| Tower (AIR) | `EGSS_TWR` | Stansted Tower | 123.805 MHz |

### Approach Control (APC – TC Stansted)

| Position | Logon Callsign | RT Callsign | Frequency |
|----------|---------------|-------------|----------|
| Radar / INT | `EGSS_APP` | Stansted Radar | 120.625 MHz |
| Director / FIN | `EGSS_F_APP` | Stansted Director | 136.200 MHz |
| Essex Combined INT | `ESSEX_APP` | Stansted Radar | 120.625 MHz |

!!! info "Position Bandboxing"
    GMP may only be staffed when GMC is online. If GMP is closed, GMC (or AIR top-down) assumes Delivery responsibilities. INT is the first APC position opened. FIN requires AIR to be online.

---

## Radio Navigation & Landing Aids

| Type | Identifier | Frequency | Remarks |
|------|-----------|-----------|--------|
| ILS/DME RWY 04 | I-SED | 110.500 MHz | LLZ / GP / DME – 3° glideslope |
| ILS/DME RWY 22 | I-SX | 110.500 MHz | LLZ / GP / DME – 3° glideslope |
| ATIS | — | 127.180 MHz | Also available on Clacton VOR 114.550 MHz |

---

## Runways

| Designator | Bearing | Length | Cat II/III |
|-----------|---------|--------|-----------|
| **04** | 042° | 3,048 m | ✅ |
| **22** | 222° | 3,048 m | ✅ |

### Preferential Runway

Runway **22** is preferred whenever the tailwind component is **5 knots or less** and the runway surface is **dry**. In calm or crosswind conditions, the TAF and winds at 2,000 ft should be used to determine the best runway in use. AIR is responsible for runway selection.

---

## Altimetry

| Reference | Value |
|-----------|-------|
| Transition Altitude | 6,000 ft |
| QFE offset | QNH − 12 hPa |
| ASR | Chatham |

### Transition Level Table (London TMA)

| Heathrow QNH (hPa) | Transition Level | Min Stack Level |
|--------------------|-----------------|----------------|
| 1050 – 1060 | FL60 | FL70 |
| 1032 – 1049 | FL65 | FL70 |
| 1013 – 1031 | FL70 | FL70 |
| 995 – 1012 | FL75 | FL80 |
| 977 – 994 | FL80 | FL80 |
| 959 – 976 | FL85 | FL90 |
| 940 – 958 | FL90 | FL90 |

Departing aircraft should state the QNH on first contact with GMP. Arriving aircraft below the transition level are to fly with reference to the Stansted QNH. QFE may be requested by pilots on final approach.

---

## Ground Movement Planner (GMP) – Stansted Delivery

### Responsibilities

GMP issues ATC departure clearances and verifies flight plan validity. GMP shall:

- Verify aircraft type, stand, ATIS letter and QNH on initial call
- Check route validity to at least the London/Scottish FIR boundary per the Standard Route Document (SRD)
- Confirm flight level is appropriate for direction of flight
- Update the data-block with flight rules, cleared level and SSR code

### Clearance Format

Clearances are issued in the following sequence:

1. Callsign
2. Clearance Limit (destination)
3. Standard Instrument Departure (SID)
4. SSR Code (Squawk)

> **Example:** *"EZY123, cleared to Edinburgh, NUGBO 1 Romeo departure, squawk 0312"*  
> **Readback confirmation:** *"EZY123, correct. Information Alpha, Stansted QNH 1013."*

### Pre-Departure Clearance (PDC)

Datalink clearances (PDC) are available via TopSky, vStrips, vSMR or Hoppie ACARS. PDC **must not** be issued:

- Within 30 minutes of a runway change (auto-PDC must be deactivated)
- When the route requires amendment or re-routing

### Flights to Local Airfields

For flights to airports within the London TMA, GMP must initiate delay absorption coordination with the receiving TC sector before transferring to GMC.

| Destination | SID | Route | Coordination |
|-------------|-----|-------|-------------|
| Luton (EGGW) | BKY | DCT BKY DCT BUSTA | TC Luton INT |
| Cambridge (EGSC) | BKY | DCT BKY DCT | Cambridge APC |
| Thames Group (EGLC/EGKB/EGMC) | CLN | CLN DCT LOGAN | TC North East |
| Heathrow / Northolt (EGLL/EGWU) | CLN | CLN DCT LAM | TC North East |
| Gatwick (EGKK) | DET | DET DCT TIMBA | TC North East / TC South East |
| Farnborough / Southampton / Bournemouth | NUGBO | NUGBO DCT SILVA DCT CPT | TC NW |
| Birmingham (EGBB) | UTAVA | UTAVA Q75 BUZAD | TC NW |

---

## Ground Movement Control (GMC) – Stansted Ground

### Responsibilities

GMC is responsible for all aircraft movements on aprons and taxiways, excluding the active runway and holding points. GMC also assumes GMP duties when Delivery is offline.

### Pushback Clearance

Pushback clearances include the stand number for situational awareness:

> **Example:** *"EZY123, stand 22, push and start approved."*

Turboprop aircraft shall be passed the outside air temperature with start clearance. All south-side aprons have a single entry/exit direction — push direction need not be specified. Aircraft on the G apron (north side) may need clarification.

### Runway Crossings

All crossings of the active runway must be conducted on the AIR frequency — clearance is **not** to be relayed by GMC. When Runway 22 is in use, GMC must not taxi aircraft to N1 due to the risk of conflict with the rapid exit taxiway NR.

> **Example:** *"EZY123, taxi Alpha, Hotel, hold short taxiway November."*

### Taxiway Restrictions

| Location | Restriction |
|----------|------------|
| Taxiway G (past G3) | Max wingspan 36 m when Runway 04 in use — traffic should cross at V |
| Link D / H east of Link D | Max wingspan 52.9 m |
| Link E | Max wingspan 36 m |

**Code F aircraft** (A380, B747-8) may use stands: 6, 9, 204–205, 213.

### Departure Runway Holding Points

- **Runway 04:** Avoid G1 for departures where possible. Route north-side traffic to V unless runway length requires G.
- **Runway 22:** When considering departure from P instead of Q, account for wake turbulence spacing against higher-category aircraft at R/S.

### Stand Allocation

| Stands | Operator |
|--------|----------|
| 1 – 6 | Cargo (excl. FedEx) |
| 10 – 34 | All airlines (excl. Ryanair) |
| 40 – 85 | Ryanair (exclusively) |
| 204 – 214 | FedEx only |
| 501 – 509 | Executive aircraft |
| 510 – 515, 517, 519 | Long-stay executive |
| 516, 518 | Non-passenger Titan flights |

---

## Air Control (AIR) – Stansted Tower

### Responsibilities

AIR is responsible for:

- Safe and expeditious use of the active runway and rapid exit taxiways
- Provision of information to aircraft on instrument approach
- Control of VFR aircraft in the visual circuit
- Obtaining departure releases from TC Stansted / London TC as required

### Line-Up Procedures

All line-up instructions must include:

1. Runway designator
2. Holding point designator for runway entry
3. For crossing traffic: holding point designator for runway exit

Multiple simultaneous line-ups are permitted with sufficient jet blast separation:

| Runway | Permitted combination |
|--------|----------------------|
| **22** | R/S and Q; Q and P |
| **04** | H/G and K; K and L |

### Conditional Clearances

- Conditionals behind arriving traffic must include the distance from touchdown
- Only issue a conditional against the **first** aircraft on approach
- The word **"follow"** must **not** be used in runway conditionals
- Maximum of **two** active conditionals at any one time

> **Example:** *"EZY456 behind the landing Boeing 737-800 at 3 miles, via R1, line up Runway 22 behind."*

### Runway Vacation Guidelines

Rapid exit taxiways PR, QR, NR and LR are designed for 52-knot exit speed. Pilots **must not** stop on any rapid exit taxiway.

| Runway | Preferred exit |
|--------|---------------|
| **22** | NR or LR permitted |
| **04** | PR — pilots should not extend roll beyond PR unless authorised |

### Special Landing Procedures

A landing clearance may be issued while a departing aircraft occupies the runway, provided:

- Daylight hours only, dry runway
- Visibility ≥ 6 km, ceiling ≥ 1,000 ft
- Both aircraft normal operations, landing aircraft IAS < 160 kt
- At time of threshold crossing, departing aircraft is ≥ 2,500 m from threshold (or ≥ 2,000 m and airborne)

> **Phraseology:** *"(Callsign) after the departing (Aircraft Type) cleared to land Runway (04/22)"*

### Departure Separation

#### Speed Groups

| Group | Aircraft |
|-------|----------|
| **4** | All jet aircraft (excl. Group 3 / Concorde / Military) |
| **3** | BAe146/RJ, CRJ series, E135/145, DH8D, SB20 etc. |
| **2** | ATR variants, DH8A/B/C, F50, King Air, SF34, SW3/4 etc. |
| **1** | BN2, C208, DA62, DHC6 etc. |

#### Route Separation (minutes, same speed group)

| Leading \ Following | CLN/DET | UTAVA/BKY | NUGBO |
|--------------------|---------|-----------|-------|
| **CLN/DET** | 2 | 1 | 1 |
| **UTAVA/BKY** | 1 | 2 | 2 |
| **NUGBO** | 1 | 2 | **3** |

!!! warning
    NUGBO following NUGBO is **always 3 minutes**, even if the preceding departure was not via NUGBO.

When a faster aircraft follows a slower one, add 1 minute per speed group difference. The interval may reduce to 1 minute if the following aircraft is 2 or more groups slower.

### Departure Releases (Subjects)

AIR must obtain a release from **Stansted FIN** before issuing take-off clearance for:

- Traffic to EGGW or EGSC
- Non-airways IFR and SVFR departures
- Airways departures unable to fly or deviating from SID/NPR
- Any subsequent SID departure after the above
- First departure after a runway change
- First departure after a missed approach
- VFR departures not routing via standard routes

AIR must obtain a release from the **receiving controller (TC or FIN)** for:

- Aircraft types not on the speed table, or following aircraft 3 speed groups faster
- Successive aircraft separated by less than the required interval
- **All DET SID departures** (pre-note to TC Thames / TMS DIR required)

### Transfer of Control – Departures

Departures transferred **no later than 2,000 ft or 2.5 NM** from runway end. Handoff priority:

| SID | First handoff |
|-----|---------------|
| CLN / DET | TC North East (or bandbox) |
| UTAVA / NUGBO / BKY | Stansted FIN → Stansted INT → TC NW |

### Transfer of Control – Arrivals

FIN transfers arriving aircraft to AIR **no later than 6 NM from touchdown**, callsign only:

> *"Contact Stansted Tower 123.805, callsign only."*

FIN retains responsibility for radar and wake turbulence separation until touchdown. AIR may not change speed without FIN agreement.

### Missed Approach

On becoming aware of a go-around, AIR shall:

1. Activate the UKCP Go-Around Alarm
2. Restrict go-around traffic to ≤ 3,000 ft
3. Issue tactical headings only if needed to avoid an immediate conflict
4. Coordinate with FIN as soon as possible

The next departure following a missed approach requires a release from FIN.

---

## Standard Instrument Departures (SIDs)

| Route | RWY 22 SID | Initial Climb | RWY 04 SID | Initial Climb | Notes |
|-------|-----------|--------------|-----------|--------------|-------|
| **BKY** | BKY 6R | 4,000 ft | BKY 3S | 5,000 ft | Re-positioning to EGGW or via BKY only |
| **CLN** | CLN 2E† (9R) | 4,000 ft\* | CLN 5S | 4,000 ft\* | See Note 2 |
| **DET** | DET 2R | 5,000 ft | DET 2D† (2S) | 5,000 ft | See Notes 2 & 3 |
| **NUGBO** | NUGBO 1R | 4,000 ft | NUGBO 1S | 5,000 ft | See Note 3 |
| **UTAVA** | UTAVA 1R | 4,000 ft | UTAVA 1S | 5,000 ft | — |

† RNAV SID (RNP1). () = alternative for non-RNAV equipped aircraft. \* = stepped climb.

!!! note "SID Notes"
    **Note 1:** RNAV SIDs should be issued unless the pilot requests otherwise.  
    **Note 2:** DET traffic is not permitted, 0600–2300 local, to route eastbound via DVR/KONAN/VABIK/RINTI (L6, L9, L18, Q70, L10). Re-route via CLN.  
    **Note 3:** DET/LYD traffic is restricted to FL175 or below as a final cruise level (FL265 permitted for Paris TMA via XIDIL). Traffic wishing to cruise higher must re-route via NUGBO.

### Noise Preferential Routings (NPR)

NPRs are mandatory for all jet aircraft and all aircraft exceeding 5,700 kg MTOW. Stansted ATC deviates from NPR **only for safety**. NPR terminate at **4,000 ft**, except BKY/NUGBO/UTAVA SIDs between 0600–2330 local time which terminate at **3,000 ft**.

Arriving traffic may not descend below 2,000 ft before intercepting the glidepath. Between 2330–0600 local time, no aircraft shall descend below 3,000 ft until established on final approach.

---

## Standard Arrival Routes (STARs)

### Main STARs

| Designator | Route |
|-----------|-------|
| AVANT 1L | AVANT – OCK – VATON – BPK – BKY – BUSTA – **LOREL** |
| BANVA 1L | BANVA – UNDUG – MAY – VATON – BPK – BKY – BUSTA – **LOREL** |
| DET 2A | DET – LOFFO – **ABBOT** |
| FINMA 1L | FINMA – BOMBO – BKY – BUSTA – **LOREL** |
| LISTO 1L | LISTO – PEDIG – ROGBI – FINMA – BOMBO – BKY – BUSTA – **LOREL** |
| LOGAN 2A | LOGAN – CLN – **ABBOT** |
| MEGEL 1A | MEGEL – DITOB – LAPRA – **ABBOT** |
| RINIS 1A | RINIS – IDESI – LAPRA – **ABBOT** |
| SILVA 1L | SILVA – BOMBO – BKY – BUSTA – **LOREL** |
| SIRIC 1L | SIRIC – NIGIT – VATON – BPK – BKY – BUSTA – **LOREL** |
| TELTU 1L | TELTU – VATON – BPK – BKY – BUSTA – **LOREL** |
| TOSVA 1A | TOSVA – IDESI – LAPRA – **ABBOT** |
| XAMAN 1A | XAMAN – IDESI – LAPRA – **ABBOT** |

### Stack Switching STARs

| Designator | Route |
|-----------|-------|
| ABBOT 1Z | ABBOT – TABIS – BUSTA – LOREL |
| BPK 1X | BPK – ADNAM – ABBOT |
| BKY 1X | BKY – ADNAM – ABBOT |

---

## Holding Procedures

| Hold | Inbound Course | Direction | Holding Levels | Holding Speed | Notes |
|------|---------------|-----------|---------------|--------------|-------|
| **LOREL** | 187° | Left | FL70 – FL140 | 220 kt | 4.0 NM legs. No holding below FL90 (Luton interaction) |
| **ABBOT** | 264° | Right | FL80 – FL140 | 220 kt | 6.0 NM legs |

- MSL at LOREL allocated to **FIN**
- MSL at ABBOT allocated to **INT**
- LOREL inbounds released by **TC North East**
- ABBOT inbounds released by **TC East**

---

## Approach Control (TC Stansted)

### Area of Responsibility

TC Stansted (INT + FIN) is responsible for the Stansted CTR/CTAs and delegated London TMA airspace (the Stansted RMA). When TC Luton is offline, TC Stansted INT may provide a Combined APC service using the `ESSEX_APP` logon.

### Minimum Sector Altitudes (MSA – within 25 NM)

| Sector | MSA |
|--------|-----|
| NW | 2,000 ft |
| NE | 1,800 ft |
| SW | 2,100 ft |
| SE | 1,700 ft |

Lowest assignable level within the SMAA: **1,700 ft**. Aircraft on an instrument approach or cleared to establish at ≤ 40° may descend to **1,500 ft**.

### Radar Separation

TC Stansted may apply **3 NM** radar separation between identified aircraft, provided both aircraft are identified and appropriate wake turbulence separation is applied.

### Approach Speed Control

| Phase | Speed |
|-------|-------|
| Intermediate (clean) | 220 kt (or higher minimum clean speed) |
| Final approach | 165–180 kt |
| Established, 2,500–3,000 ft to 5 NM | 165 kt |

!!! note
    CDA is used for **Runway 22 only**. Due to departure conflicts with Luton and London City, CDA is **not** used for Runway 04 approaches.

### Missed Approach Procedures

| Approach | Missed Approach Procedure |
|----------|---------------------------|
| **ILS / LOC / RNP Z RWY 22** | Climb straight ahead not above 3,000 ft. At I-SX DME 3.1 (BKY R156) turn right to establish on BKY R171 (QDM 351°) by BKY DME 8, continuing climb to BKY VOR at 3,000 ft or as directed. |
| **ILS / LOC / RNP Z RWY 04** | Climb straight ahead not above 3,000 ft. At I-SED DME 2 (BKY R116) turn left to establish on BKY R101 (QDM 281°). Cross BKY DME 5 at 3,000 ft, then continue to BKY VOR at 3,000 ft or as directed. |

!!! info
    RNP missed approaches resume conventional navigation at 800 ft.

### RNP Approaches

Only **RNP Z** approaches to Runway 04 and Runway 22 are used on SkyHigh (RNP Y is for maintenance threshold use). Aircraft are radar vectored to establish on the final approach track **inside the IF but at least 2 NM prior to the FAF**. The pilot must be informed they will be vectored inside the IF. Clearance format:

> *"(Callsign), cleared RNP Zulu approach runway [04/22], QNH [hPa]."*

---

## Low Visibility Procedures (LVP)

### Initiation

LVP come into effect when:

- IRVR (or met visibility) is **≤ 600 m**, or
- Cloud ceiling is **≤ 200 ft**

AIR notifies FIN immediately. ATIS must be updated. During LVP, only one aircraft may use the runway at any one time — conditional clearances are suspended.

### CAT II/III Holding Points

| Runway | South | North |
|--------|-------|-------|
| **22** | S3, R3, Q3 | — |
| **04** | H3, K3, L3 | G3, W3 |

### Arrival Spacing During LVP

- Standard spacing increased to **10 NM** from touchdown
- May reduce to **6 NM** when no departures are expected (coordinated between FIN and AIR)
- Aircraft should be established on ILS by **10 NM** from touchdown

---

## VFR Operations

### Airspace Classification

The Stansted CTR is **Class D** from surface to 3,500 ft. Stansted CTA-1 and CTA-2 have designated **Transponder Mandatory Zones (TMZ)** from surface to 1,500 ft.

### Visual Reference Points (VRPs)

- Audley End Railway Station
- Berners Lake
- Braintree
- Canfield A120/B1256 Interchange
- Chelmsford
- Chipping Ongar A414/B184 Interchange
- Debden Disused Aerodrome
- Epping
- Hazelend Wood
- Nuthampstead Aerodrome
- Puckeridge A10/A120 Interchange
- Spriggs Solar Farm
- Ware

### Standard VFR Departure/Arrival Routes

VFR/SVFR departures are cleared to **not above 2,000 ft**, squawk **7410**:

1. Canfield A120/B1256 Interchange
2. Audley End Railway Station (via M11)
3. Nuthampstead Aerodrome via Hazelend Wood VRP
4. Puckeridge A10/A120 Interchange via Hazelend Wood VRP

VFR circuit traffic squawks **7010**. Circuits operate to the **south** of the aerodrome at **1,400 ft** (or height 1,000 ft on QFE).

!!! warning "Noise Sensitive Areas"
    Do not vector aircraft over Bishop's Stortford (west of Stansted) at any level, Sawbridgeworth or Stansted Mountfitchet below 2,500 ft, or St Elizabeth's Home (514949N 0000523E) below 4,000 ft.

### SSR Codes – VFR/Low Level

| Code | Use |
|------|-----|
| 7410 | VFR/SVFR departure (issued by ADC) |
| 7411 | VFR arrival (issued by TC Stansted) |
| 7402–7407, 7412–7414 | TC Stansted allocation range |
| 7013 | Stansted listening squawk (monitoring 120.625 MHz) |
| 7010 | VFR circuit |

---

## Aerodromes in the Vicinity

| Aerodrome | Notes |
|-----------|-------|
| Luton (EGGW) | Separate TC; shares Stansted STARs via ABBOT |
| Cambridge (EGSC) | Uses Stansted STARs; coordinated via FIN |
| Duxford (EGSU) | Licensed aerodrome; ATZ 2 NM / 2,000 ft – Class G |
| North Weald (EGSX) | Unlicensed; under CTA-2, within TMZ-2 |
| Andrewsfield (EGSL) | Grass runway 27/09; operates up to 1,500 ft QNH without ATC reference in ATZ |
| Audley End (EGO2) | Microlight/fixed wing; operates in CTR up to 1,500 ft without clearance |
| Hunsdon | Microlight; operates up to 1,000 ft under CTA-2 |

---

## Flight Level Capping

Certain destinations have maximum FL restrictions. Key examples:

| Destination / Group | Max FL |
|---------------------|--------|
| EGBB / BE / NX (Birmingham group) | FL180 |
| EGCC / GP / NR (Manchester group) | FL180 |
| EGFF / GD / SY (Cardiff group) | FL200 |
| Belfast Group | FL320 via LIPGO |
| Dublin Group | FL340 via LIPGO/VATRY |
| EH** Netherlands (excl. EHAM) | FL230 |
| EHAM | FL210 (FL290 via REDFA) |
| Brussels Group | FL230 |
| Roissy Group (LFPB/LFPG/LFPT) | FL250 |
| Lille Group | FL170 |
| LFRR FIR | FL290 |

Full capping table available in the GMP section of the Stansted MATS Part 2.

---

## Key References

- [UK AIP – EGSS AD2 (NATS eAIP)](https://www.aurora.nats.co.uk/htmlAIP/Publications/2025-08-07-AIRAC/html/eAIP/EG-AD-2.EGSS-en-GB.html)
- [CAP 493 – MATS Part 1 (Edition 12)](https://www.caa.co.uk/cap493)
- [CAP 413 – Radiotelephony Manual](https://www.caa.co.uk/cap413)
