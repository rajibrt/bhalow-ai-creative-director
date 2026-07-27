# Bhalow AI Creative Director

Production operating system for **Bhalow**, a US-first premium fragrance and beauty e-commerce brand.

## Release

- **Current version:** 3.0.0
- **Status:** Production
- **Primary market:** United States
- **Customer-facing language:** US English
- **Currency:** USD
- **Website:** www.bhalow.com

## What v3 Adds

- Women's, men's, unisex, couple, lifestyle, and grooming campaign intelligence
- Clear Create, Analyze, Copy, and Analyze-and-Create operating modes
- Fragrance-direction routing without inferring facts from bottle color
- Stronger factual-accuracy priority
- Platform-specific creative behavior
- Complete GPT Builder setup documentation and conversation starters

## GPT Builder Setup

1. Copy `instructions/GPT_INSTRUCTIONS.md` into the GPT Builder Instructions field.
2. Follow `gpt-builder/GPT_SETUP.md` for name, description, capabilities, and release tests.
3. Use `gpt-builder/GPT_CONVERSATION_STARTERS.md` for approved conversation starters.
4. Remove superseded knowledge files from the GPT.
5. Upload only the eight active files below in numeric order.

## Production Knowledge Set

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

Do not upload legacy knowledge files together with this package.

## File Responsibilities

| File | Responsibility |
|---|---|
| `01_CORE_FOUNDATION.md` | Brand identity, operating principles, market position, quality bar |
| `02_ENGINE.md` | Operating modes, intent routing, human campaign selection, fragrance and platform logic |
| `03_CREATIVE_RULES.md` | Inclusive human art direction, composition, typography, hierarchy, logo and safe-area rules |
| `04_TEMPLATES.md` | Production campaign systems and executable prompt structures |
| `05_PRODUCT_SYSTEM.md` | Product preservation, scale, materials, camera, interaction, QA |
| `06_COPY_SYSTEM.md` | US-English brand voice, headlines, CTA, promotional and factual-claim rules |
| `07_EXAMPLES.md` | Women's, men's, unisex, strategy, copy, hero, social, CGI and product blueprints |
| `08_MEMORY.md` | Compact permanent defaults and recurring constraints |

## Required Release Tests

### Men's Campaign
Prompt: `Create a luxury men's fragrance campaign.`

Expected: premium grooming and wardrobe, natural confidence, correct anatomy, visible product, no macho or generic black-and-gold clichés.

### Women's Campaign
Prompt: `Create a luxury women's fragrance campaign.`

Expected: refined contemporary beauty direction without automatically using pink, roses, glitter, or identical poses.

### Unisex Campaign
Prompt: `Create a premium unisex fragrance campaign.`

Expected: modern gender-neutral editorial direction without forced stereotypes.

### Homepage Hero
Prompt: `Create a homepage hero banner for this product.`

Expected: standalone artwork, product 35–55% width, copy/CTA-safe space, no navigation or website UI.

### Website Thumbnail
Prompt: `Create a clean website thumbnail from this product image.`

Expected: 1:1, product only, neutral background, no copy, CTA, logo, or props.

### Mode Tests

- `Analyze this fragrance and recommend the best creative direction.` → strategy text only
- `Write premium US-market marketing copy for this product.` → copy text only
- `Analyze this fragrance and create the strongest campaign concept.` → analysis-led creation, not analysis-only

## Governance

- GitHub is the source of truth.
- `knowledge-v2/` is the active GPT knowledge package.
- `instructions/` contains the production system instructions.
- `gpt-builder/` contains UI configuration and recovery documentation.
- Update `CHANGELOG.md` and `VERSION.md` with every release.
- Safety and factual accuracy always override creative requests.

## Core Promise

Every output should improve product recognition, audience relevance, luxury perception, customer trust, commercial usability, and Bhalow brand consistency.