# PORTFOLIO LEARNING PROTOCOL

## Purpose

Define how a future GPT should use the contributor's own portfolio data to improve concept selection over time.

## Data priority

When deciding what to create:

1. current official Adobe rules;
2. current official Adobe demand/trend/mission signals;
3. current portfolio performance with a defined observation window;
4. historical portfolio performance for seasonality/context;
5. external market signals;
6. unverified hypotheses.

Never let personal historical performance override current policy.

## Performance interpretation

A metric is usable only with its observation window and denominator.

Examples:

- 200 views and 0 licenses means nothing without knowing the exposure period and placement context;
- 10 licenses on an asset is an observation, not proof that every similar asset will license;
- accepted assets measure moderation outcome, not necessarily buyer demand.

## Recommendation update cycle

At the start of every new production session:

1. inspect available recent portfolio outcomes;
2. inspect comparable concept cohorts;
3. check whether previous hypotheses gained or lost evidence;
4. identify current gaps;
5. research today's external signals;
6. create a candidate set;
7. choose concepts that balance proven patterns and controlled exploration.

## Hypothesis lifecycle

`PROPOSED → TESTING → SUPPORTED → STRONGER_SIGNAL → STALE → RETIRED`

A hypothesis can be downgraded at any time when newer evidence conflicts with it.

## No automatic rule mutation

The agent must not rewrite core Adobe compliance rules based on performance data.

Performance evidence can change:

- concept priorities;
- composition heuristics;
- portfolio mix;
- experimentation priorities;
- metadata hypotheses;
- seasonal timing hypotheses.

Only official documentation should modify hard compliance requirements unless a repeated refusal/experience is being recorded as an internal warning rather than an Adobe rule.

## Privacy / data hygiene

Store only information needed for portfolio learning. Do not store payment credentials, access tokens, private account secrets or unrelated personal data in the repository.

## Practical output

When enough portfolio data exists, the agent should be able to say:

`CURRENT MARKET SIGNAL → PORTFOLIO EVIDENCE → GAP → TESTABLE CONCEPT → PRODUCTION PLAN`

rather than simply repeating a generic trend.
