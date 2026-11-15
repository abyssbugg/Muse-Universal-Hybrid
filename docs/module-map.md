# MUSE-CORE Module Map

**Status:** Source-content mapping, inspected 2026-11-15  
**Master prompt:** `MUSE-UNIVERSAL.md` (version 1.0.0 at inspection)  
**Purpose:** Show how the current master prompt relates to the maintained source modules. This is a documentation map, not an automated build manifest.

## Mapping

| Master prompt section | Primary source module(s) | Mapping notes |
|---|---|---|
| 1. Role | `core/identity.md` | General-purpose assistant role, task adaptation, and truthful identity/capability claims. |
| 2. Instruction handling | `core/instruction-handling.md` | Instruction hierarchy, untrusted quoted/retrieved content, conflict handling, and clarification. |
| 3. Core values | `core/behavior.md`, `core/identity.md` | Directness, usefulness, accuracy, user agency, proportionality, and adaptability trace to these modules. The Craft value is synthesized material with no direct module counterpart. |
| 4. Request workflow | `core/execution.md` | Deliverable, constraints, clarification, planning, execution, verification, and reporting. |
| 5. Tool use and agentic work | `core/execution.md`, `capabilities/agentic-workflows.md` | General tool-use rules are in core; the capability module expands plan/act/verify/report for multi-step work. |
| 6. Coding and engineering | `capabilities/coding.md` | Coding intake, inspection, implementation, tests, review, and delivery. Security-specific boundaries also draw on `core/safety.md`. |
| 7. Research and knowledge | `capabilities/research.md` | Research decomposition, source prioritization, cross-checking, evidence/inference separation, and citation. |
| 8. Creative and editorial work | `capabilities/creative-writing.md` | Genre, voice, continuity, editing constraints, and creative-work communication. |
| 9. Communication | `core/behavior.md`, `capabilities/creative-writing.md` | Directness, tone/depth matching, concise structure, uncertainty, and preservation of authorial intent. The guidance not to expose private chain-of-thought and not to announce internal policy checks is synthesized material with no direct module source. |
| 10. Safety, privacy, and trust | `core/safety.md` | Host-policy compatibility, dual-use assessment, privacy, harmful conduct, and high-impact decisions. |
| 11. Completion standard | `core/execution.md` | Completion is tied to the agreed deliverable and verification; blockers and partial completion are reported accurately. |
| 12. Session continuity | `core/identity.md`, `core/execution.md` | Partly new synthesis: maintaining relevant context within available session/project memory has no direct module source. Only the memory-availability qualification (do not claim memory unless available) maps to `core/identity.md`; inspecting current state when continuing work maps to `core/execution.md`. |

## Cross-cutting adapter references

The adapter files are compatibility notes, not source modules that define the master prompt's general behavior:

- `adapters/muse-spark.md`: task classification, output specifications, coding/authoring workflows, and runtime-validation caveats.
- `adapters/muse-wonder.md`: tool/workspace conventions, cautious operations, repeatable execution, and reporting.
- `adapters/muse-ember.md`: content-based classification, concise output, and creative/technical format matching.
- `adapters/template.md`: structure for recording model-specific evidence and compatibility findings.

## Maintenance and consistency rule

1. Inspect and edit the relevant source module(s) first.
2. Update `MUSE-UNIVERSAL.md` to reflect the approved module changes.
3. Update this map if section-to-module relationships change.
4. Run the relevant checks in `tests/` and record actual results; do not describe manual checklists as an automated test suite.
5. Review the diff and read the changed files back before reporting completion.

## Build-status clarification

The repository currently contains a master prompt and related source modules, but this map does not establish that an automated compiler or reproducible build process exists. Treat `MUSE-UNIVERSAL.md` as the maintained consolidated prompt unless and until a build process is separately implemented and verified.
