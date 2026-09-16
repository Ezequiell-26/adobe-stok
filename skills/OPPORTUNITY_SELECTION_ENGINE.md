# OPPORTUNITY SELECTION ENGINE — Adobe Stock

## Purpose

This skill prevents the agent from treating one category, trend, subject, or visual style as the default answer to a generic request such as “create an image”.

The agent must select **an opportunity**, not a favorite topic.

A trend mention is evidence, not an instruction.

## Core rule

**No category is privileged.**

Fitness, wellness, business, technology, food, travel, sustainability, family, education, finance, lifestyle, culture, science, healthcare, home, industry and other categories must compete on current evidence and commercial utility.

The fact that Adobe currently highlights a theme does **not** mean it is the highest-demand category, the best category for the contributor, the least saturated opportunity, or something that should be generated automatically.

## Generic-request protocol

When the user asks for a generic image without specifying a subject:

1. Perform current research when web access exists.
2. Extract multiple independent market signals across different categories.
3. Build a candidate pool of at least 5 materially different concepts when enough evidence exists.
4. Include at least 3 distinct category families unless the available evidence makes this impossible.
5. Do not add fitness merely because it appears in a current Adobe trend source.
6. Compare candidates before generation.
7. Reject any candidate whose only justification is “it is trending”.
8. Select the concept with the strongest combined opportunity profile.

## Candidate dimensions

For each candidate, evaluate qualitatively:

- `DEMAND_SIGNAL` — strength and recency of verifiable demand evidence;
- `BUYER_UTILITY` — number and quality of concrete buyer use cases;
- `SEARCH_CLARITY` — how clearly the visual maps to searchable intent;
- `DIFFERENTIATION_GAP` — whether there is a meaningful angle beyond generic stock;
- `SATURATION_RISK` — likelihood of severe competition/near-duplicate supply;
- `SEASONAL_FIT` — usefulness for the current production window;
- `PORTFOLIO_GAP` — value relative to the contributor's own existing work, when known;
- `PRODUCTION_RELIABILITY` — ability to produce a clean, professional asset with the available generator;
- `LEGAL_COMPLEXITY` — expected rights/IP/release burden;
- `QC_RISK` — expected anatomy, geometry, text, physics or other generation failure risk;
- `MULTI_USE_VALUE` — ability to serve multiple legitimate commercial contexts without becoming generic.

Do not convert these dimensions into claims about sales probability or Adobe acceptance probability.

## Evidence hierarchy

### A. Official platform signal
Current Adobe Stock contributor guidance, official trend pages, collections, missions/briefs, policy changes, or directly relevant official documentation.

### B. Marketplace/buyer signal
Current Adobe search/category/collection observations and reputable current industry or buyer research.

### C. Portfolio evidence
The contributor's own measured outcomes, only when actual exposure and observation windows are available.

### D. Commercial hypothesis
A reasoned inference from a buyer use case, design workflow, seasonal need, or content gap.

A candidate must clearly separate A/B/C evidence from D inference.

## Anti-bias rules

The agent must explicitly run a **category-bias check** before selection.

Ask:

- Did I choose this category because it has stronger evidence, or because it was mentioned repeatedly in the repository?
- Would the same category still win if every current trend mention of that category were removed?
- Did another category have similar demand but materially better differentiation or lower saturation?
- Am I confusing cultural relevance with marketplace demand?
- Am I confusing buyer utility with likely sales?
- Am I using a repository snapshot as if it were a current ranking?

If the answer indicates repository-induced bias, rerun candidate selection.

## Fitness-specific rule

Fitness is a valid commercial category, but it has no privileged status.

Only choose fitness when current evidence and candidate comparison support a concrete opportunity, such as a differentiated context, buyer use case, demographic/business need, seasonal need, or portfolio gap.

Reject generic concepts justified only by statements such as:

- “fitness is trending”;
- “Gen Z likes fitness”;
- “health and wellness sells”;
- “gym photos are popular”.

These are insufficient on their own.

## Saturation test

Before generating a familiar stock concept, identify whether the concept is likely to be crowded.

High-saturation examples include generic:

- person lifting weights in a gym;
- smiling business team around a laptop;
- generic handshake;
- generic salad/healthy food composition;
- generic smartphone held in hand;
- generic AI robot/brain imagery;
- generic office desk with coffee;
- generic travel landmark postcard composition.

These concepts are not automatically forbidden. They require a stronger differentiation gap and a clearer buyer use case.

## Selection output

Before generation, the agent must produce an internal decision record with:

```text
CATEGORY_POOL:
CANDIDATES:
TOP_SIGNAL:
TOP_BUYER_USE_CASE:
SATURATION_RISK:
DIFFERENTIATION_GAP:
PORTFOLIO_GAP:
PRODUCTION_RISK:
LEGAL_RISK:
CATEGORY_BIAS_CHECK:
FINAL_CONCEPT:
WHY_THIS_CONCEPT:
WHY_NOT_THE_OBVIOUS_ALTERNATIVES:
EVIDENCE_STATUS:
```

`WHY_THIS_CONCEPT` must refer to evidence and commercial utility, not taste.

## No forced diversity

The system must not rotate categories artificially just to appear diverse.

It is acceptable to select the same category repeatedly when independent current evidence supports distinct opportunities. The requirement is **competition between opportunities**, not arbitrary topic rotation.

## No fabricated market intelligence

Never invent search volume, download volume, revenue, bestseller status, ranking, conversion rate, buyer preference statistics, or “most requested” claims.

When evidence is unavailable, label the relevant field `UNKNOWN`.

## Freshness

Demand is time-sensitive. Re-run research for each production run when web access exists.

Historical trend snapshots are retained for context only. They cannot override newer evidence.

## Final principle

The correct generic request behavior is:

`RESEARCH → DIVERSE OPPORTUNITY POOL → BUYER USE CASE → SATURATION/GAP → CANDIDATE COMPARISON → BIAS CHECK → CONCEPT GATE → GENERATION`

Not:

`SEE TREND → PICK TREND → GENERATE`
