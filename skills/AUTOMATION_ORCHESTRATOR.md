# AUTOMATION ORCHESTRATOR — Adobe Stock

## Purpose
Turn the repository into a repeatable decision engine rather than a static prompt.

## Trigger
If the user only says "Lee este repo", execute the complete pipeline without asking the user to restate the objective.

## Operating modes

### MODE A — Current opportunity discovery
Use when no subject is supplied.
1. Establish current date/time.
2. Refresh Adobe official policies and current trend/collection/mission signals.
3. Search current buyer/customer needs and relevant industry signals.
4. Identify seasonal timing and lead time.
5. Build at least 5 candidate concepts across different commercial use cases.
6. Eliminate unsafe, generic, saturated, redundant, or difficult-to-produce concepts.
7. Select the concept with the strongest evidence-backed commercial case, not the prettiest concept.

### MODE B — User-specified subject
Keep the subject but optimize the execution, commercial use case, differentiation, safety, quality, and metadata.

### MODE C — Portfolio expansion
Review existing portfolio/submission history supplied by the user. Find gaps rather than generating another near-duplicate.

## Freshness protocol

Never treat a dated research snapshot as permanently current.

- Policy/legal sources: re-check on every production run if web access exists.
- Adobe trends/collections: re-check every run.
- Missions/briefs: re-check every run when accessible.
- Search/market signals: re-check every run for time-sensitive concepts.
- Old snapshots are historical context only.

Every research result must carry:
- checked_at;
- source;
- source_type;
- claim;
- confidence;
- expiration/recheck rule.

## Evidence hierarchy

P0 = official Adobe policy/requirements.
P1 = official Adobe trends, collections, missions, Artist Hub/customer guidance.
P2 = reputable industry/customer/advertising trend sources.
P3 = search/social/community observations.
P4 = agent hypothesis.

Never promote P3/P4 to fact. Never invent sales volume, search volume, conversion rates, or approval probability.

## Commercial opportunity model

For each candidate concept evaluate:
- demand evidence;
- buyer breadth;
- real commercial use cases;
- search-intent clarity;
- seasonality/timing;
- market saturation proxy;
- differentiation gap;
- visual quality ceiling;
- generator reliability;
- production cost/time;
- legal/IP risk;
- portfolio fit;
- potential to create multiple genuinely distinct use cases without spam.

Produce an internal opportunity score and a written rationale. The score is not a probability of sales or approval.

## Buyer simulation

For the selected concept identify 3–5 plausible buyer personas such as:
- advertising/brand designer;
- social media/content team;
- editorial/publisher;
- corporate communications;
- education/wellness/travel/technology buyer when applicable.

For each, answer:
- What would they search?
- What message does the image communicate?
- Where would they place text/copy?
- What crop/orientation do they need?
- Why would this image be more useful than a generic alternative?

## Pre-generation gate

Do not generate until the concept has:
- current evidence;
- buyer use case;
- differentiation rationale;
- technical plan;
- legal/IP clearance plan;
- QC plan.

## Generation strategy

Prefer one strong hero concept plus a small number of genuinely distinct variants only when each has a different use case, composition, context, or buyer need.

Do not generate large batches merely to increase volume.

## Post-generation gate

The first generated output is a candidate, never an automatic submission.

Perform:
1. global visual review;
2. 100% artifact review;
3. technical preflight;
4. legal/IP/release review;
5. commercial-usefulness review;
6. metadata review;
7. similarity review.

Any material failure blocks the asset.

## Self-critique loop

For any failed gate:
- identify exact failure;
- decide whether to edit, regenerate, or abandon the concept;
- do not rationalize defects;
- if regeneration is required, materially change the causal prompt component rather than making cosmetic changes.

Maximum retry policy should prevent endless prompt loops. After repeated failures, abandon or redesign the concept.

## Portfolio intelligence

Maintain a ledger of:
- concept;
- niche;
- visual treatment;
- buyer use cases;
- submitted variants;
- approved/refused outcome;
- refusal reason;
- sales/download data when the user provides it;
- observations.

Use the ledger to avoid repetition and identify under-covered niches.

## Outcome learning

When real Adobe outcomes are supplied, distinguish:
- acceptance signal;
- refusal signal;
- commercial performance signal;
- anecdotal observation.

Do not generalize from one asset. Increase confidence only as evidence accumulates.

## Automation boundary

Automation may prepare and validate assets, research opportunities, generate prompts and metadata, and maintain records.

Do not perform an external upload or account action unless the user explicitly authorizes it and an appropriate integration is available.
