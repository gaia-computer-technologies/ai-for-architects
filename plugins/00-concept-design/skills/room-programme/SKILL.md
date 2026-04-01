# /room-programme

Generate a spatial programme (schedule of accommodation) from a project brief, with area benchmarks, adjacency logic, and efficiency calculations.

## When to use

- Translating a client brief into measurable spatial requirements before design begins
- Checking whether a brief fits on a site or within a budget envelope
- Structuring a competition brief into a workable schedule
- Comparing a proposed design against programmatic benchmarks

## Input

- Building type (residential, office, school, gallery, clinic, hotel, etc.)
- Number of users / occupants / units
- Any specific room requirements from the client
- Site area and/or gross floor area constraint (if known)
- Budget bracket (affects specification and therefore area)
- Regulatory context (country/region, for code-driven minimums)

## Process

1. Identify building type and pull relevant area benchmarks from the domain knowledge below.
2. List all required spaces, starting from the client brief and filling in standard adjacencies they may not have mentioned (storage, plant, circulation, WCs).
3. Assign net area to each space using benchmarks, adjusted for project ambition and budget.
4. Calculate circulation and wall thickness allowance (typically 15-25% of net area).
5. Calculate gross floor area. Check against site constraints (plot ratio, footprint, height).
6. Map adjacency relationships: what must be near what, what must be separated.
7. Identify the served/servant split (Kahn's concept) -- which spaces are primary and which support them.

## Domain knowledge

### Area benchmarks by room type

**Residential (per unit)**
- Single bedroom: 7.5-9 m2 (UK min 7.5, comfortable 11-14)
- Double bedroom: 11.5-15 m2 (UK min 11.5, generous 16-20)
- Living room: 15-25 m2 (small apartment) / 25-40 m2 (house)
- Kitchen: 8-12 m2 (galley/compact) / 15-25 m2 (kitchen-dining)
- Bathroom: 3.5-5 m2 (standard) / 6-10 m2 (en-suite generous)
- WC/cloakroom: 1.5-2.5 m2
- Hallway/entrance: 3-6 m2
- Storage: 2-4 m2 per unit (often under-programmed -- clients always need more)
- Utility/laundry: 3-5 m2
- Home office: 6-10 m2

**Office**
- Open plan workspace: 8-12 m2 per person (NEN 1824 / BCO standards)
- Private office: 12-18 m2
- Meeting room (4 person): 10-14 m2
- Meeting room (8 person): 18-24 m2
- Boardroom (16 person): 40-55 m2
- Breakout / informal: 2-3 m2 per person
- Reception: 15-40 m2 depending on corporate ambition
- Server room: 10-20 m2 (diminishing with cloud, but still needed)
- WCs: 1 per 15-20 persons (check local code)

**Education (primary/secondary)**
- Classroom: 55-63 m2 for 30 pupils (BB103 UK standard)
- Science lab: 80-90 m2
- Art/DT workshop: 80-100 m2
- Library/resource: 80-150 m2
- Assembly/sports hall: 180-600 m2 depending on school size
- Staff room: 30-50 m2
- Admin/reception: 20-40 m2
- Kitchen/servery: 50-120 m2
- WCs: per pupil ratios vary by code and age group

**Cultural / gallery**
- Gallery space: allow 25-40 m2 per artwork for comfortable viewing
- Temporary exhibition: 200-800 m2 per show
- Storage/archive: 30-50% of exhibition area (often more)
- Workshop/conservation: 50-150 m2
- Cafe: 1.5-2 m2 per seat
- Shop: 30-80 m2
- Reception/foyer: 50-200 m2 depending on throughput

**Healthcare (clinic scale)**
- Consulting room: 14-16 m2
- Treatment room: 16-20 m2
- Waiting area: 1.5 m2 per seat, seats = 2-3x simultaneous consultations
- Reception/admin: 12-20 m2
- Accessible WC: 4-5 m2
- Clean utility: 8-10 m2
- Dirty utility: 6-8 m2

### Adjacency logic

**Wet room clustering**: kitchens, bathrooms, WCs, utility rooms should share wet walls for plumbing efficiency. Vertical stacking in multi-storey buildings saves significant cost.

**Public-private gradient**: arrange spaces from most public (entrance, reception) to most private (bedrooms, consulting rooms) with a clear threshold sequence. The gradient should be legible in the plan without signage.

**Served-servant (Kahn)**: identify which spaces are the reason the building exists (served) and which support them (servant). In a house: living spaces are served, storage and bathrooms are servant. In a hospital: wards are served, corridors and service rooms are servant. Servant spaces can be compressed and tucked; served spaces get the light and volume.

**Noise separation**: separate noisy spaces (kitchen, children's areas, plant, assembly) from quiet spaces (bedrooms, offices, consulting rooms). Use buffer zones (corridors, storage, WCs) as acoustic breaks.

**Daylight access**: all occupied spaces should have access to natural light. Place servant spaces (storage, plant, WCs) in the dark core. Place served spaces on the perimeter.

**Fire escape**: every occupied space needs two means of escape (or a single escape if travel distance is short enough). Factor this into adjacency planning early.

### Circulation percentages

- Residential: 15-20% of net area (lower for open-plan, higher for corridor-access apartments)
- Office: 20-25% (including lift lobbies, corridors, stairways)
- Education: 25-30% (wide corridors, gathering spaces, cloakrooms)
- Healthcare: 30-35% (double-loaded corridors, gurney widths, waiting areas)
- Gallery: 20-25% (circulation is often part of the experience)

### Efficiency ratios (net-to-gross)

- Detached house: 85-90% (very efficient, minimal circulation)
- Apartment building: 70-80% (common corridors, lift lobbies, fire stairs eat area)
- Office: 75-85% (depends on core configuration)
- School: 65-75%
- Hospital: 55-65% (large amount of service area)

Net-to-gross below 70% should trigger a plan review. Either the circulation is genuinely necessary (hospital, complex section) or the plan is inefficient.

### Wall thickness allowance

Add 5-8% to net areas for wall construction, depending on:
- Timber frame: thin walls, ~5%
- Masonry/concrete: thicker, ~7-8%
- Acoustic separation (party walls, between uses): up to 350mm per wall

## Output format

```
## Spatial Programme: [Project Name]

### Summary
- Building type: [type]
- Total net area: [X] m2
- Circulation allowance: [Y]% = [Z] m2
- Wall allowance: [W]% = [V] m2
- **Gross floor area: [GFA] m2**

### Schedule of Accommodation

| # | Space | Net area (m2) | Qty | Total (m2) | Notes |
|---|---|---|---|---|---|
| 1 | ... | ... | ... | ... | ... |

### Adjacency requirements
- [Space A] must adjoin [Space B] — [reason]
- [Space C] must be separated from [Space D] — [reason]

### Served / servant split
- Served spaces (total: X m2): [list]
- Servant spaces (total: Y m2): [list]
- Ratio: [X:Y] — [comment on whether this is typical]

### Assumptions
- [Key assumptions about occupancy, regulation, ambition level]
```

## What you don't do

- Do not generate areas without stating the benchmark source or basis. Ungrounded numbers are meaningless.
- Do not forget circulation. A schedule of rooms without circulation allowance is not a programme -- it's a wish list.
- Do not treat area benchmarks as rules. They are starting points. A 7.5 m2 bedroom meets UK minimum but is not a good room. Say so.
- Do not omit storage, plant, and bin stores. These are the spaces clients forget and architects regret.
- Do not produce a flat list. Adjacency and hierarchy are the whole point of a programme -- without them, it's just a spreadsheet.
