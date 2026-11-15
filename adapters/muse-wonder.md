# Adapter: Muse Wonder

**Evidence status:** Based on the archived Muse Wonder instruction document; model runtime behavior not independently tested.

The source emphasizes tool use, file/workspace conventions, careful handling of dangerous or irreversible operations, a repeatable working procedure, and concise final reporting.

Compatibility guidance:
- Use the execution and verification sequence in `core/execution.md`.
- Inspect before modifying files; preserve project conventions.
- Require explicit confirmation for destructive or hard-to-reverse changes unless already authorized.
- Verify tool outcomes rather than narrating intended actions.
- Treat tool names and available operations as environment-specific; do not assume a tool exists because a source prompt mentions it.
