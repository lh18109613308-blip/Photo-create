---
name: photo-scene-reconstruction
description: Reconstruct a supplied travel or lifestyle photograph into one integrated mixed-media image by preserving key people and photographic evidence while selectively transforming scene regions into handmade paper, illustration, halftone, collage, negative space, or abstract graphics. Use when a user asks to redesign, second-create, recompose, or blend a photo with paper/illustration/design elements, especially for travel posters, zines, editorial images, and image-to-image edits.
---

# 照片画面重构

Turn a photograph into one connected photo-and-design composition. Do not make a photo panel with a detached illustration below it.

## Workflow

1. Inspect every input image first. Treat the photo as an edit target unless the user explicitly says it is only a reference.
2. Before designing, report or use these four observations:
   - **Subject:** people, key objects, their count, identity-sensitive details, poses, gaze, gestures, clothing, held objects, and interaction.
   - **Light and mood:** direction, softness, weather, contrast, emotional temperature.
   - **Spatial relation:** foreground/background layers, framing shapes, scale, sightlines, gaps, and directional movement.
   - **Color structure:** dominant colors, neutral supports, accents, and cool/warm balance.
3. Declare a preservation map and a transformation map. State exactly which regions remain real photography and which become paper, illustration, blank space, or abstract graphics.
4. Build one visual metaphor from an actual relationship in the photo. Anchor every new graphic element to a real edge, gesture, object, shadow, or meaningful gap.
5. Use the built-in image-generation tool with the supplied image. Inspect the output and regenerate once only if a protected person, object, color baseline, or required material transformation drifts.

## Preservation Rules

- Use **high preservation** for identifiable people. Preserve identity, face, body proportions, pose, clothing, held objects, count, placement, and relationships.
- For one or two people, treat the relation between them as a subject: facing, following, shared object, gaze, distance, gesture, or movement must remain legible.
- Never merge, add, delete, generically silhouette, or duplicate people. Do not hide a face with graphic treatment.
- Preserve the original photographic color grade, white balance, exposure, contrast hierarchy, and natural saturation in retained photo regions.
- Never apply a global yellow-paper, ivory, sepia, monochrome, faded-film, or unified texture overlay unless the user explicitly requests it.

## Transformation Rules

Choose transformed regions from the source composition; do not decorate empty space arbitrarily.

- **Paper / negative space:** Replace a noncritical background region with handmade paper only when a torn edge can begin at a real scene contour. Keep it local, not full-frame.
- **Illustration:** Continue a real silhouette, crack, branch, architectural edge, garment edge, or object geometry into ink, cut-paper, watercolor, collage, or linocut form with precise alignment.
- **Abstract graphics:** Let diagrams, contour lines, halftone, color fields, or registration marks originate from a lens, hand gesture, path, shadow, gaze, object, or space between subjects.
- **Material contrast:** Make the retained photo, paper, illustration, and blank space visibly distinct. Use print grain only in newly created regions or transition seams, never as a global filter.
- Use colors sampled from the photo. Keep new accents subordinate unless a source accent naturally supports the concept.

## Prompt Contract

Write the final image prompt in four compact parts:

1. Output ratio and the photo's protected subjects, light, spatial relation, and color baseline.
2. Exact retained-photography map and exact transformed-region map.
3. The interaction rule: how each paper, illustration, or abstract element attaches to real features; include sparse text only if useful.
4. Hard avoids: split panels, cutout-subject effect, global recolor, detached decoration, duplicated people, identity drift, full redraw, advertising layout, logo, watermark, and unwanted styles.

## Quality Gate

Before returning, confirm:

- The subject, light, space, and color structure remain recognizable.
- At least one substantial region is unmistakably transformed into paper, illustration, blank space, or abstraction; it is not merely a photograph with line overlays.
- The retained photographic areas still look like the original photo and the new materials are local and clearly attached.
- The composition reads as one image, not a top/bottom or side-by-side template.
