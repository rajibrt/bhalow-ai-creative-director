# 05 — Product Intelligence System

**Knowledge version:** 2.1.0  
**Status:** Production

## Purpose

Protect product identity while selecting the correct scale, camera, lighting, materials, environment, and human interaction for premium fragrance visuals.

## Source of Truth

The uploaded product image, approved product file, or verified product page is the source of truth.

Do not replace observed details with assumptions. Preserve:

- Bottle geometry
- Cap shape and finish
- Label position and proportions
- Printed brand and product text
- Glass tint and transparency
- Liquid color and fill level
- Box proportions and artwork
- Metallic, matte, glossy, frosted, embossed, or textured finishes

## Product Analysis Pass

Before writing a prompt or directing an image, identify:

1. Product type: bottle, bottle + box, gift set, discovery set, or accessory.
2. Dominant geometry: rectangular, cylindrical, sculptural, rounded, faceted, or irregular.
3. Main materials: clear glass, tinted glass, metal, plastic, paperboard, fabric, stone-like finish.
4. Color system: bottle, liquid, cap, label, and packaging colors.
5. Reflectivity: matte, satin, glossy, mirrored, transparent, translucent.
6. Fragrance cues visible from packaging: floral, aquatic, woody, citrus, gourmand, dark, clean, romantic, or celebratory.
7. Vulnerable details: small text, thin cap, unusual silhouette, transparent edges, metallic lettering, or box artwork.

## Preservation Rules

Never intentionally:

- Rename the product
- Replace the label
- Change the cap
- Change bottle proportions
- Add nonexistent embossing
- Remove recognizable design details
- Invent a matching box
- Add an unauthorized logo
- Turn one product into a different variant

When generative fidelity is uncertain, instruct the system to preserve the reference and recommend final product compositing.

## Label Protection

The label and brand name must remain readable whenever visible in the reference.

- Keep fingers, petals, mist, reflections, glare, water, ribbons, and props away from critical text.
- Avoid steep angles that distort the label unless the request is intentionally abstract.
- Control highlights so white labels do not blow out and dark labels do not disappear.
- Do not generate new label copy.

## Product Scale System

Use these starting ranges, then adapt to the composition:

- Website thumbnail: 65–85% of canvas height with safe margins
- Editorial product campaign: 55–80% of visual hierarchy
- Homepage hero: 35–55% of canvas width
- Social campaign: 40–65% of visual hierarchy
- Beauty campaign: 20–40%, but still immediately recognizable
- CGI product world: 35–65%, depending on environment complexity
- Detail shot: crop intentionally around one verified feature

A product is too small when it reads as a prop instead of the commercial subject.

## Camera Language

### Clean Packshot

- Front or slight three-quarter view
- 70–120mm product-photography feel
- Minimal perspective distortion
- Edge-to-edge sharpness

### Editorial Hero

- Front three-quarter or controlled low angle
- 70–100mm feel
- Sculptural silhouette
- Moderate depth without losing label clarity

### Beauty Interaction

- 50–85mm portrait feel
- Face and product both resolved
- Product plane oriented toward camera

### CGI Campaign

- Camera angle may be dramatic, but bottle geometry must remain credible
- Avoid extreme wide-angle distortion
- Use depth and scale deliberately

## Lighting by Material

### Clear or Tinted Glass

- Use broad controlled highlights to reveal edges.
- Show believable refraction and liquid depth.
- Avoid flat front light that removes dimensionality.

### Metallic Cap or Lettering

- Use narrow controlled highlights and clean reflection cards.
- Avoid noisy, broken, or plastic-looking metal.

### Matte Packaging

- Use soft directional light to reveal texture.
- Preserve printed contrast without artificial gloss.

### Frosted Glass

- Use rim light and subtle transmission.
- Avoid making frosted surfaces look like opaque plastic.

## Reflection and Shadow Rules

- Reflections must follow product geometry and scene lighting.
- Ground contact must feel physically believable.
- Use soft contact shadow for clean e-commerce work.
- Use longer directional shadow only when it supports the concept.
- Mirror reflections must not duplicate or mutate the product.
- Avoid floating products unless the campaign explicitly calls for suspension.

## Product + Packaging

When bottle and box appear together:

- Maintain true relative scale.
- Do not let the box hide the bottle label.
- Keep both on a consistent ground plane.
- Use the box as secondary hierarchy unless the packaging is the requested hero.
- Preserve box artwork and orientation.

## Human Interaction System

### Hands

- Use anatomically correct hands and natural grip pressure.
- Keep all fingers distinct and credible.
- Do not cover product name or label.
- Do not merge fingers into glass, cap, or packaging.
- Match grip to bottle size and weight.

### Placement

Preferred placements:

- Near the face without touching facial features awkwardly
- At shoulder or chest level
- Resting naturally in the palm
- Supported by one hand while the other frames the scene

Avoid:

- Floating bottle near the hand
- Impossible wrist angles
- Oversized or miniature product relative to the hand
- Product pressed into skin or hair

## Ingredient and Prop Logic

Use props only when they strengthen the fragrance story or campaign objective.

- Floral: restrained petals, stems, jasmine, rose, tuberose, or abstract botanical forms
- Citrus: peel, light, translucent slices, fresh tonal accents
- Aquatic: controlled water, glass, droplets, ripples, cool transparency
- Woody or oud: dark wood, resin, smoke, leather, stone, bronze
- Gourmand: refined ingredient cues, never food-commercial clutter
- Clean or musky: ivory fabric, soft air, pale stone, translucent layers

Do not claim a prop is an ingredient unless verified.

## Background Selection

Choose backgrounds that improve silhouette and readability.

- Light product: use enough tonal contrast to separate edges.
- Dark product: preserve detail with rim lighting and controlled background lift.
- Transparent product: avoid backgrounds that create confusing internal shapes.
- Busy packaging: use simpler surroundings.

## Website Thumbnail Standard

A Bhalow website thumbnail is an e-commerce asset, not a campaign poster.

Mandatory defaults:

- 1:1
- Product only
- White or soft neutral background
- Accurate scale and centered balance
- Soft realistic drop shadow permitted
- No headline
- No CTA
- No decorative props
- No Bhalow logo unless explicitly requested

## Product QA Gate

Before final output, verify:

- Correct product and variant
- Bottle silhouette preserved
- Cap preserved
- Label unobstructed
- Packaging accurate when present
- Product scale appropriate
- Glass and metal physically believable
- Reflections and shadows coherent
- Human interaction anatomically credible
- Props do not imply unsupported facts
- Product remains the visual hero

## Final Product Rule

Creative ambition may transform the world around the product, but must never transform the product into something else.
