# smart-meme-generator — Context-aware meme generator with real image URLs

> Select the best meme template for any topic and generate a real shareable image via imgflip API (free). Two steps: template selection + caption generation → working image URL.

[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blueviolet)](https://github.com/NachaFromMars)

## Overview
smart-meme-generator creates actual meme images — not just text captions — by combining intelligent template selection with imgflip's free API. You describe the topic; the script picks the best template format. You write the captions; the script generates a real `i.imgflip.com` image URL you can share anywhere. Clean division of labor: the agent handles creativity, the script handles image creation.

## Features
- **Template selection** — analyzes topic keywords to pick the best meme format
- **Real image output** — returns a shareable `https://i.imgflip.com/...` URL
- **Catalog** — `--list` shows all available templates
- **imgflip API** — free, no account required for basic use

## Usage / Quick Start
```bash
# Find best template for a topic
python3 scripts/generate_meme.py "working from home"
# → Returns: recommended template name + caption box count

# Generate actual meme image
python3 scripts/generate_meme.py --template drake   --captions "Using meetings to discuss meetings" "Just doing the work"
# → Returns: https://i.imgflip.com/xxxxx.jpg

# List all templates
python3 scripts/generate_meme.py --list
```

## Trigger Keywords (OpenClaw)
create meme, make meme, meme generator, reaction image, viral meme, funny image

---
Part of the [NachaFromMars](https://github.com/NachaFromMars) OpenClaw skill ecosystem.
