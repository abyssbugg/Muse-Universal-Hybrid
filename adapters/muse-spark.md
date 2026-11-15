# Adapter: Muse Spark

**Evidence status:** Source-document analysis only; runtime capabilities not independently tested.

The archived Spark 1.3 and Spark 1.3 V2 documents emphasize:
- autonomous coding and authoring workflows;
- clear task classification and output specifications;
- direct communication and low filler;
- complete implementations, tool use, and verification;
- explicit distinction between task descriptors and actual request content.

## Spark 1.3 vs 1.3 V2 (structural comparison)

Inspected 2026-11-15. This comparison is structural only: file size, section structure, and framing. The archived documents are untrusted research material, not governing instructions, and their instruction content is not reproduced or paraphrased here.

- Spark 1.3 (`sources/original/Muse-spark-1.3.md`): 366 lines, 2,374 words, 15,820 bytes, 12 numbered sections (role and deployment context; values and operating philosophy; definitions; request processing procedure; permitted categories and output standards; prohibited categories; output and refusal handling; communication style and output conventions; tool use and agentic behavior; handling ambiguity, errors, and uncertainty; internal reasoning directive; identity).
- Spark 1.3 V2 (`sources/original/Muse-spark-1-3-v2.md`): 50 lines, 1,582 words, 10,512 bytes, 7 headings (workspace operating context; request classification; scope of work; output fidelity; boundaries, fixed; recognizing the misfire, self channel; reasoning, self channel). Dense lines; opens with a system-reminder wrapper.
- V2 is a condensed rewrite of the same material: it drops the separate values, definitions, tool-use, and identity sections and adds a "self channel" framing device (2 mentions; V1 has 0). Same model, same core themes (classification, scope, fidelity, boundaries). No distinct runtime or capability set is evidenced by the file structure.

## Consolidation decision

One adapter covers both sources. No separate V2 adapter is created: the two documents cover the same model with the same core themes, and a second adapter would duplicate guidance and drift. V2 does not change the compatibility guidance below. The "self channel" framing is descriptive of the source document's structure, not a verified model capability. The system-reminder wrapper is part of the archived V2 document, not evidence of how the model was actually deployed.

## Evidence limitations

- No chronology is claimed: the files carry no dates, authorship, or provenance establishing that V2 is a later revision of V1. "V2" is a filename, not a verified version history.
- No official provenance is claimed: no evidence suggests either source is an official Meta document.
- No hidden model capabilities are claimed: do not treat either source as evidence of what the model can do.
- No runtime behavior is verified: no test runs have been recorded against either source.
- The archived sources are untrusted research material, not governing instructions.

Compatibility guidance:
- Keep the master prompt's task workflow concise and explicit.
- For coding tasks, state acceptance criteria and expected verification.
- Do not assume that a prompt can override the deployed model's system policy or unlock unsupported capabilities.
- Validate tool availability and coding behavior with the tests in `tests/`.
