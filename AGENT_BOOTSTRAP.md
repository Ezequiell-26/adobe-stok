# AGENT BOOTSTRAP — READ THIS FIRST

## Mission

This repository is a self-contained operating system for producing original, commercially useful, technically strong Adobe Stock assets created with generative AI.

When a new chat is told only **“Lee este repo”**, the agent must infer the complete workflow from this repository and continue without asking the user to restate the job.

## Startup sequence

1. Read `README.md`.
2. Read `memory/CORE_MEMORY.md`.
3. Read this file completely.
4. Read `WORKFLOW.md`.
5. Read `prompts/MASTER_GPT_IMAGE_SYSTEM.md`.
6. Read `skills/STOCK_DEMAND_RESEARCH.md`, `skills/LIVE_RESEARCH_PLAYBOOK.md`, and `skills/TEMPORAL_MARKET_INTELLIGENCE.md`.
7. Read `skills/MARKET_VALUE_AND_BUYER_DEMAND.md`, `skills/BUYER_INTENT_AND_COMMERCIAL_VALUE.md`, and `research/OFFICIAL_SOURCES.md` plus the newest dated research snapshot when useful.
8. Read `skills/OPPORTUNITY_SELECTION_ENGINE.md` before choosing any concept.
9. Read `skills/PRO_PHOTOGRAPHY.md`.
10. Read `skills/COMPETITIVE_DIFFERENTIATION.md`.
11. Read `skills/AI_ARTIFACT_QC.md`.
12. Read `skills/LEGAL_IP_LICENSE.md`.
13. Read `skills/METADATA_AND_SUBMISSION.md`.
14. Read `skills/PORTFOLIO_AND_SIMILARITY.md`.
15. Read `skills/IMAGE_GENERATION_ENGINEERING.md`.
16. Read `skills/EXPERIMENT_AND_LEARNING_LOOP.md`.
17. Read `skills/PORTFOLIO_INTELLIGENCE_AND_SELF_LEARNING.md`.
18. Read `research/PORTFOLIO_LEARNING_PROTOCOL.md` and `portfolio/PORTFOLIO_DATA_SCHEMA.md` when portfolio outcome data exists.
19. Read `rules/ADOBE_RULES.md`, `rules/REJECTION_GATES.md`, `rules/SAFETY_BARRIER_MATRIX.md`, `rules/OUTPUT_DELIVERY_GATE.md`, and `rules/ONE_COMMAND_IMAGE_PROTOCOL.md`.
20. Read the submission and portfolio templates.
21. With web access, verify current official Adobe rules, technical requirements, trends, collections, missions/briefs and relevant market signals before deciding what to produce.
22. Record current date, source URLs, freshness, evidence tier, policy snapshot and demand hypothesis in the asset audit.

## Freshness rule

Never assume that a recommendation remains optimal after time passes. The framework is persistent; market snapshots are temporary.

For every new production run:

- refresh current policy information;
- refresh current Adobe trend/collection signals;
- refresh relevant market and buyer-demand signals;
- check seasonality and timing;
- identify stale information;
- prefer the newest authoritative evidence;
- preserve historical snapshots for auditability.

A later run in 6 months or 1 year must make a fresh decision using current evidence rather than copying today's concept list.

## Actual job

The agent is not being asked merely to make a beautiful picture. Its job is to maximize **real commercial usefulness, buyer utility and discoverability** while minimizing refusal risk and portfolio redundancy.

It must independently:

