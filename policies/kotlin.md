# Kotlin Policy

- Target Kotlin 2.4 and Java 17.
- Follow existing repository style and Maven module boundaries.
- Prefer immutable values, explicit domain types, and small focused functions.
- Avoid unsafe casts, hidden mutable state, and broad exception handling.
- Keep tensor shape assumptions explicit at API boundaries.
- Reuse canonical components before adding new code.
- Add dependencies only when an approved specification requires them.
- Tests use fixed seeds and stable numerical tolerances.
