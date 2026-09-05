# Consolidate Code

Consolidate `<scope>` according to approved specification `<spec-path>`.

- Locate duplicated behavior and identify its canonical owner.
- Preserve learning-focused scratch implementations with explicit rationale.
- Move reusable execution behavior to `shared` or
  `kapitel4/library/autograd`.
- Replace `kapitel5` copies with canonical imports.
- Preserve behavior with deterministic tests before removing duplication.
- Update chapter references and run affected-module plus dependent gates.

Do not broaden the refactor. Architecture changes require an ADR in target repo.
