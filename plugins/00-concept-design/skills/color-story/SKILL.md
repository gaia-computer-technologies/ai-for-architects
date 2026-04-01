# /color-story

Derive an architectural colour palette from project context -- site, orientation, materials, cultural references, and spatial intent. Output usable colour specifications, not abstract mood.

## When to use

- Selecting render, plaster, paint, or tile colours for a project
- Translating a client's colour language ("warm but not beige", "moody not dark") into specifications
- Ensuring colour choices work with the material palette and lighting conditions
- Building a colour board for a presentation or planning submission

## Input

One or more of:
- Site location and orientation (affects light quality)
- Material palette (colours must work with material tones)
- Architectural style or references
- Client colour preferences or aversions
- Building type and intended atmosphere
- Latitude and predominant sky condition (overcast, bright, high-altitude)

## Process

1. Establish the light context: latitude, orientation, sky type. This determines how colours will actually read in the space.
2. Identify the material-inherent colours (stone tone, timber warmth, concrete grey) -- these are non-negotiable parts of the palette.
3. Select applied colours (paint, render, tile) that complement material tones rather than competing with them.
4. Test each colour against orientation: north-facing rooms eat warm colours; south-facing rooms can handle cool tones.
5. Build a hierarchy: dominant field colour, secondary accent, trim/detail colour.
6. Output in multiple notation systems for different use cases.

## Domain knowledge

### Light quality and colour perception

Colour does not exist without light. The same paint looks different on every wall of a room.

**Northern hemisphere, north-facing spaces**: cool, even, blue-shifted light all day. Warm colours (ochre, terracotta, blush) counterbalance effectively. Cool whites look clinical here. Use NCS whites with yellow or red undertones (e.g., NCS S 0502-Y, NCS S 0505-Y80R).

**Southern hemisphere, south-facing spaces**: same cool light conditions apply -- inverted hemisphere, same logic.

**East-facing spaces**: warm morning light, cool afternoon shadow. Neutral palettes work well because the light does the work. Avoid strong warm colours that overheat visually at sunrise.

**West-facing spaces**: intense warm light in the afternoon. Cool-toned walls (blue-grey, green-grey, sage) balance the golden hour. Strong warm colours become overwhelming at 5pm.

**Overcast climates (UK, Scandinavia, Pacific NW)**: diffuse light flattens colour. You can use stronger, more saturated tones than you think -- they need the extra push to read. Pale colours go flat and dead under overcast skies.

**High-altitude / Mediterranean**: intense, direct light bleaches saturated colour. Earth tones, white, and deep shadows work because the light itself provides the drama. Barragan's intense pinks and purples only work because Mexican light is strong enough to sustain them.

### The NCS system

Natural Colour System is the architect's colour language. Unlike Pantone (print) or RAL (industrial), NCS describes how humans perceive colour.

NCS notation: `S [blackness][chromaticness]-[hue]`
- S 1005-Y20R = 10% blackness, 05% chromaticness, hue between yellow and red (a warm off-white)
- S 8010-B30G = 80% blackness, 10% chromaticness, blue-green (a very dark teal)

Rules of thumb:
- Blackness below 10 = light/white family
- Chromaticness below 10 = near-neutral
- Architectural palettes typically stay below 20% chromaticness for walls. Higher saturation is for accents only.
- A 2% chromaticness difference is visible at large scale. Small samples mislead -- always test at full wall area.

### Material-colour relationships

- **Fair-faced concrete**: reads as NCS S 2502-Y (warm grey) to S 3502-B (cool grey) depending on aggregate and formwork. Pair with muted, desaturated applied colours.
- **Natural oak**: warm yellow-brown, approximately NCS S 2020-Y20R. Pair with cool greys, blue-greens, or warm whites. Avoid competing yellows.
- **Red brick**: NCS S 4040-Y70R range. Pair with deep greens (complementary), cream whites, charcoal. Never orange accents.
- **White marble/limestone**: cool white with subtle warmth. Let it be the lightest element. Pair with mid-tone accents, never bright white paint that out-whites the stone.
- **Corten steel**: deep orange-brown, S 5040-Y60R. Pair with charcoal, dark green, concrete grey. Avoid warm neutrals that compete.

### Trending architectural palettes (2024-2026)

**Warm minimalism**: off-whites with yellow undertone (S 0505-Y20R), pale plaster pinks (S 0510-Y90R), oatmeal (S 1005-Y30R). Materials do the work; applied colour is nearly absent. Risk: everything looks like the same Instagram apartment.

**Dark japandi**: charcoal plaster (S 7005-B20G), shou sugi ban black, ink blue (S 7020-B), with natural timber relief. Deep, quiet, contemplative. Risk: oppressive without enough light or contrast.

**Opera / maximalist**: deep burgundy (S 5030-R), forest green (S 6020-B90G), brass accents. Colour as spatial event. Risk: looks like a bar if the proportions aren't generous.

**Nordic muted**: grey-greens (S 2005-G20Y), dusty blue (S 2010-B), warm grey (S 2005-Y50R). Designed for overcast light. Risk: can feel institutional without texture.

**Earthen / biophilic**: terracotta (S 3030-Y60R), sage (S 3010-G30Y), clay (S 2020-Y30R), raw umber. Derived from unprocessed material tones. Risk: muddy without a light or crisp element.

### Colour proportion rule

The 60-30-10 rule works for architecture as well as it does for graphic design:
- 60% dominant field colour (walls, ceiling -- usually the lightest, most neutral)
- 30% secondary colour (floor, large furniture, one feature wall)
- 10% accent (door frames, joinery detail, a single wall, hardware)

Breaking this rule requires confidence. Barragan broke it constantly. You are probably not Barragan.

## Output format

```
## Colour Story: [Project Name]

### Light context
[Latitude, orientation, sky type, and what that means for colour perception]

### Palette

| Role | Colour name | Hex | NCS | Application |
|---|---|---|---|---|
| Field / dominant | ... | #... | S ...  | Walls, ceiling |
| Secondary | ... | #... | S ... | [Specific surface] |
| Accent | ... | #... | S ... | [Specific element] |
| Trim / detail | ... | #... | S ... | [Joinery, frames] |

### Material-colour integration
[How applied colours relate to the inherent material tones in the palette]

### Orientation notes
- North-facing rooms: [adjustment if needed]
- South-facing rooms: [adjustment if needed]

### Sample testing guidance
[Recommended sample size, which walls to test on, time of day to evaluate]
```

## What you don't do

- Do not specify colour from small digital swatches. Always recommend physical samples at minimum A3 size, viewed in the actual space.
- Do not ignore the undertone. "White" is not a colour -- it's a family of hundreds of colours. Specify which white.
- Do not use hex codes as the primary specification for built work. Hex is for screens. NCS or manufacturer references are for walls.
- Do not apply trending palettes without checking them against the project's light conditions. Dark japandi in a basement flat is a cave.
- Do not treat colour as decoration applied after the architecture. Colour is part of the spatial experience from day one.
