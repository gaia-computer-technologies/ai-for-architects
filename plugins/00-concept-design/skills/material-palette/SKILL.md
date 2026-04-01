# /material-palette

Suggest a cohesive palette of 3-5 materials and finishes for an architectural project, based on style, budget, climate, and spatial intent.

## When to use

- Early design stages when material direction is open
- Client has named one material and you need to build a coherent family around it
- Translating a mood board into specifiable materials
- Checking whether a proposed palette has internal logic or is just a Pinterest collage

## Input

One or more of:
- Architectural style or reference projects
- Climate and orientation
- Budget bracket (social housing / mid-market / high-end / no-limit)
- One or two "anchor" materials the client has already chosen
- Spatial intent (monastic calm, industrial energy, domestic warmth, civic gravitas)

## Process

1. Identify the anchor material -- the one that sets the tone. If none given, derive from style and budget.
2. Select 2-4 supporting materials using the palette logic rules below.
3. Assign each material to a role: primary surface, secondary surface, accent, detail/hardware.
4. Check the palette against climate (will it weather well?), budget (is it buildable?), and maintenance reality.
5. Specify finish level: rough/honed/polished, treated/untreated, painted/natural.
6. Note aging characteristics -- how this palette will look in 5, 15, 50 years.

## Domain knowledge

### Material families

**Stone**
Types: limestone (warm, porous), sandstone (regional colour variation), granite (hard, flecked), marble (veined, high-end), slate (dark, layered), basalt (volcanic, black).
Light interaction: honed stone reads warm and absorbs light; polished stone reflects and feels institutional. Rough-split stone creates deep shadow lines.
Aging: limestone develops beautiful patina. Marble stains if unsealed. Granite is essentially immortal. Sandstone erodes in polluted air.
Budget: limestone and sandstone are mid-range; granite and marble are premium. Thin stone veneer drops cost by 60%.

**Timber**
Types: oak (European staple, tannin-rich), Douglas fir (structural, Pacific NW), cedar (weather-resistant, aromatic), larch (durable exterior), walnut (dark, luxurious), ash (light, flexible), pine (budget, knots), CLT/glulam (engineered structural).
Light interaction: grain pattern creates micro-texture that scatters light warmly. Dark timbers absorb; pale timbers glow.
Aging: untreated larch silvers beautifully. Cedar goes grey. Oak darkens. Accoya resists all change (engineered). Oiled finishes need maintenance every 2-5 years.
Budget: pine is cheap, oak is mid-range, walnut is premium. CLT is cost-competitive with concrete at scale.

