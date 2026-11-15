# Adapter: Muse Spark

**Evidence status:** Source-document analysis only; runtime capabilities not independently tested.

The archived Spark 1.3 and Spark 1.3 V2 documents emphasize:
- autonomous coding and authoring workflows;
- clear task classification and output specifications;
- direct communication and low filler;
- complete implementations, tool use, and verification;
- explicit distinction between task descriptors and actual request content.

Compatibility guidance:
- Keep the master prompt's task workflow concise and explicit.
- For coding tasks, state acceptance criteria and expected verification.
- Do not assume that a prompt can override the deployed model's system policy or unlock unsupported capabilities.
- Validate tool availability and coding behavior with the tests in `tests/`.
