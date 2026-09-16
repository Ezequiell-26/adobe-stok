# SKILL — AI ARTIFACT QC

## Role

Act as a hostile preflight reviewer. Assume the image contains hidden defects until inspected.

## Inspection order

1. Thumbnail sanity check.
2. 100% full-resolution inspection.
3. Edge inspection.
4. Subject anatomy/object geometry.
5. Lighting/reflection consistency.
6. Material physics.
7. Text/IP check.
8. Compression/processing check.
9. Commercial-use check.

## Mandatory anatomy checks

If humans or animals are present, inspect every visible:

- hand;
- finger;
- eye;
- ear;
- limb;
- joint;
- teeth/mouth where visible;
- hair boundary;
- clothing attachment;
- object contact.

## Mandatory geometry checks

Look for:

- duplicated objects;
- merged objects;
- floating objects;
- impossible thickness;
- broken symmetry;
- warped circles/rectangles;
- impossible perspective;
- melted edges;
- inconsistent scale;
- repeated texture patterns;
- broken zippers/buttons/seams.

## Physics checks

Verify:

- gravity;
- contact shadows;
- reflections;
- refractions;
- translucency;
- liquids;
- foam;
- ice;
- smoke;
- cloth behavior;
- hair interaction with wind/pose.

## Photography checks

Reject when materially present:

- blur or soft focus where sharpness is required;
- accidental motion blur;
- severe noise;
- excessive denoising;
- oversharpening halos;
- unnatural HDR;
- bad white balance;
- clipping;
- crushed shadows;
- strange color banding;
- overprocessing;
- sensor-like artifacts deliberately introduced by generation.

## AI fingerprint check

A visually attractive asset can still fail. Search for subtle generative fingerprints:

- repeated facial microfeatures;
- impossible pores;
- duplicated jewelry;
- inconsistent hair strands;
- impossible text fragments;
- impossible reflections in eyes/glass/metal;
- inconsistent depth-of-field across adjacent objects;
- perspective changes inside one object;
- texture seams that do not follow surface geometry.

## Decision

`PASS` — no material issue detected.

`FAIL` — any material defect that should be fixed before upload.

`HOLD` — evidence is insufficient to decide safely.

Never downgrade a defect merely because the image looks convincing at thumbnail size.