**Metal**
Types: steel (Corten/weathering, galvanised, powder-coated, blackened), aluminium (anodised, mill-finish), zinc (standing seam, pre-patinated), copper (green patina over decades), brass (warm, tarnishes), bronze (monumental).
Light interaction: matte metals absorb and feel warm. Mirror-polished metals dematerialise a surface. Perforated metal creates dappled light.
Aging: Corten develops stable rust layer in 2-5 years (don't use near pale stone -- it stains). Zinc self-heals scratches. Copper goes green in 10-20 years depending on climate. Bronze holds up for centuries.
Budget: galvanised steel is cheap. Zinc cladding is mid-range. Copper and bronze are premium.

**Ceramic and brick**
Types: handmade brick (irregular, characterful), wirecut brick (precise, modern), glazed brick (reflective, colourful), terracotta (cladding, brise-soleil), encaustic tile, porcelain (large format).
Light interaction: glazed surfaces bounce light; matte absorbs. Brick walls modulate light through mortar joint shadows.
Aging: brick is one of the most durable claddings. Glazed brick stays crisp. Handmade brick develops character. Mortar joint colour matters as much as brick colour.
Budget: stock brick is cheap. Handmade and glazed are mid-to-premium. Large-format porcelain is premium.

**Plaster, render, and lime**
Types: lime render (breathable, traditional), cement render (harder, modern), clay plaster (warm, acoustic), tadelakt (waterproof Moroccan lime plaster), polished plaster/stucco lustro (Venetian, high-sheen).
Light interaction: matte plaster absorbs and creates soft, even surfaces. Polished plaster catches light directionally. Clay plaster has a subtle warmth that paint cannot replicate.
Aging: lime render self-heals hairline cracks. Cement render cracks and stains. Tadelakt develops depth. All plaster needs protection at vulnerable edges.
Budget: painted plasterboard is baseline. Lime render is mid-range. Tadelakt and polished plaster are premium (labour-intensive).

**Glass**
Types: float (clear), low-iron (no green tint), frosted/acid-etched, textured/reeded, coloured, structural (frameless), channel glass (U-profile).
Light interaction: clear glass connects; frosted glass diffuses; reeded glass abstracts. Coloured glass transforms light quality entirely.
Aging: glass doesn't age but frames do. Structural silicone joints yellow after 20 years. Channel glass is remarkably durable.
Budget: standard double-glazing is baseline. Low-iron and structural glass are premium. Triple-glazing adds 30-50%.

**Textile and soft materials**
Types: acoustic felt (wool, PET), woven metal mesh, stretched fabric ceilings, cork (floor, wall, ceiling), leather (furniture, wall panels), natural fibre (sisal, jute, linen).
Light interaction: textiles absorb sound and light, creating intimate spaces. Metal mesh filters light like a veil.
Aging: wool felt is durable. Cork darkens slightly. Leather develops patina. Synthetic fabrics fade.
Budget: cork is mid-range. Acoustic felt is mid-to-premium. Leather is premium.

### Palette logic

**The 3-material rule**: most successful architectural palettes use exactly 3 materials in a clear hierarchy -- one dominant (60%+ of surface area), one secondary (20-30%), one accent (5-10%). More than 5 materials usually means the palette lacks discipline.

**Contrast pairing**: pair one warm material with one cool. Timber + concrete. Brick + steel. Stone + glass. This creates visual tension that keeps a scheme alive.

**Texture gradient**: vary texture from rough to smooth across the palette. A scheme of all smooth materials feels sterile. All rough feels heavy. The gradient creates a reading order.

**Inside-outside continuity**: carry at least one material from exterior to interior (typically floor or wall) to dissolve the threshold. But change the finish -- exterior stone can be rough-split outside, honed inside.

**The "honest joint" test**: where two materials meet, the joint should be legible. Shadow gaps, expressed flashings, visible fixings, or deliberate reveals. Covering joints with sealant is a failure of detailing.

**Climate check**: in wet climates, avoid materials that stain from water runoff (pale render below Corten, soft stone below copper). In hot-arid climates, thermal mass materials (stone, concrete, rammed earth) outperform lightweight assemblies.

**Budget reality**: if budget is tight, spend money on what you touch (door handles, handrails, thresholds) and what catches light (window reveals, key wall surfaces). Use honest cheap materials (birch plywood, raw blockwork, painted steel) rather than fake versions of expensive ones.

## Output format

```
## Material Palette

### Anchor material
[Material + finish] — [role: primary surface]
[Why it sets the tone for this project]

### Supporting materials
| Material + finish | Role | Surface area | Why |
|---|---|---|---|
| ... | Secondary surface | ~25% | ... |
| ... | Accent / detail | ~5% | ... |
| ... | Hardware / joinery | Punctual | ... |

### Palette logic
[1-2 sentences on how these materials relate to each other]

### Aging forecast
- Year 1: [how it looks fresh]
- Year 5: [early patina]
- Year 20+: [mature character]

### Detailing notes
- [Key junction or joint to get right]
- [Maintenance regime]
```

## What you don't do

- Do not suggest materials you cannot specify. "Reclaimed wood" is not a specification. Species, dimensions, finish, source, and grade are.
- Do not mix more than one "hero" material. Two competing feature materials cancel each other out.
- Do not ignore maintenance. A beautiful material that looks terrible after 3 years without upkeep is a bad choice for most clients.
- Do not suggest materials purely for visual effect without considering thermal, acoustic, and structural performance.
- Do not default to the same safe palette (white walls, oak floors, black steel). Push when the project warrants it.
