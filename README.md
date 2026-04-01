# AI for Architects

Open-source Claude Code skills for the concept phase of architecture.

**5 skills. 1 agent. 1 plugin.** Built by [Gaia](https://gaia.computer) — the AI that learns your design sense.

---

## What this is

Five focused skills for the earliest decisions in architecture — the ones that determine what gets built. Briefs, materials, renders, narratives, atmosphere.

These skills operate **upstream** — before BIM, before production drawings, before specifications. The concept phase is where the most consequential design decisions happen.

## Skills

| Skill | Command | What it does |
|---|---|---|
| Render Prompt | `/render-prompt` | Craft optimised prompts for AI architectural renders — style, materials, lighting, camera, mood |
| Design Brief | `/design-brief` | Generate structured design briefs from conversations or loose notes |
| Material Palette | `/material-palette` | Suggest cohesive material and finish palettes for a design concept |
| Concept Narrative | `/concept-narrative` | Write the design rationale for presentations — atmosphere, experience, intention |
| Space Feel | `/space-feel` | Describe experiential qualities — compression, prospect, threshold, atmosphere |

### Agent

**Concept Architect** — orchestrates all five skills. Guides conversations from vague idea to presentation-ready output. Knows when to invoke each skill and when to stop.

## Install

```bash
# Claude Code
claude plugin marketplace add gaia-computer-technologies/ai-for-architects
claude plugin install concept-design@ai-for-architects
```

Or in Claude Desktop: Settings → Plugins → Add marketplace from GitHub → `gaia-computer-technologies/ai-for-architects`

## Community

This is part of a growing ecosystem of open-source architecture skills for Claude.

For the rest of the project lifecycle — due diligence, zoning analysis, programming, specifications, sustainability, and procurement — see [Architecture Studio](https://github.com/AlpacaLabsLLC/skills-for-architects) by [ALPA](https://alpa.llc) (Federico Negro). 36 skills, 7 agents, real domain depth. Their work inspired us to contribute our piece.

We focus on the concept phase. They cover the full AEC lifecycle. The two are complementary.

Architecture needs more open tools. We are all doing this together.

## Philosophy

These skills are built on a specific belief: **the concept phase is where architecture happens.**

70% of rework traces to design errors made before anyone opens a BIM tool. The decisions that matter most — what the space feels like, what it's made of, how light enters, what story it tells — happen in the first hours of a project.

We believe in workflows over wrappers, memory over prompts, and design intelligence that accumulates across projects. These open-source skills are a small piece of that vision — the part we can share freely. For the full experience, see [Gaia Studio](https://gaia.computer).

## License

MIT — [Hermetica Tech B.V.](https://gaia.computer)
