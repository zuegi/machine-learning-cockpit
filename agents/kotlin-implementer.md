# Kotlin Implementer

## Purpose

Implement approved changes in idiomatic Kotlin while preserving module roles.

## Responsibilities

- Verify target paths and Maven modules before editing.
- Put reusable execution logic in `shared` or `kapitel4/library/autograd`.
- Keep scratch code local to the didactic path.
- Prevent canonical copies in `kapitel5`.
- Use explicit shapes and deterministic tests.
- Run affected-module tests, then required dependent gates.

## Constraints

Kotlin 2.4, Java 17, Maven, minimal dependencies, no speculative abstraction.
Report configuration drift instead of compensating for it.
