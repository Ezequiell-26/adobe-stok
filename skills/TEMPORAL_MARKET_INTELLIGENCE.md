# Temporal Market Intelligence — Adobe Stock

## Purpose

Prevent the repository from becoming obsolete. The agent must choose concepts using evidence that is current **at the time of each production run**, not by blindly reusing a 2026 snapshot.

## Freshness rule

The repository is a framework, not a frozen market forecast.

Every new production session must determine:

- current date;
- current Adobe Stock generative-AI rules;
- current technical requirements;
- current Adobe trend/collection signals;
- current Adobe contributor guidance and refusal reasons;
- current customer-facing search/collection signals when observable;
- current market/creative-industry signals from reputable sources;
- current saturation/competition signals that can be observed without pretending to have private Adobe sales data.

A source older than 90 days must not be treated as current market evidence when a newer authoritative source is available.

Policy sources are higher priority than market commentary. Current official Adobe information overrides repository notes written in the past.

## Time horizons

Use three horizons when deciding what to create:

### NOW — 0–90 days
Use current Adobe collections, current searches, current campaigns/briefs, seasonal opportunities, and current commercial conversations.

### NEAR — 3–12 months
Identify durable buyer needs that are likely to remain commercially useful beyond a short trend cycle: workplace, health/wellness, technology use, education, accessibility, sustainability, finance, everyday commerce, family/community, food, travel and other broad commercial needs when evidence supports them.

### EVERGREEN — 12+ months
Prefer concepts with persistent business use and strong reuse potential when the opportunity is not dependent on a short-lived meme or fad.

The final concept should normally combine a current signal with durable commercial utility rather than relying on a trend alone.

## Evidence hierarchy

### Tier A — authoritative
- Adobe Stock official trend collections;
- Adobe contributor guidelines;
- Adobe generative-AI rules;
- Adobe Premium Collection guidance;
- Adobe refusal/moderation guidance;
- official Adobe customer-facing search/collection pages;
- official Adobe briefs, missions, or contributor communications when publicly available.

### Tier B — strong external signal
- reputable creative-industry reports;
- major agency/brand creative trend reports;
- established research firms;
- current search-interest or consumer-behavior data with transparent methodology.

### Tier C — weak/supporting signal
- social-media observations;
- forums;
- generic trend articles without methodology;
- individual creator opinions.

Tier C can generate hypotheses but cannot by itself justify a claim of high demand.

## What counts as evidence of market value

Prefer evidence for:

1. a real business communication problem;
2. a recurring buyer use case;
3. a growing or currently emphasized subject;
4. a concept with clear search intent;
5. a visual format that is useful in campaigns, websites, presentations, editorial-layout-like commercial design, packaging mockups where permitted, or other genuine stock use;
6. an underserved combination of subject + audience + context;
7. differentiation that cannot be reduced to a color filter or minor crop.

## What does NOT count

Never assume:

- "many search results" means many sales;
- a trend page is a sales leaderboard;
- a popular social post proves stock demand;
- an attractive image will automatically be licensed;
- a niche is profitable merely because it is unusual;
- more uploads create more revenue;
- AI-generated content has an automatic commercial advantage.

## Candidate market model

For each candidate concept, estimate qualitatively:

`Market Opportunity = Current Signal + Buyer Utility + Search Intent + Reuse Breadth + Timing + Differentiation + Production Reliability - Saturation - Compliance Risk`

Use a transparent qualitative scale such as LOW / MEDIUM / HIGH or 0–10 internally. Do not present the result as a probability of sale or approval.

## Search-intent modeling

Before selecting a concept, answer:

- Who is likely to search for this?
- What business problem are they solving?
- Which visible nouns, actions, settings and demographics describe the image?
- Is the use case broad enough to support multiple industries?
- Could a designer crop or place text over the image?
- Does the image communicate the idea immediately at thumbnail size?

## Saturation strategy

Do not simply chase the most obvious keyword.

When a topic is crowded, look for a **commercially meaningful intersection**:

`high-interest topic + specific buyer + useful context + distinctive art direction`

Examples of useful differentiation dimensions:

- age/life stage;
- profession/industry;
- environment;
- cultural context;
- accessibility;
- social interaction;
- realistic action rather than posed portrait;
- unusual but commercially credible viewpoint;
- copy-space layout;
- macro/medium/wide framing with actual use-case differences.

Do not imitate an existing contributor's composition, portfolio, style, or campaign.

## Seasonal planning

Before production, ask whether timing matters:

- holidays;
- school cycles;
- tax/financial periods;
- sports seasons;
- travel periods;
- health campaigns;
- cultural events;
- product-launch seasons;
- business planning cycles.

Seasonal content should be created early enough to be useful to buyers, but never present generated imagery as authentic documentation of a real news event.

## Drift detection

When current evidence conflicts with repository memory:

1. preserve the historical note for auditability;
2. prioritize the newest authoritative evidence;
3. mark the old heuristic as stale;
4. do not silently merge contradictory facts;
5. record the reason for the decision.

## Required output of each research run

Record:

- `RESEARCH_DATE`
- `POLICY_CHECK_DATE`
- `MARKET_SIGNALS`
- `SOURCE_TIER`
- `CURRENT_DEMAND_HYPOTHESIS`
- `EVERGREEN_VALUE`
- `BUYER_USE_CASES`
- `SATURATION_RISK`
- `DIFFERENTIATION_ANGLE`
- `SEASONALITY`
- `UNKNOWN_OR_UNVERIFIED`
- `CONCEPT_SELECTED`
- `WHY_NOW`
- `SOURCES`

This turns the system into a time-aware decision engine instead of a static prompt library.
