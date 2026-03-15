# Prompt Engineering

This directory contains all prompt construction resources for New Age Glam Fantasy.

---

## Files in this directory

| File | Purpose |
|------|---------|
| [prompt-anatomy.md](prompt-anatomy.md) | Layer-by-layer prompt building system, examples, troubleshooting |
| [consistency-recipes.md](consistency-recipes.md) | Reusable prompt recipes for 6 core scene types |
| [negative-prompts.md](negative-prompts.md) | Negative prompt blocks by platform and drift category |

---

## Quick start

If you are new to prompting this style, start with:

1. Read [prompt-anatomy.md](prompt-anatomy.md) to understand the 10 prompt layers
2. Copy a recipe from [consistency-recipes.md](consistency-recipes.md) and fill in your variables
3. Add negative prompts from [negative-prompts.md](negative-prompts.md) as guardrails

---

## Always end prompts with the style lock line

```
Style: New Age Glam Fantasy — 1978–1986 metaphysical glam sci-fantasy, diffusion bloom/halation, prismatic pastels, VHS/CRT artifacts, analog film wear.
```

---

## Machine-readable data

For programmatic prompt building:
- `../data/prompt_templates.yaml` — YAML prompt templates with variables
- `../data/style.json` — Complete style spec including prompt examples
- `../data/negative-prompts.json` — Structured negative prompt library

---

## Planned files

- `video-prompts.md` — Motion/video specific prompt techniques
- `platform-guides.md` — Platform-specific optimization (Midjourney, SD, DALL-E, Firefly, etc.)
- `prompt-testing-log.md` — Community-sourced prompt test results
