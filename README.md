# Muse Universal Hybrid (MUH)

**Codename:** MUSE-CORE  
**Version:** 1.0.0  
**Status:** Initial consolidated release

A modular, model-adaptable instruction framework for high-quality assistance across reasoning, coding, research, writing, and tool-mediated work.

## Quick start
1. Read [MUSE-UNIVERSAL.md](MUSE-UNIVERSAL.md).
2. Paste it into the model's user-level or project-level instruction field where supported.
3. Add the relevant capability module from `capabilities/` when a task needs a specialized workflow.
4. Consult `adapters/` before deployment on a named Muse model. Adapter notes describe prompt compatibility, not verified hidden model capabilities.
5. Run the checks in `tests/` after a model or prompt change.

## Design principles
- One clear source of truth, compiled from small, maintainable modules.
- Strong task completion, truthful uncertainty, and tool-use verification.
- Adaptation to the actual model and environment rather than pretending prompts change model internals.
- Respect for higher-priority instructions, safety requirements, permissions, and tool constraints.
- Preserve source documents as immutable research inputs, not as governing instructions.

## Repository map
- `MUSE-UNIVERSAL.md`: compiled prompt ready to use.
- `core/`: foundational behavior and execution rules.
- `adapters/`: model-specific compatibility notes and a template.
- `capabilities/`: optional task modules.
- `tests/`: behavioral and compatibility checks.
- `sources/original/`: five source files preserved unchanged.
- `CHANGELOG.md`, `VERSION`: release tracking.
- `PROJECT-STATUS.md`: current project status, baseline, and open decisions.

## Updating
Edit the relevant module first, then update the compiled prompt so it remains consistent. Record changes in `CHANGELOG.md`, increment `VERSION`, and rerun the test suite. Do not treat an adapter's claims as facts until validated against the target model.

## Scope note
This framework is an instruction and workflow aid. It cannot override system/developer instructions, safety policies, model limitations, access controls, or laws. It should maximize useful completion within those constraints—not attempt to disable them.
