---
name: photo-interactive-design
description: Create or prompt tall travel-editorial posters that preserve an uploaded photograph while transforming it into a related graphic design through an interlocking transition zone, balanced visual weight, and an intentional mood-led color treatment. Use for requests involving original-photo plus illustration layouts, torn-paper or wave transitions, photo-to-design interaction, paper-texture zines, travel-photo posters, expressive photo grading, or multiple photos that should each become separate coordinated posters.
---

# 照片交互设计

Turn one supplied photograph into a vertical paper poster where the real photo and its derived graphic design visibly interact instead of sitting in two disconnected boxes.

## Route The Request

- Default to **Generate Mode** when the user asks to make, create, or produce a poster. Return the generated raster image and the final prompt.
- Use **Prompt-only Mode** only when the user explicitly asks for a reusable prompt without generating an image.
- Treat every supplied photograph as an **edit target** unless the user says it is style reference only.
- When several photographs are supplied, make one independent poster per photograph unless the user explicitly requests one combined collage.

Read `references/transition-patterns.md` before compiling any prompt.

## Inspect And Preserve

1. Inspect every supplied image before describing or using it. Record dimensions when available, main subject count, relative positions, scale, interaction, dominant lines, colors, mood, visible text, brands, and sensitive information.
2. Use High preservation for identifiable people, products, artworks, pets, tickets, documents, or distinctive objects. Prefer an original-photo crop or clipped photographic fragment over redrawing.
3. List concrete invariants: identity, face, body proportions, pose, object count, geometry, spatial order, landmark traits, recognizable colors, and interaction.
4. Allow only crop, scale within the poster, restrained print treatment, privacy masking, and the transition effects declared in the prompt.
5. Obscure personal names, barcodes, QR codes, booking details, addresses, account data, or other sensitive text unless the user explicitly requires readable preservation.

## Build The Poster

Use a tall 3:5 warm-paper canvas unless the user requests another ratio.

- Keep the clear photographic region around 43%-48% of the canvas height.
- Keep a narrow paper border at the top and sides.
- Do not finish the photo with a straight rectangular bottom edge.
- Reserve an overlapping 10%-15% transition zone rather than an additive third panel.
- Use a lower derived-design region around 32%-38%, with enough open paper that the result still feels editorial.
- Select one main accent hue and at most one subordinate hue after the color-emotion analysis. They may come from the source or be a justified mood-led transformation of it.
- Use small monospaced, typewriter, old-serif, or fine-serif text. Invent only a short content-related English title and non-identifying microtext.

## Balance The Visual Weight

Treat the percentage ranges as starting points, not a license to place a visually heavy photograph over a weak decorative footer. Balance perceived mass across the complete 3:5 canvas before generating.

1. Make a thumbnail-level weight map of the source: identify its darkest or highest-contrast mass, the main directional flow, the subject's visual center, and the largest empty area.
2. Set the combined transition plus lower design to carry roughly **35%-45% of the poster's perceived visual weight**, even when it uses more negative space. Increase scale, stroke weight, contrast, repetition, or vertical reach when the upper photo is dark, dense, wide-angle, or architecturally complex. Reduce those properties when the photo is pale and quiet.
3. Give the lower design one dominant anchor occupying about **22%-32% of the canvas area** or an equivalent distributed field. Do not leave it as a tiny pale icon floating at the bottom. Let its widest or strongest element span about **55%-80% of the usable width** when the photograph is visually broad.
4. Use the transition as a structural counterweight. Continue one or two strong source directions into the lower half, such as a staircase arc, horizon, facade rhythm, road, shoreline, or movement path. Avoid concentrating all contrast, detail, and curvature above the midpoint.
5. Place title and microtext as secondary counterweights near an otherwise empty lower corner; typography must support the composition but must not compensate through oversized text.
6. Preserve breathing room around the lower anchor. Visual balance means deliberate scale and placement, not filling every blank area.

Judge balance by the poster's **optical center**, not only by geometric height. The finished composition should feel stable when blurred or viewed at thumbnail size: neither top-heavy nor bottom-heavy, with no isolated weak footer.

## Direct Color And Emotion

Do not automatically use the source photograph as the final color benchmark. Analyze the image first, then choose a color direction that best expresses its subject, light, atmosphere, and emotional meaning.

