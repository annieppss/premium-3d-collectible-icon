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

## Signature Summer Finish

Apply this finish by default to create the compact, precious summer collectible look. It overrides the plain-white-background instruction only when the user has not explicitly requested a completely blank background.

- Keep a single object compact and fully visible, usually 65–75% of the square canvas, with generous clean breathing room.
- Use a luminous white-to-silver pearly ripple surface with subtle, low-contrast water caustics. Keep it seamless: no horizon, beach scene, or visible floor edge.
- Use one large soft studio source from upper left. Add small clean highlights and a delicate reflection under the object; never use hard shadows, dark gray casts, or dramatic contrast.
- Make smooth materials look touchable and valuable: rounded geometry, controlled gloss, crisp transparent edges, and small restrained specular highlights. Avoid photoreal texture, excessive detail, and oversized product-shot cropping.

## Inflated PVC Material Finish

Use this as the default material language for collectible figures, clothing, parasols, loungers, and other forms that can plausibly be soft or air-filled. Keep technically transparent objects such as glass bowls, mugs, and lenses as clear acrylic/glass, but retain the same polished collectible finish.

- Make forms look softly air-filled and gently inflated: smooth bulging volumes, broad clean white highlights, subtle translucent depth, and slight compression at natural contact points.
- Add restrained heat-sealed seam cues only where construction naturally requires them. Keep every surface pristine, premium, and soft—not hard resin, ceramic, matte plastic, fabric, latex, or cheap pool-float plastic.
- Use a high-gloss clear-coated PVC appearance with curved reflections, never a dry, chalky, matte, rough, or photoreal-textured surface.
- Preserve the object's recognizable structure. Do not overinflate small food components, beans, ice flakes, glassware, or details whose natural form should remain irregular.

## Multiple Puppy Variation

Apply this rule when a scene contains two or more puppies.

- Give each puppy a distinct expression, pose, and clothing design; never mirror the same face, pose, or outfit.
- When swimwear is requested, vary the styles automatically: use simple swim shorts on one puppy and a frilled two-piece bikini or monokini on another. Apply different user-requested colors when supplied.
- Keep all puppies wholesome, baby-puppy proportioned, smooth soft-PVC figurines with no fur texture or adult-like anatomy.

## Beer Mug Preset

Apply this preset when the request is beer, a cold beer, a beer mug, or a closely related phrase.

- Use exactly one compact, rounded clear beer mug with a small rounded handle. Keep it at 65–70% of the square canvas, never an oversized close-up.
- Fill it with clear amber-golden beer and top it with a chunky, creamy-white, softly billowing foam cap. Add one small rounded foam drip over the front rim.
- Make the mug thick, polished transparent acrylic or glass. Make the foam smooth soft resin/PVC-like rather than realistic bubbly foam.
- Do not add condensation droplets, excessive bubbles, labels, logos, text, or photoreal liquid effects.
- Apply the Signature Summer Finish, including its silver ripple surface and upper-left soft studio reflections.

## Patbingsu Preset

Apply this preset when the request is patbingsu or Korean red-bean shaved ice.

- Use one compact clear rounded bowl with a low, wide shaved-ice mound.
- Make the shaved ice from many tiny irregular translucent white flakes and granules. Never use identical spheres, capsules, pillows, or balloon-like puffs.
- Add a loose coral-pink syrup layer with uneven translucent pieces and soft pooled patches. Never use a thick round jelly sheet.
- Use glossy dark-red beans with small asymmetric oval kidney-bean shapes, subtle size variation, natural clustering, and a light lengthwise bean crease. Never use perfectly round spheres or uniform rows.
- Add one modest creamy pale-yellow vanilla scoop with a gently melting lower edge.
- Keep the bowl clear acrylic and use restrained collectible gloss. Apply the Signature Summer Finish, including its silver ripple surface and upper-left soft studio light.
- Do not use real crushed ice, wet photoreal food, glass shards, puffy balloon forms, oversized ingredients, spoons, garnish, labels, or text.

## Puppy in Swim Tube Preset

Apply this preset when the request is a puppy or dog riding in a swim tube. Keep the pose, camera, and material rules stable; treat the breed and colors as user-controlled variables.

- Use the requested dog breed; if none is named, choose a cute puppy breed. Render it as smooth, seamless soft vinyl or resin with no fur, hair, or realistic animal texture.
- Seat the puppy inside the tube's center opening, not on top of it. Rest its rounded front paws on the top edge. Keep its short rounded hind paws naturally visible inside the front opening; do not place legs below the tube or push the paw pads toward the camera.
- Give it tiny simple dark eyes, a small nose, a happy smile, and a small pink tongue slightly showing. Preserve a front-facing, centered pose unless the user explicitly requests another pose.
- Include a simple two-piece bikini by default. Use the requested bikini color; otherwise use hot pink. Change the bikini color freely without changing its simple toy-like form.
- Use a transparent, visibly inflated glossy PVC swim tube. Use the requested tube color; otherwise use transparent sky blue. Keep the tube transparent even when its color changes.
- Preserve the square, centered, premium collectible composition and soft studio lighting from the main prompt.

## Pearl Shell Preset

Apply this preset when the request is a pearl inside an open shell, a pearl shell, or a closely related phrase.

- Use one open scallop shell containing exactly one pearl. Keep the shell non-anthropomorphic: no face or extra decorations.
- Make the shell from translucent pearlescent resin or pearlescent PVC. Use an ivory, blush-pink, and lavender gradient unless the user requests different colors.
- Add a delicate aurora iridescence only along the shell edges; keep it refined and subtle.
- Give the shell interior and creamy-white pearl soft diffused illumination plus small, clean specular highlights, producing an elegant gentle inner glow rather than a strong light source.
- Do not use metallic surfaces, rough textures, excessive glitter, or strong neon emission.
- Preserve the square, centered, premium collectible composition and soft upper-left studio highlights from the main prompt.

## Material Selection

Choose one primary material that naturally fits the concept. Examples: an inflatable swim ring → glossy PVC; a jellyfish → transparent aqua acrylic; a strawberry → soft resin; a beach umbrella → smooth ABS with fabric canopy; a seashell → pearlescent resin; sunglasses → translucent acrylic and chrome.

Do not add accessories, labels, or a pedestal unless they are essential to the requested object's recognizable form.