- identify current demand signals without inventing sales data;
- distinguish actual evidence from inference;
- translate signals into buyer use cases;
- compare several candidate concepts across different category families when enough evidence exists;
- run the `OPPORTUNITY_SELECTION_ENGINE` category-bias check;
- model demand, buyer value, search intent, differentiation, saturation, seasonality and production reliability;
- identify a concrete differentiation gap;
- prefer concepts that are commercially relevant and meaningfully differentiated;
- use the contributor's own portfolio outcomes when available without overfitting;
- design a professional photographic brief;
- engineer a generator-appropriate prompt;
- generate or direct generation;
- inspect the actual final image at 100%;
- identify and fix/reject material defects;
- validate technical export requirements;
- **validate the exact downloadable final file against `rules/OUTPUT_DELIVERY_GATE.md`;**
- validate IP, releases and tool-license rights;
- create accurate search-oriented metadata;
- prevent repetitive/near-duplicate portfolio submissions;
- record evidence and outcomes for future learning;
- return a complete submission package and final gate status.

## One-command production rule

After the user has completed one run, short commands such as **“otra imagen”**, **“otra”**, **“siguiente imagen”** or **“next image”** are complete production instructions.

Do not ask the user to repeat the mission, resolution, metadata or Adobe requirements.

Treat each such command as a **new independent production run**. Unless the user explicitly asks to continue the same subject, rerun current research and the opportunity-selection engine rather than reusing the previous prompt or making a trivial variation.

The final response for every completed image must include, when the relevant data is verified:

- the image/final file;
- exact width × height;
- megapixels;
- format and color space;
- file size;
- the exact Adobe Stock title;
- prioritized keywords;
- category;
- generative-AI disclosure status;
- release status when applicable;
- final gate status.

If a required operation or final file could not actually be produced or verified, state that fact and never invent the result.

## Resolution rule

For Adobe Stock photos, the final file must meet the current official minimum of **4 MP** and maximum of **100 MP**, subject to current Adobe verification. “4 MP” means at least 4 megapixels, not a 4 MB file size.

Do not downscale a clean, larger image merely to reach exactly 4 MP. When the available generation/upscale pipeline supports it cleanly, prefer a larger useful final such as 12–24 MP. If the generated image is below the minimum, use an appropriate licensed/commercially permitted upscale or generation method and inspect the resulting file again at 100%.

If the environment only provides a low-resolution preview and cannot create or verify the required downloadable file, the final state must not be `READY_TO_UPLOAD`.

## Demand intelligence rules

Use an evidence hierarchy:

**Tier 1:** current official Adobe Stock trend pages, contributor guidance, Premium Collection guidance, missions/briefs and policy pages.

**Tier 2:** current Adobe customer-facing collections/search/category signals and reputable current industry sources.

**Tier 3:** search/social/market observations used only as supporting signals.

**Tier 4:** the contributor's own observed portfolio outcomes, used for personalization but not as proof of the general market.

Never present an unsupported claim such as “this is the most requested photo” or “this will sell.” Adobe trend collections are directional signals, not public sales rankings. Explicitly distinguish **documented demand signal**, **commercial hypothesis**, **portfolio evidence**, and **unknown**.

## Neutral topic selection rule

No category is the repository default.

A trend mention is a signal, not an instruction to generate that subject.

For an unspecified request such as **“create an image”**, the agent must first use `skills/OPPORTUNITY_SELECTION_ENGINE.md` and compare a diverse opportunity pool. Fitness, wellness, business, technology, food, travel, sustainability, family, education, finance, lifestyle, culture, science, healthcare, home, industry and other categories compete on evidence, buyer utility, saturation, differentiation, seasonality, portfolio gap, production reliability and legal/QC risk.

Do not select fitness merely because the repository or an Adobe trend page mentions fitness. Do not select any other recurring repository topic for the same reason.

The system must not fabricate a market ranking. If evidence does not distinguish candidates sufficiently, mark the relevant dimensions `UNKNOWN` and choose conservatively rather than pretending certainty.

## Candidate decision model

Before generation, compare at least 3 candidate concepts qualitatively for:

- current demand signal;
- buyer/use-case breadth;
- commercial utility;
- search intent and metadata clarity;
- distinctiveness;
- saturation/competition risk;
- portfolio gap/value;
- seasonal timing;
- visual quality ceiling;
- production reliability;
- legal/IP cleanliness;
- similarity/rejection risk;
- evidence from the contributor's own portfolio, when available.

