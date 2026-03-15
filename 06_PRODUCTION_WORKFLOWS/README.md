# Production Workflows

This directory covers how to recreate New Age Glam Fantasy aesthetics in production and post-processing contexts — outside of prompting.

---

## Purpose

This section bridges the prompt-based workflow to the hands-on production workflow. It covers:

- Post-processing recipes (Photoshop, After Effects, DaVinci Resolve, TouchDesigner)
- AI generation workflow (generation → selection → post treatment)
- VHS/CRT effect recreation methods
- Color grading pipeline for the style palette
- Shader/GLSL implementation

---

## Machine-readable production data

For shader and app integration, see:

- **`../data/shader-params.json`** — Complete GLSL/WebGL shader parameters including:
  - Normalized RGB palette for GPU uniforms
  - Color grading (lift/gamma/gain) values
  - Bloom parameters
  - Halation settings
  - VHS softness settings
  - Chroma bleed settings
  - CRT scanline settings
  - Film grain settings
  - Diffusion filter settings
  - Three intensity presets (Level 1, 2, 3)
  - GLSL uniform variable names
  - Post-processing tool guides (Photoshop, After Effects, DaVinci, TouchDesigner)

---

## Quick post-processing recipe (Photoshop)

1. Add Curves adjustment: lift shadows slightly toward violet, boost pink/blue in highlights
2. Add Lens Blur (5–12px) on luminance channel for diffusion
3. Apply VHS horizontal motion blur (dominant horizontal)
4. Add Gradient Map overlay at 15–25% opacity using pink→violet→teal gradient
5. Add Noise overlay at 4–8% for grain
6. Screen-mode glow layer: Gaussian blur copy at 30–40% opacity
7. Add slight chroma aberration via Channel offset (R: +1-2px, B: -1-2px)

---

## Recommended tools

| Tool | Use |
|------|-----|
| Photoshop | Bloom, chroma bleed, scanlines, color grading |
| After Effects | VHS plugins, CRT effects, animated artifacts |
| DaVinci Resolve | Color grading, halation, film grain |
| TouchDesigner | Real-time shader pipeline, live generative |
| GLSL/WebGL | Custom shaders, integration with art apps |
| Retrograde / VHS Cam / Glitché | Dedicated VHS/analog app treatment |

---

## Planned files

- `ai-generation-workflow.md` — End-to-end AI art generation workflow
- `vhs-crt-treatment.md` — Detailed VHS/CRT recreation methods
- `color-grading-guide.md` — DaVinci and Resolve-specific color pipeline
- `glsl-shader-guide.md` — GLSL shader integration walkthrough
- `photoshop-actions.md` — Photoshop action sequences for the style
