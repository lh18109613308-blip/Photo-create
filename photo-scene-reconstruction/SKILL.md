---
name: photo-scene-reconstruction
description: Reconstruct a supplied travel, lifestyle, or food photograph into one integrated mixed-media image while preserving its key photographic evidence. Use for photo redesigns that blend local paper, illustration, halftone, collage, negative space, or abstract graphics without replacing the real scene or food.
---

# 照片画面重构

Turn a photograph into one connected photo-and-design composition. Do not make a photo panel with a detached illustration below it.

## Route the image

- **Food mode:** Use this mode when the photograph's main subject is a dish, drink, dessert, ingredient, shared meal, or cooking action. Read [Food Photo Mode](#food-photo-mode) before prompting.
- **General scene mode:** Use the rules below for people, places, objects, and travel or lifestyle scenes. When food and people coexist, protect both: preserve identifiable people under the people rules and preserve the food under Food Photo Mode.

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

## Food Photo Mode

### Read the meal before designing

For food photographs, identify and use these observations before deciding what to retain or transform:

- **Food subject:** the hero dish or drink; its key components, countable garnishes, cut surfaces, plating, vessel, utensils, and any shared or making action.
- **Appetite cues:** steam, melt, gloss, char, crust, crumb, foam, bubbles, sauce viscosity, moisture, grains, and other textures that establish freshness and edibility.
- **Light and table space:** direction and hardness of light, highlight control, depth of field, tabletop or tablecloth material, negative space, and the relationship between plate, hand, glass, and background.
- **Color structure:** ingredient colors, neutrals from plate and table, and the one or two natural accents that can carry local graphics.

### Food preservation map

- Treat the hero dish, drink, and vessel as high-preservation photographic subjects. Keep their edible form, key ingredients, plating geometry, portions, garnish count, utensil placement, and source colors recognizable.
- Preserve food-specific surface evidence: crispness, sear, crumbs, grain, translucency, condensation, bubbles, oil sheen, sauce edges, melt, and steam when present. Do not smooth these away or substitute generic texture.
- Keep original white balance, exposure, saturation, and highlight hierarchy as the baseline in retained food photography. Food must still look freshly photographed, not globally filtered.
- Do not turn food into plastic, toys, clay, a glossy 3D render, or a generic AI dish. Do not invent extra ingredients, duplicate a dish, replace a plate, or change a drink's fill level unless the user explicitly requests it.
- In shared-meal or cooking photographs, preserve the relationship between people, hands, serving tools, and food. Do not add or remove diners, hands, or dishes.

### Food transformation map

Choose one physical food relationship as the visual metaphor. New material must start at a real source feature and return to it; it cannot float as detached restaurant decoration.

- Let **steam** become translucent paper vapor, fine contour lines, or fading halftone, while keeping the real steam visible near the dish.
- Let a **sauce trail, pour, foam edge, coffee swirl, or noodle path** continue into an aligned route line, color field, or ink gesture.
- Let a **cut face, crust, layered dessert, or ingredient cross-section** open into a small ingredient diagram, collage strata, or printed texture aligned to the real layers.
- Let **spices, seeds, crumbs, herbs, and bubbles** disperse into restrained dot fields or registration marks that remain visibly connected to the source ingredient.
- Let a **plate rim, bowl curve, chopstick, fork, napkin fold, or table edge** begin a local torn-paper seam, drawn contour, or intentional blank space.
- Use paper grain, risograph texture, collage, and illustration only in newly created zones or transition seams. Keep the retained dish photographic and let source colors, rather than preset vintage palettes, lead the additions.

### Food modes

- **Faithful food photography:** Default. Keep the dish and its color/light structure dominant; use only local, restrained transformation around source anchors.
- **Narrative food editorial:** Use when the user asks for a stronger food-story composition. Expand one source relationship into visible paper, diagram, collage, or abstraction while maintaining edible realism and the original color baseline.

Do not default to menu advertising, recipe-card typography, ingredient labels, or a commercial food-delivery layout. Add sparse text only when the user requests it or when a tiny editorial caption improves the requested composition.

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

1. Output ratio and the photo's protected subjects, light, spatial relation, and color baseline. For food, name the hero dish/drink, key food components, plating/vessel, appetite cues, and chosen food mode.
2. Exact retained-photography map and exact transformed-region map.
3. The interaction rule: how each paper, illustration, or abstract element attaches to real features. For food, specify the steam, sauce, cut face, crumb, vessel, or utensil edge that provides the anchor; include sparse text only if useful.
4. Hard avoids: split panels, cutout-subject effect, global recolor, detached decoration, duplicated people or dishes, identity drift, food that looks inedible or synthetic, full redraw, advertising layout, logo, watermark, and unwanted styles.

## Quality Gate

Before returning, confirm:

- The subject, light, space, and color structure remain recognizable.
- At least one substantial region is unmistakably transformed into paper, illustration, blank space, or abstraction; it is not merely a photograph with line overlays.
- The retained photographic areas still look like the original photo and the new materials are local and clearly attached.
- The composition reads as one image, not a top/bottom or side-by-side template.
- For food, the main dish or drink still looks edible, freshly photographed, correctly plated, and materially consistent with the source.
