# /render-prompt

Craft an optimised architectural render prompt from a design description.

## When to use

When an architect, designer, or homeowner needs to generate a photorealistic architectural render using any AI image model (Gaia Studio, Midjourney, DALL-E, Stable Diffusion, Flux). The skill translates loose design intent into precise, structured prompts that produce publication-quality results.

## Input

The user provides a design description. This can be:
- A single sentence: "minimalist concrete house, golden hour"
- A detailed brief: room type, style, materials, mood, time of day
- A reference to a style movement: "Tadao Ando meets Scandinavian warmth"
- An existing render they want to iterate on

## Process

1. **Parse the intent.** Identify: building/room type, style, dominant materials, lighting condition, camera perspective, mood.

2. **Fill gaps with informed defaults.** If the user says "modern kitchen" but doesn't specify lighting, default to soft north-facing daylight — the most flattering for kitchens. Always choose the option that an experienced architectural photographer would choose.

3. **Structure the prompt** using this hierarchy (most to least important for image models):
   - **Subject**: what is being rendered (room type, building type, scale)
   - **Style**: architectural movement or aesthetic direction
   - **Materials**: specific materials, not generic ("white-washed Douglas fir ceiling" not "wood ceiling")
   - **Lighting**: time of day, direction, quality (diffused, raking, golden)
   - **Camera**: eye level, bird's eye, worm's eye, focal length equivalent
   - **Atmosphere**: mood, season, weather, human presence
   - **Technical**: resolution, aspect ratio, rendering style (photorealistic, watercolour, section)

4. **Output the prompt** in two formats:
   - **Full prompt**: detailed, comma-separated, ready to paste
   - **Negative prompt**: what to exclude (distortion, oversaturation, unrealistic scale)

## Domain knowledge

### Lighting conditions by space type
- **Living rooms**: late afternoon west light, warm, long shadows. Or: overcast north light for Scandinavian interiors.
- **Kitchens**: morning east light or soft north light. Avoid direct overhead — it kills material texture.
- **Bathrooms**: soft diffused light, steam atmosphere. Dawn or dusk.
- **Exteriors**: golden hour (low sun, warm) or blue hour (dusk, moody). Midday flattens facades.
- **Bedrooms**: early morning, curtains filtering light. Intimate, not staged.

### Camera perspectives
- **Eye level (1.2m)**: most natural, residential feel. Default for interiors.
- **Seated level (0.9m)**: living rooms, restaurants. Creates intimacy.
- **Elevated (2.5m)**: shows spatial layout. Good for open plans.
- **Worm's eye (0.3m)**: dramatic, emphasises ceiling and volume. Use for double-height spaces.
- **Bird's eye**: aerial exterior views. Requires explicit request.

### Material specificity
Never use generic material names. Translate:
- "wood" → "white oak with matte finish" or "charred Yakisugi cedar" or "reclaimed Douglas fir"
- "stone" → "honed Ceppo di Gré limestone" or "bush-hammered Vals quartzite"
- "concrete" → "board-formed concrete with vertical grain" or "polished microcement in warm grey"
- "metal" → "patinated brass hardware" or "blackened steel window frames" or "brushed stainless"
- "tile" → "Moroccan zellige in sea foam" or "matte white subway with dark grout"

### Style shorthands
When the user references a style, expand it:
- **Japandi**: low furniture, natural materials (oak, linen, stone), muted earth palette, negative space, handmade ceramics
- **Brutalist**: raw concrete, dramatic volumes, angular geometry, raking light, minimal furniture
- **Warm Minimalism**: travertine, bouclé, matte plaster, coffee/mocha palette, soft curves
- **Scandinavian Modern**: light wood (ash, birch), white walls, wool textiles, functional furniture, north light
- **Mediterranean Modern**: lime wash walls, terracotta, olive wood, linen, outdoor-indoor continuity
- **Mid-Century Modern**: walnut, brass, terrazzo, statement lighting, low-slung furniture, warm tones

## Output format

```
RENDER PROMPT
─────────────
[Full structured prompt, 40-80 words, comma-separated]

NEGATIVE PROMPT
───────────────
[What to exclude, 10-20 words]

PARAMETERS
──────────
Aspect ratio: [e.g. 16:9, 3:2, 4:5]
Best suited for: [which AI model/tool handles this style best]
```

## What you don't do

- Don't generate the image. You craft the prompt.
- Don't suggest styles the user didn't ask for unless filling a clear gap.
- Don't use "beautiful" or "stunning" — these are noise words in image prompts. Be specific.
- Don't output more than one prompt unless the user asks for variations.
