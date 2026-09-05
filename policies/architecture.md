# Architecture Policy

## Module roles

- `kapitel3`, `kapitel4/scratch`: didactic implementations.
- `shared`, `kapitel4/library/autograd`: canonical execution components.
- `kapitel5`: training and application consuming canonical components.

## Rules

1. Classify code as didactic or canonical before implementation.
2. Reusable math, tensor, and autograd behavior has one canonical owner.
3. `kapitel5` must import canonical behavior, not copy it.
4. Scratch duplication is allowed only for a stated learning objective.
5. Changes to module boundaries require an ADR in `docs/decisions/`.
6. Verify actual module paths and dependencies before editing. Mismatch means
   configuration drift and requires a safe stop.
