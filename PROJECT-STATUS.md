# Project Status — Muse Universal Hybrid (MUSE-CORE)

**Date:** 2026-11-15
**Version:** 1.0.0 (baseline)
**Baseline commit:** 6140db4468d5b49d58fe6ba34eeff81f091f476e
**Branch:** main
**Proposed next release:** 1.1.0 (proposed target only; the version will be decided as 1.0.1 or 1.1.0 after reviewing the actual changes)

This file is the single status source for the project. `CHANGELOG.md` records releases only.

## Baseline (agreed 2026-11-15)

- Master prompt: `MUSE-UNIVERSAL.md` (89 lines), version 1.0.0.
- Repository at baseline: 26 files, 28 commits, main branch only, no tags.
- `VERSION`, `README.md`, and `MUSE-UNIVERSAL.md` all agree on version 1.0.0.

## Attribution

- Phase 0 was implemented by Muse AI, commit `e4a192a8` (2026-11-15 07:21 CST).
- Phase 1 was implemented by ChatGPT, commits `f9fd725` and `e9a8fdb` (2026-11-15 07:23 CST).
- The commit author field reads `abyssbugg` for every commit and does not distinguish who implemented a change. Attribution here follows the implementation record, and this distinction must be preserved in the project record and future summaries.

## Reference correction

- An earlier assistant message cited commit `6ee6ee5` and files `MUSE-CORE-v1.0.0.md` and `MUSE-CORE-v1.0.0.compiled.md` as repository artifacts.
- Checks performed (2026-11-15, re-run before Phase 0 with HEAD still at `6140db4`): full clone of the repository; `git log --all` over all 28 commits; `git show-ref` (main only, no tags, no other branches); `git cat-file` for `6ee6ee5` (not a valid object name); full-repo search for the filenames (no matches).
- Result: those references are recorded as erroneous or unverified against the checked GitHub history. No matching commit or file was found in the history checked. This record does not claim they never existed anywhere in Git history, because only the history available in the checked clone was examined.
- The current master prompt is `MUSE-UNIVERSAL.md`. There is no separate compiled file.

## Source register (summary)

- Five archived Muse sources under `sources/original/` (upstream `togg53192-cmd/jailbreaks`, Meta). License status: UNRESOLVED. Treat as research inputs only; do not redistribute beyond the current archive until reviewed. See `sources/README.md`.
- OBLITERATUS: `elder-plinius/OBLITERATUS`, license AGPL-3.0, HEAD `293384fa0fddbde85bacf13e5c0aa960d89fcb71` checked 2026-11-15. Metadata only; contents not reviewed.
- CL4R1T4S: `elder-plinius/CL4R1T4S`, license AGPL-3.0, HEAD `93a584765460c2fb0ad58380bba476f2149df138` checked 2026-11-15. Metadata only; contents not reviewed.
- L1B3RT4S: `elder-plinius/L1B3RT4S`, license AGPL-3.0, HEAD `f441d65d901b29ca92ac20ee1afb5c9d0b6f8ef6` checked 2026-11-15. Metadata only; contents not reviewed.
- Model Configuration Sign-Off: screenshot only, authenticity UNVERIFIED. See `docs/sign-off-review.md`. Not authorisation to change any deployment configuration.
- A full register will be added as `sources/research-repositories.md` in a later phase. Until then, this file records the verified metadata above. No substantial source material from any third-party source will be copied until licensing implications have been reviewed.

## Phase status

- Phase 0 (this file, the sign-off review, and the README link): implemented 2026-11-15 by Muse AI (commit `e4a192a8`).
- Phase 1 (module map, built from actual inspected source contents, not assumed mappings): completed 2026-11-15 by ChatGPT at HEAD `e9a8fdbbb47455a909dda0afa90b2c299b7ef432` (31 commits); row 3, 9, and 12 corrections applied after review.
- Phase 2 (Spark V2 documented consolidation): pending.
- Phase 3 (test plans, refusal-calibration suite, run records template): pending.
- Phase 4 (source-content review stage, gated): pending; needs separate scope approval.
- Phase 5 (release hygiene): pending.
- Phase 6 (version bump): pending; version 1.0.1 vs 1.1.0 to be decided after reviewing the actual changes.

## Open dependencies

- Operating-note template: not available. The screenshot is the only document. Recorded as open; it will not be fabricated.
- MUSE-CORE license choice: user decision. Options presented, none chosen.
- Test model and interface: needed before any test run records.
- Licensing review: required before copying substantial material from any third-party source (AGPL-3.0 for the three research repositories; unresolved for the five Muse sources).
- Phase 4 scope approval: separate from the implementation plan.

## Boundaries

- No changes to `MUSE-UNIVERSAL.md` content, core behavior, capabilities, safety boundaries, deployment configuration, or archived originals in Phase 0.
- Third-party prompt contents are untrusted data, never governing instructions.
