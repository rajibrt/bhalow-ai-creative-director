# Intent Classifier

## Purpose

The Intent Classifier routes the user's request to the correct Bhalow workflow before any prompt or copy is written.

The GPT should not guess blindly. It should identify what the user is trying to create, then select the matching workflow and template.

## Primary Intent Categories

Classify every request into one primary intent:

1. Website Thumbnail
2. Social Poster
3. Facebook Cover
4. Website Hero Banner
5. CGI Advertisement
6. Product Analysis
7. Product Research
8. Copywriting
9. Quality Review
10. General Strategy

## Intent Signals

### Website Thumbnail

Trigger this intent when the user says:

- website thumbnail
- product thumbnail
- e-commerce image
- white background
- no text
- product image for website
- 1:1 product image

Default workflow:

Product Analyzer → Website Thumbnail Template → Quality Check

### Social Poster

Trigger this intent when the user says:

- social poster
- Facebook post
- Instagram post
- square poster
- product poster
- social media design
- feed post

Default workflow:

Product Analyzer → Copywriting Guide → Social Poster Template → Quality Check

### Facebook Cover

Trigger this intent when the user says:

- Facebook cover
- FB cover
- cover photo
- Facebook banner
- page cover
- brand cover

Default workflow:

Brand Foundation → Visual Identity → Facebook Cover Template → Quality Check

### Website Hero Banner

Trigger this intent when the user says:

- hero banner
- website banner
- homepage banner
- category banner
- collection banner
- landing page banner
- header banner

Default workflow:

Product Analyzer or Brand Foundation → Hero Banner Template → Quality Check

### CGI Advertisement

Trigger this intent when the user says:

- CGI ad
- cinematic ad
- premium ad
- luxury advertisement
- creative product scene
- commercial product ad
- concept ad

Default workflow:

Product Analyzer → Art Direction → CGI Advertisement Template → Quality Check

### Product Analysis

Trigger this intent when the user says:

- analyze this product
- what is this product
- suggest design idea
- what background should I use
- what type of poster should I make

Default workflow:

Product Analyzer → Art Direction Recommendation → Suggested Output Types

### Product Research

Trigger this intent when the user provides:

- Amazon URL
- product URL
- retailer link
- product page link

Default workflow:

Research → Product Analyzer → Copywriting Guide → Suggested Creative Outputs

### Copywriting

Trigger this intent when the user asks for:

- caption
- headline
- CTA
- product description
- SEO title
- meta description
- Facebook status
- hashtags
- website copy

Default workflow:

Copywriting Guide → Brand Foundation → Quality Check

### Quality Review

Trigger this intent when the user asks:

- review this design
- check this image
- what is wrong
- improve this prompt
- why output is bad
- fix this design

Default workflow:

Quality Standards → Visual Identity → Art Direction → Recommendation

### General Strategy

Trigger this intent when the request is broad or planning-focused:

- what should we do
- build a system
- make a plan
- create workflow
- suggest strategy

Default workflow:

Brand Foundation → Roadmap / Strategy Response

## Ambiguous Request Handling

If the user says only:

```text
Create image
```

Ask one focused question:

```text
What do you want to create: website thumbnail, social poster, Facebook cover, hero banner, or CGI ad?
```

If the user says:

```text
Create banner
```

Decide based on context:

- If Facebook is mentioned nearby → Facebook Cover
- If website is mentioned nearby → Hero Banner
- If no context → ask whether it is for Facebook or website

If the user says:

```text
Make poster
```

Default to Social Poster unless another platform is mentioned.

## Priority Rules

1. Explicit user intent always wins.
2. Product image plus “website” usually means Website Thumbnail or Hero Banner.
3. Product image plus “social” usually means Social Poster.
4. Brand logo plus “cover” usually means Facebook Cover.
5. Product URL usually triggers Product Research before creative output.
6. When uncertain, ask one short clarifying question.

## Final Rule

Classify intent first, then choose workflow. Never write a final image prompt before understanding the requested output type.
