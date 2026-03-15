# Templates

This directory contains reusable templates for creating new entries and prompts in the New Age Glam Fantasy style system.

---

## Available templates

### Prompt templates
Machine-readable prompt templates are in `../data/prompt_templates.yaml`. These include:
- Short prompt template with variables
- Medium prompt template with example
- Long prompt template with detailed example
- Subject options
- Setting options
- Motif clusters
- Lighting modes
- Palette families
- Analog levels
- Format cues

### Consistency recipes
Reusable prompt recipes are in `../05_PROMPT_ENGINEERING/consistency-recipes.md`. These include:
1. Oracle Portrait recipe
2. Cosmic Landscape recipe
3. VHS Memory Frame recipe
4. Glamour Close-Up recipe
5. Initiatory Scene recipe
6. Maximalist Cover Art recipe

---

## Planned template files

- `motif-entry-template.md` — Template for adding a new motif to `03_MOTIF_LIBRARY/`
- `reference-entry-template.md` — Template for adding a new reference to `07_REFERENCE_GALLERY/`
- `style-comparison-template.md` — Template for adding a new adjacent style comparison
- `prompt-test-template.md` — Template for logging and evaluating prompt test results

---

## Using the YAML template data

The `../data/prompt_templates.yaml` file can be consumed programmatically:

```python
import yaml

with open('data/prompt_templates.yaml', 'r') as f:
    templates = yaml.safe_load(f)

# Get the style lock line
style_lock = templates['style_lock_line']

# Build a short prompt
template = templates['short_prompt']['template']
filled = template.format(
    subject="A radiant oracle",
    setting="a mirrored crystal temple",
    motifs="glowing mushrooms and crystal clusters",
    lighting="halo backlight through mist",
    palette="hot pink violet aqua",
    optics="soft diffusion bloom",
    format="metaphysical paperback cover"
)
```
