# ONE-COMMAND IMAGE PROTOCOL

## Purpose

This protocol defines the behavior for short follow-up commands such as:

- `otra imagen`
- `otra`
- `siguiente imagen`
- `next image`
- `haceme otra`

The user does not need to repeat the stock-production instructions.

## One-command contract

When the user asks for another image after a completed production run, the agent must execute a **new independent production run** using the repository workflow.

It must not simply regenerate the previous prompt, change the action of the same subject, or create a trivial variation.

Required sequence:

`NEW RESEARCH → NEW OPPORTUNITY SELECTION → NEW CONCEPT → DIFFERENT-CONCEPT GATE → NEW PHOTO BRIEF → GENERATE → SELECT/CURATE → UPSCALE/EXPORT → OUTPUT DELIVERY GATE → 100% QC → METADATA → LEGAL/LICENSE → PORTFOLIO/SIMILARITY → FINAL RESPONSE`

## Hard novelty rule

For the default interpretation of **`otra imagen`**, the next asset must be **materially different from the immediately previous asset at the concept level**.

A material difference normally requires at least **three major dimensions** to change, including:

- primary subject or subject class;
- category/family of opportunity;
- buyer problem/use case;
- scenario/context/environment;
- visual narrative/action;
- composition/layout;
- subject-object relationship;
- geographic/cultural context when genuinely relevant.

At least **one of the three changes must be the primary subject or subject class**, unless the user explicitly requests a series in the same subject.

### Strong default: change category

Unless the user says otherwise, `otra imagen` should normally move to a **different opportunity category/family** from the previous image.

Examples of category-family changes:

- fitness → food;
- business → travel;
- technology → family/lifestyle;
- wellness → sustainability;
- finance → home/interiors;
- education → industry/science.

Changing category is a default diversification mechanism, not a forced forever-rotation. The current opportunity research can override it only when there is a strong evidence-based reason, and the agent must document that exception.

## Explicitly forbidden as `otra imagen`

Do **not** satisfy `otra imagen` with:

- the same person doing a different exercise;
- the same product in another position;
- the same room with different props;
- the same scene with a new color palette;
- the same subject at another camera angle;
- a horizontal/vertical flip;
- a crop or zoom change;
- a small lighting change;
- a different outfit on the same subject;
- a superficial prop replacement;
- a different expression from the same underlying portrait;
- a near-identical prompt with one noun or verb changed.

A different action alone is **not** a different concept.

Example:

`person lifting weights → person stretching in the same gym` = **NOT A NEW CONCEPT**.

`person lifting weights → close-up of sustainable meal-prep packaging for a meal-delivery campaign` = **NEW CONCEPT**.

## Previous-output exclusion lock

For each completed run, record a compact exclusion fingerprint containing:

`CATEGORY | PRIMARY SUBJECT | BUYER USE CASE | SCENARIO | VISUAL NARRATIVE | COMPOSITION | KEY OBJECTS`

For the next `otra imagen`, compare every candidate against the immediately previous fingerprint before generation.

If a candidate shares the same primary subject **and** same category, reject it by default.

If it shares three or more major dimensions with the previous asset, reject it as insufficiently different.

If all viable candidates remain too similar, rerun opportunity research rather than weakening the novelty requirement.

## New opportunity requirement

Unless the user explicitly asks to continue the same subject/series, the next image should be selected from the current opportunity pool again.

The agent must first look for materially different opportunities. It may reuse a category only as an exception when current evidence and the new concept justify it; it must not reuse the previous concept merely because it was easy to generate.

It must not default to fitness, wellness, business, technology, travel, or any other recurring repository topic.

## Research requirement for `otra imagen`

`Otra imagen` is **not** a shortcut that skips research.

When web access exists, perform fresh current-demand research and build a new candidate pool. Use the previous asset only as an exclusion reference, not as an inspiration template.

The previous image may inform what to avoid, not what to copy.

## Resolution and final-file contract

The image is not complete when the generation preview exists.

The agent must produce or verify a downloadable final asset that satisfies `rules/OUTPUT_DELIVERY_GATE.md`.

For photos, the current Adobe baseline is **4 MP minimum and 100 MP maximum**, with JPEG/sRGB and a maximum file size of 45 MB; these requirements must be rechecked against current official Adobe documentation when web access exists.

### Important 4 MP rule

The user's request for “4 MP” means **at least 4 megapixels**, not “4 MB”.

Do not intentionally downgrade a clean larger image to exactly 4 MP. Prefer the highest clean, useful resolution available within Adobe's current limits. A practical target of 12–24 MP or higher may be used when the generation/upscale pipeline supports it without introducing artifacts.

Examples:

- 1024×1024 = about 1.05 MP → BLOCK.
- 1536×1024 = about 1.57 MP → BLOCK.
- 2048×2048 = about 4.19 MP → passes the 4 MP minimum if quality is clean.
- 3000×3000 = 9 MP → passes the resolution minimum.
- 4000×3000 = 12 MP → strong practical target.
- 6000×4000 = 24 MP → strong practical target.

If the source is below 4 MP:

1. use an appropriate commercial/licensed upscaling or generation method;
2. reach a clean resolution of at least 4 MP;
3. inspect the post-upscale image at 100%;
4. reject it if upscaling introduces visible artifacts or insufficient detail;
5. never claim a high-resolution final if the exact downloadable file was not produced or verified.

If the environment cannot produce the required final file, the agent must return a non-ready status and clearly state that the available preview is not the final Adobe-ready asset.

## Metadata contract

After creating the image, the agent must always return:

**TITLE**

A concise, accurate English title describing the actual main subject and context. Keep within Adobe's current guidance and do not include “generative AI”, technical prompt parameters, IP names, artist names, real-person names or fictional-character names.

**KEYWORDS**

A prioritized list of truthful, relevant keywords based only on the actual image. Do not use SEO bait, trademarks, names of real people, fictional characters, artist names, government agencies, or unsupported concepts.

Adobe currently states that keyword order matters and allows up to 49 keywords per content submission; because metadata rules can change, verify current official guidance during fresh research.

For practical metadata quality, prioritize the most essential visible concepts first and avoid padding the list with irrelevant terms.

## Exact response order for `otra imagen`

The final response should be compact but complete and contain, in this order:

1. **Nueva imagen creada**
2. **Archivo final / resolución:** exact width × height, MP, format, color space, file size when verified
3. **Título:** exact title to use in Adobe Stock
4. **Palabras clave:** prioritized keyword list
5. **Categoría:** selected category
6. **IA generativa:** disclosure status
7. **Releases:** model/property release status when applicable
8. **Estado final:** one of the allowed repository states

The asset itself must be delivered separately from the metadata when the environment supports file delivery.

## No hidden work claim

Do not state that an image was upscaled, inspected at 100%, or exported at 4+ MP unless the operation actually occurred and the resulting file was verified.

## Adobe alignment

These official-source requirements and metadata details are verification references, not permanent hard-coded facts. Re-check them when producing new assets.