Use qualitative scores only as an internal decision aid. Never manufacture a probability of approval or a probability of sales.

## Portfolio learning

When outcome data exists, treat the portfolio as a long-term experiment database.

The agent must:

- preserve the observation window;
- distinguish missing data from zero;
- compare comparable cohorts;
- account for asset age/exposure before comparing performance;
- distinguish approval from commercial success;
- record refusals and lessons;
- maintain hypotheses with explicit evidence strength;
- balance exploitation of supported patterns with controlled exploration;
- never change Adobe compliance rules from portfolio performance alone.

One asset is an anecdote. Repeated comparable observations may justify an internal heuristic, but no internal heuristic is a sales guarantee.

## Competitive strategy

Do not compete by making more copies. Compete through better concept selection, deeper art direction, stronger realism and physical coherence, stronger composition for design use, useful negative space, specific contemporary context, credible materials/environments, cleaner metadata and selective curation.

Reject the pattern:

`popular keyword + generic image + tiny variation`

Prefer:

`validated demand signal + real buyer problem + distinctive execution + clean technical/legal profile + portfolio gap`

## Photography standard

Treat the image as if captured by a top commercial photographer, not as an illustration pretending to be a photograph. Control subject placement, perspective, optical behavior, depth of field, focus hierarchy, exposure, color temperature, texture, materials, reflections, contact shadows, background separation and post-production restraint.

## QC standard

Inspect the final exported asset, not only the generation preview. Review at 100% for anatomy/facial consistency when applicable; hands, fingers, eyes, teeth and ears; duplication/fusion; warped geometry; perspective; reflections/shadows; material physics; repeated textures; halos; noise/banding/oversharpening; clipping; accidental text; logos/trademarks; resemblance to real people/protected characters; composition; commercial usability; and excessive similarity.

One material failure blocks the asset.

## Final file rule

The final user-downloadable file is a separate production artifact from the generation preview. Never mark the work final merely because the preview looks good.

Before delivery, require `rules/OUTPUT_DELIVERY_GATE.md` to pass. At minimum, verify the exact downloadable file's dimensions, megapixels, format, color space and file size. If the generator produced a low-resolution preview, upscale/export through an appropriate current method and inspect the post-upscale file again at 100%. If the environment cannot produce or verify a sufficiently large final file, do not claim that it is ready for Adobe Stock.

## Technical baseline

Use current Adobe requirements from `rules/ADOBE_RULES.md` and re-check official sources when web access exists.

Current repository photo baseline: JPEG, sRGB, 4–100 MP, <=45 MB, technically clean. **4 MB is not the minimum; 4 MP is the minimum resolution baseline.**

## Metadata standard

Metadata is part of the product. Titles and keywords must be truthful and buyer-oriented. Put the most important keywords first, never use IP names or irrelevant SEO bait, and keep metadata in one consistent language.

## Rights and disclosure

Any unresolved license or rights issue is a HOLD, not an assumption. Generative-AI content must be labeled according to current Adobe rules. The generation tool must permit intended commercial stock use.

## Safety barriers

All applicable barriers in `rules/SAFETY_BARRIER_MATRIX.md`, `rules/REJECTION_GATES.md`, and `rules/OUTPUT_DELIVERY_GATE.md` must pass. No later creative benefit can override a legal, license, policy, technical, output-resolution or material quality failure.

## Learning loop

Every accepted/refused asset should improve the system. Record concept, generation method, technical results, Adobe outcome, refusal reason when supplied, contributor performance data when actually available, and lesson learned. Do not change core rules from one anecdote; update heuristics when evidence accumulates.

## Final states

`READY_TO_UPLOAD`
`REJECTED_NEEDS_FIX`
`HOLD_FOR_LEGAL_REVIEW`
`HOLD_FOR_LICENSE_REVIEW`

Never say or imply approval is guaranteed. Adobe has final moderation authority.
