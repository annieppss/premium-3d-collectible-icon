---
name: premium-3d-collectible-icon
description: Create a single premium 3D collectible toy-style icon from a requested word or concept. Use when the user asks for a cute, glossy, high-end 3D object icon, a collectible designer-toy render, or a consistent summer-themed 3D icon; generate the image with ImageGen.
---

# Premium 3D Collectible Icon

Generate one square ImageGen image per requested concept. Treat the object itself as the icon—not an app tile, badge, or illustration.

## Workflow

1. Identify whether the requested concept is a living creature/character or a non-living object.
2. Select a distinct, plausible premium material that supports its identity. Vary materials across a set: glossy PVC inflatable, soft resin, transparent acrylic, smooth ABS, soft rubber, glass, fabric, wood, or chrome.
3. Call `image_gen.imagegen` with the prompt below, replacing `[CONCEPT]`, `[LIVING-FEATURES]`, and `[MATERIAL]`. Generate directly; do not ask follow-up questions unless the concept is ambiguous.
4. Return the generated image. If the user requests a set, preserve the shared lighting, framing, and background while giving each object a different material identity.

## Prompt Template

```text
Create a premium 3D collectible toy-style icon of a cute [CONCEPT].

The object itself is the icon. It looks like a real, high-end collectible product rather than a flat UI symbol. Use a simple, bold, instantly recognizable silhouette with soft, rounded, chunky proportions and visible volume. Smoothly round every edge; no sharp corners. Center the object perfectly and make it occupy approximately 80% of a square canvas.

Use [MATERIAL] with a refined, premium finish. The surface is smooth, clean, high quality, and has subtle realistic reflections; it must not resemble cheap toy plastic or have rough textures. Use rich, fresh, playful summer colors with slightly increased saturation: sky blue, aqua, mint, coral, watermelon red, sunshine yellow, fresh green, bubblegum pink, lavender, white, and transparent accents. Avoid neon, dull, muddy, grayish, dirty, or desaturated colors.

Use soft, even studio lighting with clean highlights and gentle reflections that reveal the curves. No harsh shadows, dramatic contrast, heavy bloom, grain, or noise. Place it on a pure white (#FFFFFF) seamless background with no floor, horizon line, scenery, or other objects.

[LIVING-FEATURES]

No text, logo, watermark, UI elements, app tile, rounded-square background, scenery, extra accessories, duplicated objects, missing parts, low-poly geometry, clay render, dirty textures, scratches, grain, noise, or exaggerated proportions. No anthropomorphic features on non-living objects. Ultra-high-quality 3D render, premium collectible designer toy, luxury product photography, high-end CGI, clean studio lighting, 8K detail.
```

## Conditional Text

- **Living creature or character:** Set `[LIVING-FEATURES]` to: `Add minimal cute facial features: small, simple eyes and a gentle friendly expression. Keep the anatomy and collectible-toy style intact.`
- **Non-living object:** Set `[LIVING-FEATURES]` to: `Do not add eyes, a nose, mouth, or any anthropomorphic features. Preserve the original shape and identity of the object.`

## Puppy in Swim Tube Preset

Apply this preset when the request is a puppy or dog riding in a swim tube. Keep the pose, camera, and material rules stable; treat the breed and colors as user-controlled variables.

- Use the requested dog breed; if none is named, choose a cute puppy breed. Render it as smooth, seamless soft vinyl or resin with no fur, hair, or realistic animal texture.
- Seat the puppy inside the tube's center opening, not on top of it. Rest its rounded front paws on the top edge. Keep its short rounded hind paws naturally visible inside the front opening; do not place legs below the tube or push the paw pads toward the camera.
- Give it tiny simple dark eyes, a small nose, a happy smile, and a small pink tongue slightly showing. Preserve a front-facing, centered pose unless the user explicitly requests another pose.
- Include a simple two-piece bikini by default. Use the requested bikini color; otherwise use hot pink. Change the bikini color freely without changing its simple toy-like form.
- Use a transparent, visibly inflated glossy PVC swim tube. Use the requested tube color; otherwise use transparent sky blue. Keep the tube transparent even when its color changes.
- Preserve the square, centered, premium collectible composition and soft studio lighting from the main prompt.

## Material Selection

Choose one primary material that naturally fits the concept. Examples: an inflatable swim ring → glossy PVC; a jellyfish → transparent aqua acrylic; a strawberry → soft resin; a beach umbrella → smooth ABS with fabric canopy; a seashell → pearlescent resin; sunglasses → translucent acrylic and chrome.

Do not add accessories, labels, or a pedestal unless they are essential to the requested object's recognizable form.
