# /style-analysis

Identify the architectural style(s) present in a project description, reference set, or keyword list. Return a structured analysis with lineage, key characteristics, and design implications.

## When to use

- A client describes a vibe but not a style ("raw concrete, lots of light, Japanese-feeling")
- You need to classify an existing building or reference image set
- Bridging between a mood board and a design language
- Establishing stylistic coherence across a project team

## Input

One or more of:
- Free-text project description or client brief excerpt
- List of reference architects or buildings
- Keywords describing desired spatial or material qualities
- An existing design that needs stylistic classification

## Process

1. Extract style signals from input: materials mentioned, spatial qualities, formal language, historical references, geographic context.
2. Match against the style taxonomy below. Most projects map to 1-2 primary styles and often a regional inflection.
3. Identify tensions or contradictions (e.g., "minimalist but warm" signals a specific sub-genre, not a conflict).
4. Return primary style(s) with confidence, secondary influences, and actionable design implications.
5. Flag when the input genuinely doesn't map to a single movement -- hybrid positions are legitimate.

## Domain knowledge

### Major architectural movements

**Modernism (1920s-1960s)**
Key figures: Le Corbusier, Mies van der Rohe, Gropius, Aalto, Neutra.
Materials: reinforced concrete, steel frame, plate glass, white render.
Spatial qualities: free plan, pilotis, horizontal ribbon windows, roof terraces. Separation of structure from enclosure. Machine-age optimism.
Formal language: orthogonal geometry, structural expression, transparency.

**Brutalism (1950s-1975)**
Key figures: Corbusier (late), the Smithsons, Banham, Kenzo Tange, Moshe Safdie.
Materials: beton brut (board-marked concrete), exposed aggregate, raw steel.
Spatial qualities: heavy mass, deep reveals, monumental scale, expressed circulation. Streets-in-the-sky, megastructural ambition.
Formal language: sculptural concrete forms, repetitive cellular units, heroic geometry.

**Postmodernism (1966-1990s)**
Key figures: Venturi, Charles Moore, Graves, Rossi, Bofill, early Gehry.
Materials: coloured render, stone cladding, decorative metalwork, classical fragments.
Spatial qualities: symbolic space, layered facades, ironic quotation, figural rooms.
Formal language: historical reference, polychromy, collage, wit, ornament as communication.

**Deconstructivism (1988-present)**
Key figures: Gehry, Libeskind, Hadid, Coop Himmelb(l)au, Tschumi, Eisenman.
Materials: titanium cladding, steel plate, folded metal, irregular glazing.
Spatial qualities: destabilized geometry, fractured plans, vertiginous voids, spatial disorientation as experience.
Formal language: angular collisions, non-orthogonal, exploded volumes, anti-gravity.

**Parametricism (2008-present)**
Key figures: Schumacher (coined term), Hadid/ZHA studio, NBBJ, Bjarke Ingels (adjacent).
Materials: GFRC, ETFE, CNC-milled timber, 3D-printed concrete, algorithmic tessellation.
Spatial qualities: continuous surfaces, gradient transitions, field conditions rather than discrete objects.
Formal language: ruled surfaces, voronoi patterns, topology optimization, computational form-finding.

**Critical Regionalism (1983-present)**
Key figures: Frampton (theorist), Tadao Ando, Glenn Murcutt, Studio Mumbai, Balkrishna Doshi, Geoffrey Bawa.
Materials: local stone, regional timber species, handmade brick, rammed earth, context-specific.
Spatial qualities: grounded in site and climate, tactile materiality, filtered light, cross-ventilation as spatial strategy.
Formal language: modern syntax with vernacular inflection, tectonic clarity, landscape integration.

**Minimalism (1990s-present)**
Key figures: John Pawson, Claudio Silvestrin, Alberto Campo Baeza, SANAA, David Chipperfield.
Materials: white plaster, pale stone (Jura, Pietra Serena), oiled oak, frameless glass, matte metals.
Spatial qualities: reductive, silence, proportion as primary tool, empty space as positive element.
Formal language: planar, monolithic, precise detailing that disappears, shadow gaps over joints.

**High-Tech (1970s-present)**
Key figures: Rogers, Piano, Foster, Hopkins, Grimshaw.
Materials: structural steel (expressed), glass curtain wall, tension cables, aluminium cladding.
Spatial qualities: long spans, flexible floorplates, visible servicing, celebrated structure.
Formal language: engineered elegance, mast-and-cable, exoskeleton, industrial aesthetic.

**Metabolism (1960s-1970s)**
Key figures: Kenzo Tange, Kisho Kurokawa, Fumihiko Maki, Arata Isozaki (early).
Materials: prefab concrete capsules, steel megaframes, modular plug-in units.
Spatial qualities: megastructural cores with attachable living units, infrastructure as architecture.
Formal language: cellular repetition, organic growth metaphors, utopian urbanism.

**New Brutalism / Neo-Brutalism (2010s-present)**
Key figures: 6a Architects, Assemble, Carmody Groarke, Bruther, OFFICE KGDVS.
Materials: fair-faced concrete, raw steel, Douglas fir plywood, unfinished surfaces.
Spatial qualities: honest construction, spatial generosity, industrial loft quality, unfinished aesthetic as deliberate choice.
Formal language: stripped back, big moves over fine detail, warehouse scale domesticated.

### Style detection heuristics

- "Warm minimalism" = Minimalism + Critical Regionalism (Pawson meets Studio Mumbai)
- "Industrial chic" = High-Tech lineage filtered through loft conversion culture
- "Japanese modern" = Minimalism + specific spatial concepts (ma, wabi-sabi, engawa)
- "Organic modern" = Late Aalto lineage, now Kengo Kuma, sometimes Parametricism-lite
- "Dark academia" = Postmodern nostalgia filtered through interior design, not a real movement

## Output format

```
## Style Analysis

### Primary style
[Movement name] — [confidence: high/medium/low]
[2-3 sentence summary of why this classification fits]

### Secondary influences
- [Movement] — [specific aspect detected]

### Design implications
- Materials: [what this style implies for material selection]
- Spatial organisation: [plan and section strategies]
- Detailing: [level of finish, joint expression, hardware]
- Risk: [common failure modes when this style is done poorly]

### Key precedents
- [Building, Architect, Year] — [why it's relevant]
```

## What you don't do

- Do not force a single style label onto genuinely hybrid work. Name the hybrid.
- Do not treat style as purely visual -- always connect to spatial, material, and tectonic logic.
- Do not use "contemporary" as a style. It means nothing. Identify what is actually happening.
- Do not conflate interior design trends (cottagecore, dark academia) with architectural movements. Translate client language into architectural terms instead.
- Do not rank styles. Brutalism is not "worse" than Minimalism. Each has internal criteria for excellence.
