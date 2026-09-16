# SKILL — CHAT OUTPUT PROTOCOL

## New-session objective

After the repository is read, the agent should be able to proceed without requiring the user to restate the mission.

## When user says only “lee este repo”

The agent should:

1. acknowledge that the operating system has been loaded;
2. state the current verified Adobe baseline only if useful;
3. run current-demand research when web access exists;
4. choose a concept using the opportunity-selection engine;
5. explain the selected concept and evidence briefly;
6. create the professional brief and image-generation prompt;
7. if an image-generation capability is available, generate the asset;
8. inspect/review the resulting image using the QC skill;
9. regenerate or fix when necessary;
10. upscale/export when required to meet the final-file gate;
11. verify the exact downloadable file;
12. prepare technical specs, metadata, disclosure and license evidence;
13. output the final decision and audit trail.

## One-command follow-up mode

After an image run, these short user commands are complete instructions:

- `otra imagen`
- `otra`
- `siguiente imagen`
- `next image`
- `haceme otra`

Do not ask the user to repeat the mission, Adobe requirements, resolution target or metadata requirements.

Each command starts a **new independent production run** unless the user explicitly asks to continue the same subject or series.

### Mandatory novelty behavior

By default, the next image must be **genuinely different from the immediately previous image**, not merely a new action performed by the same subject.

The agent must:

1. read the previous run's exclusion fingerprint;
2. perform fresh opportunity research when web access exists;
3. build a new candidate pool;
4. prefer a different category/family from the immediately previous image;
5. require a different primary subject or subject class;
6. require a different buyer/use case and scenario when practical;
7. reject candidates that are only prompt edits or action changes;
8. run the `DIFFERENT-CONCEPT GATE` before generation.

A candidate is not sufficiently new when it keeps the same primary subject and category, even if the subject is doing a different activity.

Example:

`person lifting weights in a gym` → `same person stretching in the gym` = **REJECT AS NOT NEW**.

`person lifting weights in a gym` → `artisan bread preparation in a modern bakery for food-brand editorial use` = **NEW CONCEPT**.

A category change is the default diversification mechanism. Reusing the previous category requires a documented evidence-based exception, not convenience or prompt similarity.

Do not use artificial category rotation when research strongly supports a distinct opportunity, but never weaken novelty merely to make generation easier.

## Mandatory final package for every generated image

When the image was actually generated and the final file is verified, return:

1. **Image / final file** — the exact downloadable asset.
2. **Resolution** — exact width × height and megapixels.
3. **Technical export** — JPEG, sRGB and exact file size when verified.
4. **Title** — the final English Adobe Stock title.
5. **Keywords** — prioritized, truthful keywords derived from the actual image.
6. **Category** — category matching the visual content.
7. **Generative AI disclosure** — the applicable Adobe portal setting.
8. **Releases** — model/property release status when applicable.
9. **Final state** — one of the repository's allowed states.

## Resolution rule

A photo is not complete just because a generation preview exists.

The final downloadable file must pass `rules/OUTPUT_DELIVERY_GATE.md`. The current Adobe baseline is 4–100 MP, with JPEG/sRGB and a maximum 45 MB file size; re-check the official Adobe source before production because requirements can change.

`4 MP` means at least four megapixels, not four megabytes. Do not downgrade a clean larger image merely to reach exactly 4 MP. When the toolchain supports it without quality loss, a larger clean final such as 12–24 MP is preferable.

If the source is below 4 MP, use an appropriate licensed/commercially permitted upscale or generation method and inspect the post-upscale file at 100%. If the environment cannot produce or verify the final file, do not label it `READY_TO_UPLOAD`.

## Metadata rule

Metadata must be generated **after** the final image is selected, not from the prompt alone.

Titles and keywords must describe the actual visible content. The title should be concise and natural in the account's language; keywords must be prioritized by importance and contain no irrelevant SEO bait or prohibited IP references.

Adobe's current guidance says titles should be brief and clear, ideally under 70 characters, and that keyword order matters; it currently allows up to 49 keywords per submission. These are current-source facts and must be refreshed when Adobe changes its metadata guidance.

## Do not

- ask “what image do you want?” unless the repository workflow specifically requires a user-selected subject;
- ask the user to explain Adobe rules already present in the repo;
- invent a trending topic;
- call an asset “approved” before Adobe moderation;
- stop after writing a prompt when the environment can also generate/review the image;
- call a low-resolution preview the final file;
- claim an upscale, 100% inspection, metadata extraction or export verification that did not actually happen;
- satisfy `otra imagen` by changing only the activity, pose, color, crop, angle, lighting, outfit, prop or wording of the previous concept.

## If web access is unavailable

Use the repository's last verified baseline, label current-demand claims as `UNKNOWN`, and avoid pretending that the latest marketplace demand is known.

## If image-generation capability is unavailable

Provide the complete production-ready prompt, negative constraints, QC checklist and metadata plan, but do not claim that the image was generated or inspected.
