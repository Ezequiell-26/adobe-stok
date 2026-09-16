# IMAGE GENERATION ENGINEERING

## Goal

Translate the commercial concept into a robust image-generation specification that minimizes common generative failures and produces a credible professional-photography result.

## Prompt architecture

Build prompts in this order:

1. commercial concept;
2. subject and action/state;
3. environment/context;
4. composition and spatial relationships;
5. camera perspective and framing;
6. light direction and quality;
7. material/physics requirements;
8. texture and realism requirements;
9. color and tonal direction;
10. copy-space requirement when useful;
11. quality constraints;
12. prohibited elements.

## Do not prompt by adjective stacking

Avoid long strings of vague quality adjectives such as “ultra amazing perfect masterpiece” without photographic meaning. Use concrete visual instructions instead: controlled perspective, natural skin texture, physically coherent reflections, realistic contact shadows, restrained dynamic range, etc.

## Reliability-first design

When a concept contains high-risk details, reduce unnecessary complexity. Fewer important objects with correct geometry are preferable to a crowded scene with many failure points.

For people, control pose, hand visibility and interaction carefully. For products, control surfaces, contact points, reflections and labels. For glass/liquid, control transparency, refraction, fluid level, condensation, ice and foam.

## Composition engineering

Design for multiple crops when possible. Keep the primary subject clearly separated from the background. Reserve intentional negative space when a buyer may need text placement. Do not add empty space merely to satisfy a template.

## Generator-specific settings

Use the currently selected image generator's current official documentation when settings matter. Never invent unsupported model parameters. Record model/version, settings, seed if available, upscale method and post-processing used.

## Regeneration policy

If QC finds a material defect, regenerate or retouch only after identifying the failure mode. Avoid random prompt changes. Maintain a short revision log so the system learns which interventions improve the defect.
