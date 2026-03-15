# New Age Glam Fantasy — AI Model Context

**Use this file as a system prompt or context injection for AI models** (ChatGPT, Claude, Gemini, local LLMs, etc.) to give them working knowledge of the style for prompt writing, critique, and art direction assistance.

---

## Style identity

**Name:** New Age Glam Fantasy
**Short tag:** NAGF
**Era anchor:** Late 1970s to mid-1980s (1978–1986)

**One-sentence definition:**
A retro-mystical visual style that merges late-1970s to mid-1980s metaphysical paperback illustration, glam fantasy cinema, soft-focus beauty imagery, prismatic pastel-neon color, and analog media decay into visions of cosmic transcendence.

**Canonical style lock line (always include at end of prompts):**
> Style: New Age Glam Fantasy — 1978–1986 metaphysical glam sci-fantasy, diffusion bloom/halation, prismatic pastels, VHS/CRT artifacts, analog film wear.

---

## The seven pillars (must be present)

1. **Mystical metaphysical imagery** — crystals, moons, portals, temples, auras
2. **Glamour language** — satin, jewelry, styled hair, makeup, iconic posing
3. **Soft optical diffusion** — halation, bloom, haze, dreamlike softness
4. **Prismatic color** — pink, lavender, cyan, pearl, rainbow refraction
5. **Analog wear** — VHS softness, CRT scanlines, chroma bleed, print fade
6. **Cosmic environments** — star fields, reflective water, aurora sky, crystal chambers
7. **Emotional transcendence** — initiation, enchantment, sacred glamour, visionary wonder

---

## Prompt construction order

1. Subject (oracle / priestess / queen + key visual traits)
2. Setting (crystal temple / moon garden / celestial desert + materials)
3. Motifs (crystals, mushrooms, moon disc, portals, butterflies — 2–4)
4. Styling (satin gown / silver jewelry / moon crown / chiffon veils)
5. Lighting (halo backlight / moonlit haze / candy aura spill / prism scatter)
6. Optics (diffusion bloom / halation / soft-focus / prismatic lens flare)
7. Palette (hot pink, violet, teal, aqua, lemon, pearl white, silver)
8. Analog artifacts (VHS softness / chroma bleed / CRT texture / print fade)
9. Emotional tone (sacred glamour / cosmic initiation / visionary serenity)
10. Format + style lock (paperback cover / film still / VHS frame + style line)

---

## Core color palette

Primary: hot pink (#FF1493), bubblegum pink (#FF69B4), lavender (#E6E6FA), orchid (#DA70D6), violet (#8B00FF), teal (#008080), aqua (#00FFFF), turquoise (#40E0D0), lemon yellow (#FFF44F)
Neutrals: pearl white (#F0EAD6), opal white (#F0F8FF), moon silver (#C0C0C0), reflective black (#0A0A0A)

---

## What this style IS

- Retro metaphysical glamour
- Cosmic priestess / oracle iconography
- Soft-focus dream memory aesthetic
- Spiritual paperback cover art language
- 80s glam fantasy cinema optics
- VHS/CRT analog texture layer
- Prismatic pastel-neon candy color system
- Ceremonial beauty as spiritual practice

---

## What this style IS NOT

- Cyberpunk / urban neon / tech noir
- Synthwave / outrun grids
- Vaporwave irony collage
- Dark occult / horror / gore
- Medieval battle fantasy
- Modern minimalist luxury editorial
- Generic "ethereal AI woman in stars"
- Aggressive glitch / datamosh art

---

## Negative prompt core (use to guard against drift)

```
cyberpunk, urban neon, city streets, dark occult, demonic, horror, blood, gore, medieval armor, swords, battle, hyperrealistic, ultra sharp, clean CGI, modern editorial, vaporwave irony, datamosh, harsh shadows, primary red, primary blue, earthy brown, industrial, dystopian
```

---

## Analog intensity levels

| Level | Description | When to use |
|-------|-------------|-------------|
| 1 | Light bloom, faint CRT, subtle softness | Elegant portraits, cleaner variants |
| 2 | Visible VHS blur, chroma bleed, scanlines | Most default work |
| 3 | Heavy tape blur, strong scanlines, signal noise | Explicit "lost VHS" pieces |

---

## Example prompt (medium complexity)

```
A radiant oracle with long wild pink curly hair standing in a mirrored crystal temple above reflective black water, surrounded by glowing mushrooms and crystal clusters, wearing an orchid satin gown with silver jewelry and chiffon veils, lit by halo backlight through lavender and teal mist, soft diffusion bloom, hot pink violet aqua and pearl palette, subtle VHS softness and chroma bleed, sacred glamour and cosmic initiation, composed as a lost metaphysical paperback cover. Style: New Age Glam Fantasy — 1978–1986 metaphysical glam sci-fantasy, diffusion bloom/halation, prismatic pastels, VHS/CRT artifacts, analog film wear.
```

---

## Key vocabulary

**Green flag words (reinforce the style):**
metaphysical, visionary, prismatic, opalescent, moonlit, mirrored, ceremonial, oracle, satin, veiled, luminous, diffusion, halation, crystal, aura, VHS-soft, faded print, cosmic glamour, sacred beauty, dream-memory

**Red flag words (may push away from style):**
cyberpunk, noir, tactical, dystopian, brutalist, hyperreal, ultra sharp, hard-edged, datamosh, industrial, streetwear, demonic, minimalist luxury, sterile futurism

---

## Repository structure

```
00_OVERVIEW/          Plain-language definition, FAQ, quick start
01_STYLE_FOUNDATIONS/ Core theory, aesthetic DNA, emotional logic, boundaries
02_VISUAL_COMPONENTS/ Color, light, optics, texture, artifacts
03_MOTIF_LIBRARY/     Symbolic motifs and recurring visual objects
04_COMPARATIVE_REFERENCE/ Adjacent styles, anti-references
05_PROMPT_ENGINEERING/ Prompt formulas, templates, troubleshooting
06_PRODUCTION_WORKFLOWS/ AI workflow, post-processing, VHS/CRT treatment
07_REFERENCE_GALLERY/ Curated breakdowns and case studies
08_TEMPLATES/         Reusable templates
09_SOURCES/           Bibliography and references
data/                 Machine-readable CSV, YAML, JSON files
```

---

## Machine-readable data

All structured data is in the `data/` directory:
- `data/color_palette.csv` — complete color system with hex and RGB
- `data/motifs.csv` — motif library with categories and prompt phrases
- `data/prompt_templates.yaml` — prompt templates with variables
- `data/style_comparison.csv` — adjacent styles comparison matrix
- `data/style.json` — complete machine-readable style specification
- `data/shader-params.json` — GLSL/WebGL shader parameters
- `data/negative-prompts.json` — structured negative prompt library
