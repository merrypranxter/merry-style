# Negative Prompts

## Purpose of this file

Negative prompts (or negative terms, depending on platform) tell the AI model what to avoid. For New Age Glam Fantasy, they are critical guardrails that prevent the most common drift patterns.

---

## How to use this file

Platforms handle negative prompts differently:

- **Midjourney**: Use `--no [terms]` at the end of your prompt
- **Stable Diffusion / ComfyUI**: Paste the negative prompt list into the negative prompt field
- **DALL-E / GPT image gen**: Add "Avoid:" or "Do not include:" followed by terms at the end of your prompt
- **Ideogram / Leonardo**: Use the dedicated negative prompt field if available

---

## Core negative prompt block

This is the default negative prompt for most New Age Glam Fantasy work:

```
cyberpunk, urban neon, city streets, streetwear, leather jacket, industrial, dystopian, post-apocalyptic, noir, gritty, grunge, dark occult, demonic, horror, blood, gore, skulls, medieval armor, swords, battle, warrior, fantasy castle, dragon, gritty epic fantasy, hyperrealistic, ultra sharp, 4K crisp, clean CGI, sterile, minimalist, modern luxury, contemporary editorial, vaporwave collage, ironic, parody, meme, Y2K chrome, synthwave grid, outrun horizon, car, highway, purple-black sunset, Japanese text, statues, pixel glitch, datamosh, aggressive distortion, harsh shadows, high contrast hard light, primary red, primary blue, primary yellow, flat stripes, rainbow flag, brown earthy palette, khaki, linen, denim, concrete, brutalist architecture, guns, weapons, wires, implants, rain, alley
```

---

## Negative prompt by category

### Block cyberpunk drift
```
cyberpunk, urban neon, city streets, rainy alley, neon signage, megacity, holographic advertisement, leather jacket, industrial, dystopian, post-apocalyptic, wires, implants, techno-noir, rain-slicked streets
```

### Block synthwave drift
```
synthwave, outrun, retro-wave grid, purple-black sunset gradient, car, highway, palm trees, horizon grid, electronic music poster aesthetic
```

### Block dark fantasy / horror drift
```
dark occult, demonic, horror, blood, gore, skulls, bones, decay, rot, cursed relic, dread, menace, fear, shadow-dominant, grim reapers, skeletons, monsters, undead
```

### Block medieval fantasy drift
```
medieval armor, swords, battle, warrior, castle, dragon, dungeon, gritty epic fantasy, knights, axe, shield, siege warfare, goblin, orc
```

### Block overly sharp / modern digital drift
```
hyperrealistic, ultra sharp, 4K photo-real, clean CGI, crisp digital render, sterile white studio, modern luxury editorial, contemporary fashion photography
```

### Block vaporwave drift
```
vaporwave collage, Japanese text, Greek statue, checkerboard grid, ironic nostalgia, consumer culture debris, corporate glitch
```

### Block earthy bohemian drift
```
linen, canvas, earth tones, khaki, brown rustic, natural fibers, desert realism without glamour, boho festival, folk spiritual simplicity
```

### Block generic ethereal AI drift
```
generic celestial, vague sparkle, generic magic woman, random stars background, over-polished symmetry, empty cosmic backdrop, lifeless ethereal glow
```

### Block aggressive glitch / datamosh
```
datamosh, pixel glitch, aggressive distortion, digital corruption, hard glitch art, RGB tearing, extreme chromatic aberration
```

---

## Color-based negative terms

These color terms tend to push prompts in the wrong direction:

```
primary red, primary blue, primary yellow, black dominant, high contrast stark shadows, muted desaturated, gray scale, military green, hospital white, navy blue, burnt orange, mustard yellow, khaki, olive drab, brown-beige, earth brown
```

---

## Negative prompts for specific use cases

### Portrait / beauty work
```
harsh studio lighting, unflattering angles, newspaper photo realism, clinical documentation, paparazzi style, modern magazine minimalism, harsh shadows under eyes, unflattering pose
```

### Environmental / landscape
```
urban city, factory, industrial plant, power lines, traffic, parking lot, gray concrete, modern architecture, glass office building, airport
```

### Cover art
```
modern book design minimalism, sans-serif type-only layouts, clean tech branding, contemporary corporate design, flat vector illustration
```

### Video / motion
```
handheld documentary camera, realistic news footage, surveillance camera angle, action cam POV, modern music video cuts, commercial product video aesthetic
```

---

## Platform-ready blocks

### Midjourney (append to prompt)
```
--no cyberpunk urban neon dystopian horror blood gore medieval armor swords sharp crisp hyperrealistic modern editorial vaporwave irony glitch datamosh earthy linen plain sparkle generic celestial primary colors harsh contrast streetwear industrial
```

### Stable Diffusion (negative prompt field)
```
(cyberpunk:1.3), (urban neon:1.2), (city streets:1.1), (horror:1.4), (gore:1.5), (blood:1.5), (medieval armor:1.3), (swords:1.3), (hyperrealistic:1.2), (ultra sharp:1.2), (clean CGI:1.1), (dark occult:1.4), (demonic:1.5), (dystopian:1.2), (industrial:1.1), (vaporwave:1.2), (ironic:1.1), (datamosh:1.3), (harsh shadows:1.2), (primary red:0.8), (plain sparkle:1.1), nsfw, ugly, deformed, blurry face, bad anatomy, extra limbs
```

### DALL-E / ChatGPT image generation (add to prompt end)
```
Avoid: cyberpunk, urban environments, horror, gore, blood, medieval battle scenes, modern digital sharpness, harsh studio lighting, vaporwave irony, dark occult, industrial settings, datamosh glitch, earthy boho palette, generic sparkle.
```

---

## Notes on using negative prompts

1. **Don't over-negate**: Too many negative terms can confuse models or reduce quality. Use the core block as default; add category-specific terms only when you see that specific drift.

2. **Platform behavior varies**: Some models respond strongly to negative terms; others barely register them. If negative prompts don't help, try rephrasing your positive prompt instead.

3. **Negative prompts supplement, not replace, positive direction**: A strong, specific positive prompt with clear era anchors and motif language is usually more effective than relying on negative prompts alone.

4. **The style lock line is also a form of positive guardrail**: Always include the style lock line:
   ```
   Style: New Age Glam Fantasy — 1978–1986 metaphysical glam sci-fantasy, diffusion bloom/halation, prismatic pastels, VHS/CRT artifacts, analog film wear.
   ```

---

## Machine-readable version

A structured JSON version of these negative prompts is available at `../data/negative-prompts.json`.
