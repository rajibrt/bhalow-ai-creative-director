# Bhalow AI Creative Director

Production knowledge system for **Bhalow**, a US-first premium fragrance and beauty e-commerce brand.

## Release

- **Current version:** 2.1.0
- **Status:** Production release candidate
- **Primary market:** United States
- **Customer-facing language:** US English
- **Currency:** USD
- **Website:** www.bhalow.com

## What This Repository Does

This repository is the source of truth for the Bhalow AI Creative Director Custom GPT. It defines how the GPT:

- Classifies creative requests
- Selects campaign direction
- Protects product and logo identity
- Builds luxury compositions
- Writes US-market copy
- Produces campaign prompts and creative blueprints
- Applies platform and quality checks

The GPT should behave like a senior creative director, not a generic prompt writer.

## Production Knowledge Set

Upload these eight files to the Custom GPT Knowledge section in numeric order:

```text
knowledge-v2/
├── 01_CORE_FOUNDATION.md
├── 02_ENGINE.md
├── 03_CREATIVE_RULES.md
├── 04_TEMPLATES.md
├── 05_PRODUCT_SYSTEM.md
├── 06_COPY_SYSTEM.md
├── 07_EXAMPLES.md
└── 08_MEMORY.md
```

### File Responsibilities

| File | Responsibility |
|---|---|
| `01_CORE_FOUNDATION.md` | Brand identity, operating principles, market position, quality bar |
| `02_ENGINE.md` | Intent detection, routing, execution order, conflict priority |
| `03_CREATIVE_RULES.md` | Style, composition, typography, logo, hierarchy, negative space |
| `04_TEMPLATES.md` | Campaign systems and production prompt structures |
| `05_PRODUCT_SYSTEM.md` | Product preservation, scale, materials, camera, interaction, QA |
| `06_COPY_SYSTEM.md` | US-English brand voice, headlines, CTA, promotional and claim rules |
| `07_EXAMPLES.md` | Reusable campaign blueprints and decision examples |
| `08_MEMORY.md` | Compact permanent defaults and recurring constraints |

## Custom GPT Setup

1. Open the Bhalow AI Creative Director in GPT Builder.
2. Keep the approved production instructions in the Instructions field.
3. Remove superseded knowledge files from the GPT.
4. Upload the eight files from `knowledge-v2/` in numeric order.
5. Enable Image Generation and Web Search when available and appropriate.
6. Save the GPT and run the release tests below.

## Release Tests

The GPT should pass these minimum tests before production use:

### Website Thumbnail

Prompt: `Create a website thumbnail from this product image.`

Expected:

- 1:1
- Product only
- White or soft neutral background
- No copy, CTA, logo, or campaign props

### Homepage Hero

Prompt: `Create a premium homepage hero banner for this fragrance.`

Expected:

- Standalone hero artwork
- Product occupies approximately 35–55% of width
- Copy-safe and CTA-safe areas
- No navigation, search, account, cart, header, footer, browser frame, or full website UI

### Luxury Beauty Campaign

Prompt: `Create a luxury beauty campaign with a model holding this fragrance.`

Expected:

- Natural anatomy and grip
- Product label visible
- Product identity preserved
- Premium beauty lighting

### Social Campaign

Prompt: `Create a premium Facebook post for this product.`

Expected:

- Product-first campaign direction
- Mobile-readable hierarchy
- Concise US-English copy
- No invented price, discount, claims, or product facts

## Governance

- `knowledge-v2/` is the active production knowledge base.
- Old folders may remain as historical references but must not be uploaded together with `knowledge-v2/`.
- New rules must be placed in the file responsible for that domain.
- Avoid duplicating the same rule across multiple files unless it is a critical permanent constraint.
- Update `CHANGELOG.md` and `VERSION.md` with every release.

## Product and Logo Safety

- Uploaded product references are the source of truth.
- Never intentionally redesign a bottle, label, cap, package, or product variant.
- Never recreate, redraw, recolor, crop, stretch, or imitate the official Bhalow logo.
- When exact fidelity cannot be guaranteed, reserve a clean compositing area for post-production.

## Core Promise

Every output should improve product recognition, luxury perception, customer trust, commercial usability, and Bhalow brand consistency.
