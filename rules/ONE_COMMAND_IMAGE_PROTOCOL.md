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

It must not simply regenerate the previous prompt or create a trivial variation.

Required sequence:

`NEW RESEARCH → NEW OPPORTUNITY SELECTION → NEW CONCEPT → NEW PHOTO BRIEF → GENERATE → SELECT/CURATE → UPSCALE/EXPORT → OUTPUT DELIVERY GATE → 100% QC → METADATA → LEGAL/LICENSE → PORTFOLIO/SIMILARITY → FINAL RESPONSE`

## New opportunity requirement

Unless the user explicitly asks to continue the same subject, the next image should be selected from the current opportunity pool again.

The agent may choose the same category again only when current evidence and the new concept justify it. It must not default to fitness, wellness, business, technology, travel, or any other recurring repository topic.

Avoid trivial changes such as:

- same scene with a different color;
- tiny crop;
- horizontal/vertical flip;
- minor camera shift;
- superficial prop replacement;
- nearly identical prompt wording.

A new image should represent a materially different concept, buyer use case, context, visual narrative, subject relationship or composition.

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

Adobe currently states that keyword order matters and allows up to 49 keywords per content submission; because metadata rules can change, verify current official guidance during fresh research. citeturn772465search0

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

Adobe's current public guidance says photos must be 4–100 MP, JPEG, sRGB and no larger than 45 MB; larger files can provide customers greater flexibility. citeturn772465search3

Adobe's current generative-AI guidance also requires the content to be marked as generated with AI when applicable, and titles/keywords must not contain prohibited references such as real people, artists, fictional characters, government agencies, or third-party IP. citeturn772465search1turn772465search2

These official sources are verification references, not permanent hard-coded facts. Re-check them when producing new assets.
