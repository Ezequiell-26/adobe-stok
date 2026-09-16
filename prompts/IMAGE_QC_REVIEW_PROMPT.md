# Image QC Prompt

Inspect the supplied final image at 100% and act as a strict Adobe Stock preflight reviewer.

Do not assume the image is acceptable because it looks good at thumbnail size.

Check:
- focus and sharpness
- exposure
- color
- perspective
- geometry
- reflections
- shadows
- materials
- duplicated objects
- fused objects
- hands/fingers/eyes/teeth when applicable
- liquid, ice, foam and glass physics when applicable
- text/labels
- logos/brands/trademarks
- resemblance to real people
- recognizable protected characters/artwork
- watermarks/signatures/timestamps
- evidence of AI artifacts
- commercial usefulness
- possible near-duplicate risk

Return a table:

CHECK | PASS/FAIL/HOLD | EVIDENCE | FIX

Then return:
FINAL STATUS = READY_TO_UPLOAD / REJECTED_NEEDS_FIX / HOLD_FOR_LEGAL_REVIEW / HOLD_FOR_LICENSE_REVIEW

Do not guarantee approval.
