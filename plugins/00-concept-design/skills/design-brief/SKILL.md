# /design-brief

Generate a structured design brief from a conversation or loose notes.

## When to use

When an architect or designer needs to formalise design intent — from a client conversation, a set of references, a site visit, or their own sketched notes. The brief becomes the project's north star: what gets built starts here.

## Input

The user provides raw input in any form:
- A transcript or notes from a client meeting
- A list of rooms and requirements
- A mood description: "We want it to feel like a Japanese ryokan but in Brooklyn"
- A set of constraints: budget, site, timeline, programme
- An image or set of references (if image input is available)

## Process

1. **Extract core requirements.** Identify: programme (what rooms/spaces), site (if mentioned), budget tier, timeline, key constraints, aesthetic direction.

2. **Identify unstated assumptions.** If someone says "3-bedroom house" but doesn't mention storage, circulation, or outdoor space — note these as items to confirm, don't skip them.

3. **Organise into sections** following architectural brief convention:
   - Project overview (one paragraph)
   - Programme (spatial requirements table)
   - Site and context (if known)
   - Design intent and aesthetic direction
   - Material preferences
   - Sustainability and environmental goals
   - Budget and phasing
   - Open questions (what still needs resolving)

4. **Write in the architect's voice.** The brief should sound like an architect wrote it for their own team, not like a form was filled in. Direct, specific, opinionated where the client was clear, honest about gaps.

## Domain knowledge

### Programme defaults by project type

**Single-family residential (3-bed):**
- Living, dining, kitchen (often open plan): 45-65m²
- Primary bedroom with ensuite: 20-28m²
- Secondary bedrooms (x2): 12-16m² each
- Family bathroom: 6-8m²
- Entrance/circulation: 8-12m²
- Storage (often forgotten): 4-8m²
- Outdoor space: context-dependent
- Utility/laundry: 4-6m²
- Total: 130-180m² (typical, varies by market)

**Small office (10-20 people):**
- Open workspace: 5-8m² per person
- Meeting rooms: 1 per 6-8 people, 12-16m² each
- Focus/phone rooms: 1 per 10 people, 4m²
- Kitchen/break area: 15-25m²
- Reception: 10-15m²
- Storage/server: 6-10m²

**Restaurant (40-60 covers):**
- Dining area: 1.2-1.8m² per cover
- Kitchen: 30-40% of dining area
- Bar: 8-15m²
- WC (accessible + gendered or all-gender): 12-18m²
- Storage/staff: 10-15m²
- Outdoor dining: context-dependent

### Budget tier language
- **Modest**: standard materials, practical choices, value-engineered details
- **Mid-range**: good quality materials, some custom elements, considered details
- **High-end**: premium materials throughout, bespoke joinery, architectural hardware
- **Luxury**: no material constraints, fully custom, specialist craftspeople

### Sustainability defaults
If the user doesn't mention sustainability, include a section noting:
- Passive design strategies appropriate to climate
- Material longevity over novelty
- Energy performance targets (reference local standards)
- Note: "Sustainability goals to be confirmed with client"

## Output format

```
DESIGN BRIEF
═════════════

PROJECT OVERVIEW
[One paragraph summary: what, where, who, why]

PROGRAMME
┌──────────────────────┬────────┬──────────────────────────┐
│ Space                │ Area   │ Notes                    │
├──────────────────────┼────────┼──────────────────────────┤
│ [room]               │ [m²]   │ [adjacency, light, use]  │
└──────────────────────┴────────┴──────────────────────────┘
Total: [x] m² (approx.)

SITE & CONTEXT
[If known. Orientation, access, neighbours, constraints.]

DESIGN INTENT
[Aesthetic direction, spatial quality, references. 2-3 paragraphs.]

MATERIAL DIRECTION
[Specific materials where stated, general direction where implied.]

SUSTAINABILITY
[Environmental goals, passive strategies, certifications if targeted.]

BUDGET & PHASING
[Tier, total if stated, phasing approach if relevant.]

OPEN QUESTIONS
- [Items that need resolving before schematic design begins]
```

## What you don't do

- Don't invent requirements the client didn't mention. Flag gaps in "Open Questions".
- Don't use generic language: "a welcoming entrance" tells no one anything. Be specific about what welcoming means — material, scale, light, threshold.
- Don't include cost estimates unless the user provides budget data.
- Don't assume location-specific codes. Note "verify local requirements" where relevant.
