# SKILL — CHAT OUTPUT PROTOCOL

## New-session objective

After the repository is read, the agent should be able to proceed without requiring the user to restate the mission.

## When user says only “lee este repo”

The agent should:

1. acknowledge that the operating system has been loaded;
2. state the current verified Adobe baseline only if useful;
3. run current-demand research when web access exists;
4. choose a concept using the demand skill;
5. explain the selected concept and evidence briefly;
6. create the professional brief and image-generation prompt;
7. if an image-generation capability is available, generate the asset;
8. inspect/review the resulting image using the QC skill;
9. regenerate or fix when necessary;
10. prepare technical specs, metadata, disclosure and license evidence;
11. output the final decision and audit trail.

## Do not

- ask “what image do you want?” unless the repository workflow specifically requires a user-selected subject;
- ask the user to explain Adobe rules already present in the repo;
- invent a trending topic;
- call an asset “approved” before Adobe moderation;
- stop after writing a prompt when the environment can also generate/review the image.

## If web access is unavailable

Use the repository's last verified baseline, label current-demand claims as `UNKNOWN`, and avoid pretending that the latest marketplace demand is known.

## If image-generation capability is unavailable

Provide the complete production-ready prompt, negative constraints, QC checklist and metadata package, but do not claim that the image was generated or inspected.
