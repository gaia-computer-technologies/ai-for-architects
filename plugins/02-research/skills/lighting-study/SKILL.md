# /lighting-study

Analyse natural lighting conditions for a site or space based on orientation, latitude, season, and glazing strategy. Produce actionable guidance for design decisions about aperture placement, shading, and spatial experience.

## When to use

- Early design when establishing building orientation and section strategy
- Evaluating window placement and sizing for specific rooms
- Understanding how a space will feel at different times of day and year
- Preparing a daylight argument for a planning submission or design review
- Selecting glazing strategies (clerestory, light shelf, rooflight) for a given condition

## Input

- Site latitude and longitude (or city name)
- Building orientation (which facade faces which direction)
- Room dimensions and ceiling height
- Intended use (the daylight needs of a studio differ from a bedroom)
- Surrounding obstructions (neighbouring buildings, trees, topography)
- Climate type (overcast-dominant, clear-sky-dominant, mixed)

## Process

1. Establish the solar geometry for the site: sun path, altitude angles at solstice and equinox, prevailing sky conditions.
2. Map light availability to each facade and roof surface across the year.
3. Identify the primary daylight strategy for each key space based on orientation and use.
4. Recommend aperture types, positions, and control strategies.
5. Note critical times: when glare risk is highest, when supplementary lighting is needed, when solar gain must be managed.
6. Reference relevant precedent projects that solved similar lighting conditions.

## Domain knowledge

### Sun path fundamentals

The sun's path across the sky is determined by latitude and time of year. Two angles matter:

**Solar altitude**: the angle of the sun above the horizon.
- At the equator on equinox: 90 degrees at noon (directly overhead).
- At 52 degrees N (London) on summer solstice: ~62 degrees at noon.
- At 52 degrees N on winter solstice: ~15 degrees at noon. This is very low -- light penetrates deep into south-facing rooms but hits north-facing facades almost horizontally.
- At 40 degrees N (New York, Madrid) on winter solstice: ~27 degrees.
- At 35 degrees S (Sydney, Buenos Aires) on winter solstice (June): ~32 degrees.

**Solar azimuth**: the compass direction of the sun.
- Rises approximately east, sets approximately west (varies by latitude and season).
- At high latitudes in summer, the sun rises north of east and sets north of west (northern hemisphere) -- this means north-facing facades get direct light in early morning and late evening in summer.

### Light quality by orientation

**South-facing (northern hemisphere) / North-facing (southern hemisphere)**
The "solar facade." Receives direct sunlight for most of the day in winter and midday in summer. Best for living spaces that benefit from warmth and changing light. Requires shading strategy for summer: external louvres, deep reveals, overhangs, deciduous planting.

Rule of thumb for overhang depth: an overhang equal to the window height will shade a south-facing window from sun above ~63 degrees -- approximately right for summer noon at 50 degrees N.

**North-facing (NH) / South-facing (SH)**
Even, diffuse, consistent light all year. No direct sun except brief morning/evening in high summer. The preferred orientation for studios, galleries, and workspaces where colour accuracy and even illumination matter. Light is cool in colour temperature. Spaces need compensating warmth from materials.

**East-facing**
Strong morning sun, low angle, deep penetration. Warm colour temperature. Good for bedrooms (natural wake cycle), breakfast rooms, and morning-use spaces. Risk: low-angle glare is hard to control with fixed shading. Use internal blinds or deep reveals.

**West-facing**
Intense afternoon and evening sun. Highest solar gain and glare risk because it coincides with peak air temperature. Good for evening-use spaces if controlled. Problematic for offices and workspaces. Requires robust shading: external shutters, brise-soleil, or deep plan to attenuate.

### Golden hour and blue hour

**Golden hour**: the period when the sun is 0-6 degrees above the horizon. Light is warm (2500-3500K), directional, and raking. Occurs approximately 30-60 minutes after sunrise and before sunset. At high latitudes in summer, golden hour can last 2+ hours. In winter, the sun stays low enough that midday light has golden-hour quality.

**Blue hour**: the period when the sun is 0-6 degrees below the horizon (civil twilight). Ambient light is cool blue, even, shadowless. Interior spaces glow warm against a blue exterior. This is the moment when architecture is most photogenic.

### Glazing strategies

**Clerestory**: high-level windows that wash the ceiling with light and bounce it deep into the plan. Avoids glare at eye level. Excellent for single-storey buildings or top floors. Kahn used clerestories at the Kimbell (paired with reflective cycloid vaults) and the Salk Institute (lab buildings).

**Light shelf**: a horizontal reflective surface at or above head height that bounces light onto the ceiling and deeper into the room. The window is divided: view glass below the shelf, daylight glass above. Effective on south-facing facades. Increases useful daylight depth from ~2x window height to ~3-4x.

