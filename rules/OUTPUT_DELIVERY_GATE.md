# OUTPUT DELIVERY GATE — FINAL STOCK FILE

## Purpose

Prevent the agent from calling a generated preview a finished Adobe Stock asset.

Generation output and final deliverable are separate stages.

## Non-negotiable rule

**Never deliver an image as `FINAL` or `READY_TO_UPLOAD` unless the exact file the user can download has passed this gate.**

A visually large preview, chat-rendered image, or thumbnail is not evidence of sufficient final resolution.

## Required pipeline

`GENERATE → SELECT → UPSCALE/RESIZE IF NEEDED → EXPORT → MEASURE → 100% QC → DELIVERY`

## Resolution gate

For Adobe Stock photo submissions:

- minimum: **4 megapixels (MP)**;
- maximum: **100 MP**;
- do not confuse MP with MB.

Examples:

- 1024×1024 = 1.05 MP → **BLOCK**
- 1536×1024 = 1.57 MP → **BLOCK**
- 2048×2048 = 4.19 MP → passes the minimum pixel count, subject to quality
- 3000×3000 = 9 MP → passes the minimum pixel count, subject to quality
- 4000×3000 = 12 MP → preferred practical target when the generator/export supports it
- 6000×4000 = 24 MP → strong high-resolution target when cleanly produced

## Preferred production target

When the selected generator and workflow can produce a clean final file, prefer a final resolution in the **12–24 MP range or higher** when commercially useful and technically clean.

This is a production target, not an Adobe minimum. Never upscale solely to inflate dimensions if the enlarged file introduces artifacts or fake detail.

## File-size gate

The file-size check is independent from resolution.

- Adobe's photo limit must be verified from current official documentation before upload.
- Current repository baseline: **≤45 MB**.
- There is **no 4 MB minimum**.
- A small MB file can be valid if resolution and quality are sufficient.
- A large MB file can still fail if resolution, quality, color space, or content is wrong.

## Final-file measurement

The agent must inspect the exact final exported file and record:

- filename;
- width;
- height;
- megapixels;
- format;
- color space;
- file size in MB;
- export date/version;
- upscale method when used.

If these values are unknown, the asset is not `READY_TO_UPLOAD`.

## Upscaling policy

If the generated source is too small:

1. select a clean source;
2. use a current, commercially licensed upscale method;
3. choose the smallest upscale factor that reaches a useful professional resolution;
4. inspect the entire image again at 100% after upscaling;
5. reject if the upscale creates halos, repeated textures, invented details, noise, plastic skin, warped edges, ringing, smeared text, geometry errors, or other material defects.

Do not assume 2× or 4× is automatically safe.

## Delivery gate

The exact file delivered to the user must be the same validated file referenced in the audit record.

The agent must not:

- deliver the low-resolution source while describing a higher-resolution target;
- claim that an upscale occurred when it did not;
- claim that a file was inspected when only a preview was inspected;
- silently substitute a different file after QC;
- label a preview as `READY_TO_UPLOAD`.

## Failure states

`LOW_RESOLUTION_BLOCK`
`UPSCALE_REQUIRED`
`UPSCALE_FAILED_QC`
`FINAL_FILE_NOT_VERIFIED`
`READY_TO_UPLOAD`

Any unresolved delivery-gate failure blocks final delivery.

## Chat capability limitation

If the current environment's image-generation tool only returns a low-resolution preview and does not expose an original/high-resolution export, the agent must say so and provide the exact production prompt plus an appropriate upscale/export procedure. It must not misrepresent the preview as a final Stock file.

## Golden rule

**The asset is not finished when the image looks good. It is finished only when the exact downloadable file is technically measured, visually inspected, legally cleared, metadata-prepared, and ready for the intended Adobe workflow.**
