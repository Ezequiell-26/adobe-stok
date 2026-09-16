# SKILL — LEGAL, IP, RELEASES AND LICENSES

## Purpose

Prevent avoidable legal and licensing problems before an asset reaches READY_TO_UPLOAD.

## Prompt-level exclusions

By default do not reference:

- living artists or artist names as style instructions;
- celebrities;
- named real people;
- fictional copyrighted characters;
- brands and trademark names;
- distinctive branded products;
- recognizable advertising campaigns;
- copyrighted artwork/designs;
- protected logos/packaging;
- restricted locations when rights are uncertain.

## Visual inspection

Do not only inspect the prompt. Check the final image for accidental IP:

- logos;
- labels;
- recognizable product silhouettes;
- brand-specific packaging;
- copyrighted art;
- murals/street art;
- distinctive architecture;
- signage;
- celebrity resemblance.

## People

A generic fictional person is the default. If the image intentionally depicts an identifiable real person, verify the appropriate rights/model release requirements.

For generated people who were not based on a real person but resemble one, follow Adobe's current fictional-people disclosure process.

## Property / locations

If property, architecture, artwork or a recognizable location is central, determine whether Adobe currently requires a property release or has location-specific restrictions.

When uncertain: `HOLD_FOR_LEGAL_REVIEW`.

## Generator license

For every asset record:

- tool name;
- exact plan/tier;
- date checked;
- official license/terms URL;
- relevant commercial-use language;
- whether stock submission is permitted;
- whether additional restrictions apply;
- evidence saved by the operator.

Never infer commercial stock rights from “commercial use” alone. The exact tool terms must permit the intended use.

## Metadata/IP

Never use third-party names as keyword bait. Adobe's current guidance also restricts prohibited names/references in titles and keywords. Metadata must be a truthful description of the actual asset.

## Legal states

`PASS` — rights are adequately supported.

`HOLD` — evidence is missing or ambiguous.

`FAIL` — prohibited/unsupported rights situation.

Never convert a HOLD into PASS by assumption.