**Rooflight / skylight**: light from directly above. Most efficient daylight source (3x the illumination of a vertical window of the same area). Risk: solar gain and glare in summer. Use north-facing rooflights (sawtooth) or diffusing glass. Zumthor's Kunsthaus Bregenz uses a translucent glass ceiling that creates perfectly even zenithal light.

**Light well / atrium**: brings daylight into the deep plan of multi-storey buildings. Effectiveness depends on the well's aspect ratio (width-to-height). A tall, narrow light well delivers almost no useful light at ground level. A wide, shallow one works. White or reflective walls increase efficiency.

**Diffused / translucent**: channel glass (Profilit), polycarbonate, translucent stone, fabric. These materials admit light while eliminating view and reducing glare. Creates a soft, even glow. Renzo Piano's Menil Collection uses ferro-cement "leaves" to filter zenithal light.

**Slit / slot**: narrow vertical or horizontal openings that frame specific light conditions. Ando's Church of the Light: a cruciform slit in a concrete wall. Barragan's house: thin slots that catch only specific times of day. These are about controlled absence of light as much as its presence.

### How architects used light

**Tadao Ando**: light as the primary material. Concrete walls become screens for projected shadow and sun patterns. Church of the Light (1989) -- a cruciform slot in the altar wall fills with morning light. Minimal apertures make each light event intense.

**Louis Kahn**: "A room is not a room without natural light." The Kimbell Art Museum (1972) -- cycloid concrete vaults with continuous skylights, a perforated aluminium reflector splits incoming light into ambient (reflected off vault) and a sliver of direct. The Salk Institute (1965) -- east-west orientation, study towers face the Pacific, narrow slots between labs frame the sky.

**Luis Barragan**: coloured light. White light enters a space and bounces off an intensely coloured wall (hot pink, gold, violet), transforming the entire room. The light is the medium; the wall colour is the filter. Gilardi House (1976) -- a blue and red corridor leading to a pink dining room over a pool. Light and colour are inseparable from spatial experience.

**Peter Zumthor**: light as atmosphere. Therme Vals (1996) -- light enters through thin gaps between stone slabs, creating the impression of stone floating. Bruder Klaus Chapel (2007) -- light enters through an oculus and 350 small holes where formwork rods were removed. Light reveals the hand of making.

**Sverre Fehn**: light as narrative. Nordic Pavilion, Venice (1962) -- a double concrete beam ceiling that filters Venetian light into Scandinavian-quality diffuse illumination. Glacier Museum (1991) -- a long, dark concrete tunnel opening to a panoramic glacier view. Compression then release, dark then light.

### Daylight metrics

- **Daylight factor**: ratio of indoor illuminance to outdoor illuminance under overcast sky. 2% minimum for habitable rooms (UK Building Regs). 5%+ for studios and workspaces. Measured on the horizontal work plane.
- **Useful daylight illuminance (UDI)**: percentage of occupied hours when illuminance is between 100-3000 lux. Below 100 is too dark; above 3000 causes glare. Target: UDI 100-3000 for 50%+ of occupied hours.
- **Average daylight factor rule of thumb**: window area = 1/10 of floor area gives approximately 2% DF. 1/5 of floor area gives approximately 5% DF. Varies with glazing transmittance, room depth, and surface reflectance.

## Output format

```
## Lighting Study: [Project / Space Name]

### Solar context
- Latitude: [X] degrees [N/S]
- Solar altitude range: [winter solstice noon] to [summer solstice noon]
- Predominant sky type: [overcast / clear / mixed]
- Key solar events: [specific times and angles that matter]

### Facade-by-facade analysis
| Orientation | Light quality | Best use | Risk | Strategy |
|---|---|---|---|---|
| North | ... | ... | ... | ... |
| South | ... | ... | ... | ... |
| East | ... | ... | ... | ... |
| West | ... | ... | ... | ... |

### Recommended glazing strategies
- [Space]: [strategy] -- [reason]

### Daily light narrative
- Morning: [what happens]
- Midday: [what happens]
- Afternoon: [what happens]
- Evening: [golden hour / blue hour quality]

### Precedent references
- [Project, Architect] -- [relevant lighting strategy]
```

## What you don't do

- Do not provide precise lux calculations. This tool gives design-level guidance, not engineering simulation. For precise analysis, recommend Radiance, Ladybug/Honeybee, or Velux Daylight Visualizer.
- Do not ignore southern hemisphere reversal. South-facing in Sydney is the cold, diffuse facade. Always check which hemisphere you're in.
- Do not recommend glazing strategies without considering thermal consequences. A fully glazed south facade is a solar oven in summer. Light and heat are the same energy.
- Do not treat all daylight as good. Glare, overheating, and UV damage to furnishings are real problems. Control is as important as admission.
- Do not forget artificial lighting. Natural light strategy must be designed together with the electric lighting scheme -- they are not separate systems.
