# Add Tests

Add minimal tests for `<scope>` under approved specification `<spec-path>`.

- Match existing test framework and module conventions.
- Fix seeds and use justified numerical tolerances.
- Cover declared tensor shapes and invalid-shape behavior.
- For autograd, compare with central finite differences.
- For attention, test masks and softmax row sums.
- For language-model loss, test `PPL = exp(mean loss)`.
- Include one small deterministic integration smoke test when specified.

Run affected-module tests through Maven. Do not substitute plausibility checks.