1. Assess the source white balance, dominant and secondary hues, saturation, tonal contrast, highlight and shadow character, weather or ambient light, and emotional cues such as calm, playfulness, nostalgia, solitude, energy, intimacy, or distance.
2. Choose one explicit color strategy:
   - **Faithful natural:** retain the source color relationship when it already communicates the intended feeling.
   - **Harmonized editorial:** correct an accidental cast, compress competing colors, or shift temperature and contrast so the photo, paper, transition, and design read as one system.
   - **Expressive mood-led:** deliberately cool, warm, mute, brighten, darken, or selectively recolor the poster when that treatment better conveys the scene's emotion. Ground the shift in visible content rather than applying a fashionable preset.
3. Choose the paper color as part of the emotional palette. It may be neutral white, soft ivory, cool gray-white, dusty tinted paper, or another restrained tone. Coordinate it with the photographic grade and design inks; warm ivory is a default, not a requirement.
4. Preserve believable skin, clean neutrals, important object colors, and identity- or location-defining color relationships unless the user explicitly requests a stronger stylization. Separate intentional mood color from accidental color contamination.
5. Apply color selectively. Avoid one opaque yellow, sepia, cyan, green, or magenta wash across paper, skin, whites, shadows, and design. Maintain tonal separation and at least one convincing neutral reference.
6. State the selected color strategy, emotional intention, paper tone, main accent, subordinate accent, and protected colors in the generation prompt. Let the same controlled palette cross the photo, transition, and lower design.

## Make The Transition Bidirectional

Choose one primary transition grammar from the reference file and one supporting print texture.

Require all three connections:

1. **Photo moves downward:** irregular photo fragments, subject contours, waterlines, structure lines, leaves, torn fibers, or motion traces extend 3%-8% into the paper field.
2. **Design moves upward:** derived linework, color blocks, symbols, perforations, or textures rise 2%-5% into the photographic area and align with real source features.
3. **Shared visual thread:** one continuous contour, one shared accent hue, and one shared material texture cross the boundary.

When a prominent object touches the transition area, allow part of the original photographic object to protrude across the boundary as a clipped fragment. Never duplicate it as a second realistic object.

## Derive A Readable Design

Reduce the photograph to one central relation, not a full second scene. Preserve subject count, left-to-right or front-to-back order, relative size, and interaction whenever these carry the meaning.

- People may become faceless pictograms, silhouettes, or contour marks; do not generate a second realistic portrait.
- Objects should retain landmark geometry and count.
- Repeated elements such as swimmers, buoys, windows, cabins, tickets, or street lights may become a diagrammatic field, but must remain recognizable at thumbnail size.
- Do not stop at palette extraction. The lower design must communicate what is happening in the photograph.

## Generate And Inspect

1. Pass every edit target into the built-in image-generation tool. Use local referenced image paths when available; do not rely only on a textual description.
2. Compile a four-paragraph prompt: canvas and geometry; preservation plus transition; derived design plus typography and color; reproduction mood plus avoids.
3. Inspect the actual result at full view and thumbnail scale.
4. Regenerate once with tighter wording if any central check fails: clean divider; isolated panels; lost subject count or relationship; identity drift; unrelated transition; imbalance; disconnected palette; or commercial, glossy, dense, or full-bleed result.
5. If a second result still fails, return the better version and state the limitation.

## Output

Return:

- the generated image or, in Prompt-only Mode, the compiled prompt;
- the exact final prompt;
- the selected recipe in this order: `[layout / transition / derived relation / typography / accent / texture / mood]`;
- photo role and preservation level;
- one short note describing how the photo and design interact;
- one short color rationale naming the chosen strategy, intended emotion, and paper tone;
- the saved file path for generated images.

## Hard Avoids

Avoid straight horizontal splits, rigid upper/lower boxes, empty white separator bands, uniform rectangular photo bottoms, unrelated generic torn-paper effects, top-heavy or bottom-heavy compositions, tiny faint lower ornaments, all contrast concentrated in the photo, oversized typography used as ballast, unexamined source-color copying, arbitrary mood presets, blanket yellow or sepia casts, accidental skin-color shifts, dirty whites, disconnected paper and ink palettes, duplicated people or objects, invented readable personal data, commercial headlines, logos, calls to action, glossy mockups, cinematic depth, 3D, neon, dense scrapbook layouts, and full-screen illustration.
