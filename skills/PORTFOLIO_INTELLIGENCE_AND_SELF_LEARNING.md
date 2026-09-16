# PORTFOLIO INTELLIGENCE & SELF-LEARNING ENGINE — Adobe Stock

## Purpose

Turn real portfolio outcomes into evidence that improves future concept selection, production strategy and curation without pretending that a small sample can predict sales.

This module is optional until the contributor has real outcome data, but the agent must be ready to consume it from the first asset.

## Core rule

**Learn from evidence, not from intuition alone.**

The agent must separate:

- observed fact;
- derived metric;
- hypothesis;
- decision rule;
- uncertainty.

Never convert one successful or refused asset into a universal rule.

## Asset identity

Every asset should have a stable `asset_id` and record:

- creation date;
- submission date;
- concept family;
- sub-niche;
- buyer use cases;
- demand signals used;
- seasonality state;
- source URLs checked;
- generator/model;
- model version when available;
- prompt version;
- dimensions / MP / file size;
- title;
- keywords in final order;
- category;
- AI disclosure;
- people/property/release status;
- license evidence;
- portfolio cluster / similarity group;
- Adobe submission result.

## Outcome fields

When available, record only actual observed platform data:

- submitted;
- accepted;
- refused;
- refusal reason;
- impressions / views if exposed by the platform;
- downloads/licenses if exposed;
- revenue/royalties if exposed;
- favorites/save signals if exposed;
- date range covered by metrics;
- exposure age in days.

Never fill unavailable metrics with estimates and never label a guessed number as platform data.

## Derived metrics

The agent may calculate:

### Approval rate
`accepted / submitted`

### Refusal rate
`refused / submitted`

### License rate
`licenses / eligible exposure`

Only calculate when the denominator has a valid definition.

### Revenue per license
`revenue / licenses`

### Revenue per asset
Use only with a clearly defined observation window.

### Time-to-first-license
Days between accepted publication and first observed license.

### Keyword/concept cohort performance
Compare assets grouped by concept family, buyer use case, season, format, or other meaningful cohort when sample size is adequate.

## Statistical discipline

Small samples are unstable.

Minimum operating guidance:

- 1 asset = anecdote;
- 2–4 assets = weak directional evidence;
- 5–9 assets = preliminary cohort signal;
- 10+ comparable assets = useful internal pattern, still not a forecast;
- 20+ comparable assets = stronger basis for a portfolio heuristic.

These thresholds are internal safeguards, not statistical guarantees.

Do not declare a strategy superior from tiny cohorts.

When cohorts differ in age, exposure, category or upload volume, explicitly mark the comparison as confounded.

## Cohort analysis

Prefer comparisons such as:

- same concept family, different execution;
- same buyer use case, different composition;
- portrait vs landscape;
- copy-space vs no-copy-space;
- generic vs context-specific;
- seasonal vs evergreen;
- people vs object-only;
- standard vs premium-oriented;
- different keyword structures;
- different generators where licensing and quality remain comparable.

Do not attribute causality unless the evidence supports it.

## Learning from Adobe refusals

For every refusal, classify:

`quality | technical | AI_artifact | IP/legal | metadata | similarity | release | policy | other`

Then record:

`observed_reason → root-cause hypothesis → corrective action → verification result`

A refusal becomes a permanent rule only when supported by Adobe documentation or repeated evidence.

## Learning from successful assets

A successful asset should not be copied.

Extract abstract characteristics:

- buyer/use case;
- concept clarity;
- composition;
- subject/context combination;
- seasonal timing;
- search intent;
- differentiation mechanism;
- technical quality;
- metadata structure.

Create new concepts that preserve useful principles while remaining materially distinct.

## Portfolio gap detection

The agent should maintain a conceptual map of the portfolio:

`industry × buyer × problem × subject × context × format × season`

Identify:

- high-demand areas with few assets;
- areas with many assets but weak differentiation;
- accepted concepts with insufficient follow-up coverage;
- seasonal gaps before the season begins;
- buyer use cases with no suitable composition;
- metadata/search gaps.

A portfolio gap is an opportunity signal, not proof of demand.

## Exploration vs exploitation

Future concept selection should balance:

**Exploit:** extend patterns supported by meaningful evidence.

**Explore:** test new concepts with plausible commercial value but insufficient evidence.

Recommended internal split:

- 60–80% evidence-backed extensions;
- 20–40% controlled experiments.

Adjust after sufficient portfolio data. Never use this as a promise of performance.

## Experiment registry

Each experiment should define before generation:

- hypothesis;
- variable changed;
- control/reference cohort;
- expected signal;
- success criterion;
- observation window;
- confounders;
- decision after observation.

Example:

`Hypothesis: stronger copy space increases buyer utility for marketing layouts.`

Do not silently change multiple variables and then claim one caused the result.

## Recency weighting

Current market evidence should receive more weight than old market evidence.

For external trends:

- current official source > historical snapshot;
- recent policy > old policy;
- current mission/brief > archived mission;
- current buyer signal > old speculation.

For portfolio outcomes:

Do not erase old data. Keep it for seasonality and longitudinal analysis, but distinguish:

`CURRENT`
`HISTORICAL`
`SEASONAL`
`EXPIRED`

## Seasonal intelligence

Store expected and observed timing for:

- holidays;
- annual business cycles;
- education periods;
- sports seasons;
- travel seasons;
- cultural moments;
- commercial campaigns.

Plan production sufficiently ahead of the expected buying period when evidence suggests lead time matters.

Never invent an exact lead time without evidence.

## Decision memory

Every future recommendation should be traceable to:

`current evidence + portfolio evidence + constraints + hypothesis`

Record why a concept was selected and why alternatives were rejected.

## Anti-self-deception safeguards

The agent must not:

- confuse acceptance with commercial success;
- confuse downloads with lifetime value without a defined window;
- compare new assets with old assets without considering exposure time;
- treat missing data as zero;
- infer demand from a single customer inquiry;
- infer algorithm changes without platform evidence;
- claim causality from correlation alone;
- optimize only for approval rate at the expense of buyer value;
- optimize only for downloads at the expense of legal/quality requirements;
- chase short-lived trends so aggressively that the portfolio loses durable value.

## Output: portfolio intelligence report

For any analysis, return:

1. DATA WINDOW
2. SOURCES
3. OBSERVED FACTS
4. DERIVED METRICS
5. TOP REPEATED PATTERNS
6. WEAK / UNCERTAIN SIGNALS
7. PORTFOLIO GAPS
8. TESTS TO RUN
9. RULES TO KEEP
10. RULES TO RETIRE
11. NEXT CONCEPT FAMILIES TO RESEARCH

## Golden rule

The system gets smarter by accumulating **clean evidence and controlled experiments**, not by becoming more confident.
