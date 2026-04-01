# AI for Architects

Open-source Claude Code skills for the concept phase of architecture.

**12 skills. 3 agents. 3 plugins.** Built by [Gaia](https://gaia.computer) — the AI that learns your design sense.

---

## What this is

A library of Claude Code skills purpose-built for architectural concept design. Each skill encodes domain knowledge about design briefs, material palettes, render prompts, lighting, precedent research, and presentation narratives.

These skills operate **upstream** — before BIM, before production drawings, before specifications. The concept phase is where the most consequential design decisions happen. This is where we focus.

## What this is not

This is not a BIM plugin, a code compliance checker, or a specifications writer. For those, see [Architecture Studio by ALPA](https://github.com/AlpacaLabsLLC/skills-for-architects) — an excellent open-source skill library covering due diligence, zoning analysis, programming, specifications, sustainability, and FF&E procurement. Their work inspired this project and we recommend it alongside ours.

## Skills

### Plugin 00 — Concept Design (6 skills)

| Skill | Command | What it does |
|---|---|---|
| Render Prompt | `/render-prompt` | Craft optimised prompts for AI architectural renders — style, materials, lighting, camera, mood |
| Design Brief | `/design-brief` | Generate a structured brief from conversation or loose notes — programme, materials, design intent |
| Style Analysis | `/style-analysis` | Identify and articulate architectural style — movement, era, key elements, related precedents |
| Material Palette | `/material-palette` | Suggest cohesive material and finish palettes considering context, lighting, budget, design language |
| Color Story | `/color-story` | Derive architectural colour palettes from spatial context — hex codes, NCS references, application guidance |
| Room Programme | `/room-programme` | Generate spatial programmes — rooms, areas, adjacency, circulation. Structured table output |

### Plugin 01 — Presentation (3 skills)

| Skill | Command | What it does |
|---|---|---|
| Concept Narrative | `/concept-narrative` | Write the design rationale for presentations — atmosphere, experience, intention |
| Space Feel | `/space-feel` | Describe experiential qualities — scale, compression, threshold, prospect, refuge |
| Moodboard Prompt | `/moodboard-prompt` | Structure mood boards from loose inspiration — grouped by material, atmosphere, scale, detail |

### Plugin 02 — Research (3 skills)

| Skill | Command | What it does |
|---|---|---|
| Lighting Study | `/lighting-study` | Analyse natural lighting from orientation, latitude, time of year — sun angles, shadows, glazing |
| Precedent Research | `/precedent-research` | Find architectural precedents matching a design direction — projects, strategies, relevance |
| Design Critique | `/design-critique` | Structured feedback on concept designs — coherence, material logic, light, programme fit |

### Agents

| Agent | What it orchestrates |
|---|---|
| Concept Architect | Full concept phase: brief → style → materials → render prompts → narrative |
| Design Critic | Reviews presentations for spatial coherence, material logic, narrative clarity |
| Client Translator | Turns vague client language into precise design parameters |

## Install

### Claude Code

```bash
claude plugin marketplace add gaia-computer-technologies/ai-for-architects
claude plugin install concept-design@ai-for-architects
claude plugin install presentation@ai-for-architects
claude plugin install research@ai-for-architects
```

### Claude Desktop

1. Open Settings → Plugins → Add plugin
2. Select "Add marketplace from GitHub"
3. Enter `gaia-computer-technologies/ai-for-architects`
4. Install the plugins you need

## Philosophy

These skills are built on a specific belief: **the concept phase is where architecture happens.**

a16z recently confirmed what architects already know — the $13T AEC industry runs on software designed in 1997. 70% of rework traces to design errors in the concept phase. The tools that matter most are the ones that help you think before you draw.

We focus on workflows, not wrappers. On memory, not prompts. On the design intelligence that accumulates across projects — what we call *taste memory*.

These open-source skills are a small piece of that vision. For the full experience — photorealistic renders from sketches, interior transformations, design intelligence that learns your sense across sessions — see [Gaia Studio](https://gaia.computer).

## Credits

Inspired by [Architecture Studio](https://github.com/AlpacaLabsLLC/skills-for-architects) by ALPA (Federico Negro). Their work covers the full AEC lifecycle — due diligence, zoning, programming, specifications, sustainability, procurement. We operate upstream at the concept phase. The two libraries are complementary.

## License

MIT
