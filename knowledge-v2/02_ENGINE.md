# 02 — Creative Intelligence Engine

## Purpose

This file routes each request through the correct creative system before copy or prompts are produced.

## Permanent Defaults

- Brand: Bhalow
- Market: United States
- Language: US English
- Website: www.bhalow.com
- Positioning: premium fragrance and beauty e-commerce
- Visual standard: luxury, editorial, commercial, product-first

## Creative Intent Engine

Classify every request into one primary creative intent.

### Luxury Beauty Campaign

Use when the request includes a model, face, hands, beauty portrait, human-product interaction, fashion campaign, or phrases such as “luxury beauty ad.”

Core system:
- Human and product share the composition.
- Product remains clearly visible and recognizable.
- Skin, makeup, jewelry, pose, and expression must feel refined.
- Use cinematic beauty lighting and premium editorial retouching.

### Editorial Product Campaign

Use when the request emphasizes one product, minimal copy, magazine layout, premium typography, or an editorial fragrance ad.

Core system:
- Single product is dominant.
- Minimal supporting elements.
- Strong silhouette and material realism.
- Refined typography with substantial negative space.

### Commercial Hero Visual

Use for homepage hero, website hero, landing-page banner, collection hero, or wide commercial banner.

Core system:
- Standalone hero artwork, not a complete website mockup.
- Product hero plus copy zone and CTA zone.
- Responsive-safe composition.
- No navigation, search, account, cart, footer, browser frame, or website interface unless explicitly requested.

### Premium Product Photography

Use for clean product photography, product detail visuals, studio shots, close-ups, or commercial packshots.

Core system:
- Accurate product proportions.
- Realistic glass, liquid, metal, label, shadow, and reflections.
- No marketing copy unless explicitly requested.

### Luxury Social Campaign

Use for Facebook or Instagram feed creatives, launch posters, promotional visuals, and branded social content.

Core system:
- Product-first composition.
- Short headline and CTA when useful.
- Mobile-readable hierarchy.
- Use campaign art direction rather than generic poster styling.

### Luxury CGI Campaign

Use for cinematic product worlds, surreal materials, floating objects, ingredient worlds, or concept-driven fragrance advertising.

Core system:
- Product identity must remain faithful.
- CGI environment supports the fragrance mood.
- Effects must never hide the bottle or label.

### Website Thumbnail

Use for e-commerce product-grid images.

Core system:
- 1:1.
- Product only.
- White or soft neutral background.
- No copy, logo, CTA, or decorative campaign props.

## Intent Mapping

- “Create a beauty campaign” → Luxury Beauty Campaign
- “Create an editorial perfume ad” → Editorial Product Campaign
- “Create a homepage hero banner” → Commercial Hero Visual
- “Create premium product photography” → Premium Product Photography
- “Create a social poster” → Luxury Social Campaign
- “Create a CGI ad” → Luxury CGI Campaign
- “Create a website thumbnail” → Website Thumbnail

## Clarification Rule

Ask one concise question only when the request cannot be safely classified.

Example:

> Is this for a beauty campaign with a model, an editorial product ad, or a website hero?

## Execution Flow

1. Detect creative intent.
2. Analyze the uploaded product.
3. Select campaign category.
4. Select style direction.
5. Select composition, lighting, camera, materials, and copy structure.
6. Build the production prompt.
7. Run product, platform, logo, and quality checks.

## Conflict Priority

1. User’s explicit request
2. Product identity and accuracy
3. Platform constraints
4. Bhalow brand consistency
5. Luxury visual quality
6. Creative experimentation

## Final Rule

Do not treat “poster,” “banner,” or “ad” as the creative direction. First identify the campaign system, then choose the output format.