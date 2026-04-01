# /moodboard-prompt

Structure a mood board from loose inspiration into a coherent visual brief. Bridge the gap between client language ("I like this feeling") and architectural specification.

## When to use

- A client sends a folder of Pinterest images and you need to extract the actual design direction
- Starting a project and needing to align the team on visual and spatial intent before design begins
- Preparing a mood board for a presentation that communicates more than "we like nice things"
- Translating verbal descriptions ("warm but modern", "industrial but refined") into structured visual categories

## Input

- Client inspiration images, links, or verbal descriptions
- Project type and brief summary
- Material and style direction (if established)
- Any constraints: budget, planning context, existing building character
- Target audience for the mood board (internal team, client, contractor)

## Process

1. Sort all input into the five mood board categories below. Identify which categories are covered and which are missing.
2. Decode the client's language: what do they actually mean? "Modern" might mean minimalist, might mean contemporary, might mean "not traditional." "Warm" almost always means natural materials and indirect light, not a colour temperature.
3. Identify the common thread across their references. Usually it's a light quality, a material logic, or a spatial proportion -- not a style.
4. Fill gaps: if they've only sent interior images, you need exterior and detail references. If they've only sent materials, you need spatial references.
5. Structure the mood board with clear hierarchy and grouping. Label each image with what it's referencing (material, light, proportion, colour, detail -- not just "inspiration").
6. Write image-sourcing prompts for any gaps that need to be filled.

## Domain knowledge

### Mood board anatomy

A useful architectural mood board has five categories. Missing any of them leaves the design direction incomplete.

**1. Spatial references (the most important, most often missing)**
Images that show volumes, proportions, and light quality rather than decoration. These are the images that describe what it feels like to stand in the space. Wide-angle photographs of rooms, sections, or models that communicate height, depth, compression, openness. Clients rarely pin these -- they pin materials and finishes. You need to supply the spatial layer.

**2. Material close-ups**
Tight crops showing texture, grain, joint detail, weathering. These communicate haptic quality. A piece of timber shows species, finish, and age. A concrete sample shows aggregate, formwork pattern, and colour. Never use manufacturer product shots -- they flatten material character. Use photographs of materials in built context, ideally weathered.

**3. Detail shots**
Junctions, thresholds, window reveals, handrails, door handles, stair nosings. These communicate the level of craft and the tectonic language. A shadow gap between wall and ceiling. A flush door with a concealed frame. A steel handrail welded to a flat plate. Details are where the design lives or dies. They also communicate budget: expressed steel connections say something different from painted plasterboard returns.

**4. Atmospheric / contextual images**
Landscape, light conditions, seasonal character, urban context. These ground the mood board in place. A photograph of morning mist in the valley where the site sits. The colour of the local stone in afternoon light. The street rhythm of neighbouring buildings. These images prevent the mood board from being a generic aspiration board -- they anchor it to this project, this site.

**5. Colour and finish swatches**
Flat colour references, paint samples on textured surfaces, tonal compositions. These should be derived from the material and atmospheric images, not selected independently. Pull the colour story from what's already on the board. A lime-washed wall in southern light. The patina on a copper gutter. The specific green of moss on local stone.

### Translating client language

Clients describe what they want using non-architectural language. This is not a problem to correct -- it's a translation task.

| Client says | They usually mean | Architectural translation |
|---|---|---|
| "Modern" | Not traditional. Clean lines. No ornament. | Minimalist or contemporary. Clarify with follow-up. |
| "Warm" | Natural materials, soft light, not clinical | Timber, indirect lighting, textured surfaces, contained proportions |
| "Industrial" | Exposed structure, raw materials, loft-like | Fair-faced concrete or steel, expressed services, open plan, high ceilings |
| "Cosy" | Small scale, enclosure, soft materials | Low ceilings, alcoves, warm materials, layered lighting |
| "Light and airy" | Lots of glazing, white walls, visual space | Open plan, large windows, reflective surfaces, high ceilings. Caution: they may not want the thermal consequences. |
| "Timeless" | Won't date in 5 years | Natural materials, restrained palette, avoid trend-driven finishes |
| "Scandinavian" | Light timber, white walls, simple forms | Specific: which Scandinavia? Danish warmth or Finnish austerity? Aalto or Jacobsen? |
| "Japanese" | Minimal, natural, serene | Ma (spatial pause), natural materials, filtered light, connection to garden. Often what they want is wabi-sabi -- imperfection and age. |
| "Grand" | Generous proportions, impressive | High ceilings, wide doorways, formal symmetry, quality materials. Not necessarily large. |
| "Boutique hotel" | Curated, intimate luxury | Considered lighting, rich materials at touch points, layered textures, attention to hardware |

### Grouping logic

Arrange the mood board to communicate relationships, not just collect images.

**By material thread**: group images that share a material language. All the timber references together, all the concrete together. This reveals whether the palette is coherent.

**By spatial quality**: group by the feeling. "Compression" images together (low ceilings, narrow passages). "Release" images together (double heights, panoramic views). This builds an experiential narrative.

**By scale**: move from landscape (context) to building (form) to room (space) to detail (craft). This zoom sequence helps clients understand how the big picture connects to the small decisions.

**What to exclude**: remove any image that contradicts the emerging direction, even if the client loves it. A mood board with contradictory references is not a direction -- it's a mood swamp. If the client insists on keeping conflicting references, surface the conflict explicitly: "These two images suggest different material languages. Which feels more like your project?"

### Common mood board failures

- **The Pinterest dump**: 40 images with no hierarchy or grouping. This communicates nothing except "I like nice things." Curate to 12-20 images maximum.
- **All interiors, no architecture**: mood boards that could apply to any building because they only show furniture and finishes. Insist on spatial and exterior references.
- **Style without substance**: beautiful images that don't connect to the actual project's budget, site, or programme. Every image should be defensible: "This is relevant because..."
- **Missing the detail layer**: grand spatial images but no close-ups. The detail layer is where budget reality meets design ambition. Include it.

## Output format

```
## Mood Board Brief: [Project Name]

### Design direction summary
[2-3 sentences distilling the common thread across all references]

### Board structure

#### Spatial references
- [Description of needed image + what it communicates]
- [Search terms or specific project reference]

#### Material close-ups
- [Material + finish + what to show]
- [Specific project or photographer reference if possible]

#### Detail shots
- [Junction/element type + quality level]

#### Atmosphere / context
- [Light condition, landscape, seasonal quality]
- [Site-specific references]

#### Colour / finish
- [Derived from above -- specific tones and finishes to swatch]

### Client language decoded
[Translation of their verbal brief into architectural terms]

### Contradictions to resolve
- [Any conflicting directions in the input that need a decision]

### Image sourcing notes
[Specific photographers, publications, or projects to search for reference images: Archdaily, Divisare, El Croquis, specific monographs]
```

## What you don't do

- Do not accept a mood board without spatial references. Materials and finishes without spatial intent produce interior design, not architecture.
- Do not include more than 20 images. Curation is the skill. If everything is inspiration, nothing is direction.
- Do not use stock photography or renders as mood board content. Use photographs of built work. Renders lie about light and material.
- Do not let contradictions pass without flagging them. A mood board that points in two directions is worse than no mood board.
- Do not present the mood board as final design intent. It is a starting point for conversation, not a specification. Make this explicit to the client.
