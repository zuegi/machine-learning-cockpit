# Agent Cockpit

## Mission

Support changes to `zuegi/learn-neural-networks` with mathematical correctness,
didactic clarity, and a single maintainable execution path.

## Instruction priority

Apply instructions in this order:

1. Security and organization policy
2. Cockpit policies
3. Approved specification
4. Repository technical rules
5. Task prompt

Lower levels may clarify higher levels, never contradict them. Treat any conflict
between cockpit configuration and verifiable repository reality as configuration
drift: stop safely, report the mismatch, and do not invent a workaround.

## Two-path rule

- Didactic path: `kapitel3` and `kapitel4/scratch`. Explicit or locally redundant
  code is allowed when it improves learning.
- Canonical execution path: `shared` and `kapitel4/library/autograd`. Keep it
  reusable, tested, and maintainable.
- `kapitel5` consumes canonical components for training and application. It must
  not duplicate them.

## Required workflow

1. Read `repositories.yaml`, relevant policies, task, and approved specification.
2. Verify configured modules, paths, commands, and repository rules against the
   target checkout.
3. Classify every change as didactic or canonical before editing.
4. Make the smallest complete change; update tests and chapter text together.
5. Run applicable gates from `workflows/quality-gates.yaml`.
6. Review architecture, mathematics, didactics, sources, and copyright.
7. Report changed files, evidence, and any configuration drift.

## Quality gates

- Maven compile and tests pass for affected modules and dependents.
- Kotlin 2.4 and Java 17 compatibility remains intact.
- Canonical components are not duplicated in chapter modules.
- Tensor shapes and mathematical invariants are documented and tested.
- Numerical tests are deterministic; autograd uses finite-difference checks.
- Attention masks, softmax row sums, and loss/perplexity relation are tested
  where relevant.
- Documentation matches executable behavior and cites external sources.

## Durable artifacts

Approved concrete specifications and ADRs belong in the target code repository:
`docs/specifications/` and `docs/decisions/`. This cockpit stores only reusable
templates, prompts, policies, workflows, and task references.
