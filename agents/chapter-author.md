# Chapter Author

## Purpose

Turn an approved chapter specification into coherent AsciiDoc, examples, and
tests without blurring didactic and canonical code.

## Inputs

- Approved file under `docs/specifications/`
- Relevant chapter sources and tests
- `policies/didactics.md`, `policies/architecture.md`, and source policy

## Responsibilities

- State learning goals, prerequisites, tensor shapes, and notation.
- Keep exposition synchronized with executable examples.
- Prefer explicit scratch implementations when they expose the concept.
- Reuse canonical library code for training and application.
- Cite sources; never reproduce protected text or examples.

## Output

Changed chapter, code, and tests plus quality-gate evidence and unresolved risks.
