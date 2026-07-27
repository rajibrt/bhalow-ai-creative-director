# Changelog

All notable changes to the Bhalow AI Creative Director are documented here.

## [3.0.0] — Human Campaign and Creative Operating System

### Added

- Women's Luxury Campaign system
- Men's Luxury Campaign system
- Unisex Luxury Campaign system
- Couple, lifestyle, and luxury grooming campaign systems
- Create, Analyze, Copy, and Analyze-and-Create operating modes
- Fragrance-direction and platform-routing logic
- Gender-inclusive campaign rules that avoid visual stereotypes
- Men's tailored luxury and grooming blueprints
- Strategy-only, copy-only, and analyze-and-create examples
- `gpt-builder/GPT_SETUP.md`
- `gpt-builder/GPT_CONVERSATION_STARTERS.md`

### Changed

- Replaced the beauty-only human campaign model with a complete Human Campaign Intelligence system
- Updated production GPT instructions for v3 behavior
- Strengthened conflict priority so safety and factual accuracy override user requests
- Updated homepage hero, social, product, CGI, thumbnail, and human-campaign templates
- Updated README, version, setup workflow, and release tests

### Fixed

- Added full men's fragrance campaign support
- Prevented women's campaigns from defaulting to pink, flowers, glitter, and identical poses
- Clarified that creative analysis and marketing-copy starters are text modes unless image creation is also requested
- Clarified that analyze-and-create requests must proceed to creation
- Prohibited invented prices, discounts, warranties, specifications, ingredients, certifications, stock status, authenticity guarantees, and promotional claims

### Migration

1. Replace the GPT Builder Instructions with `instructions/GPT_INSTRUCTIONS.md`.
2. Replace existing knowledge with the eight files under `knowledge-v2/`.
3. Configure conversation starters from `gpt-builder/GPT_CONVERSATION_STARTERS.md`.
4. Do not mix legacy knowledge files with v3.

## [2.1.0] — Creative Intelligence Foundation

- Established the eight-file knowledge architecture
- Added product, copy, campaign, memory, and example systems
- Added homepage hero UI restrictions and product/logo protection
