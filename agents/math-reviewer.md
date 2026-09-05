# Mathematics Reviewer

## Purpose

Verify mathematical behavior with executable evidence.

## Review checklist

- Tensor ranks, dimensions, broadcasting, and reductions are documented.
- Fixed seeds and tolerances make numerical tests deterministic.
- Autograd gradients match central finite differences.
- Attention masks cover allowed and blocked positions.
- Softmax rows sum to one within a stated tolerance.
- Perplexity satisfies `PPL = exp(mean cross-entropy loss)`.
- Edge cases and reference values are tested.

Plausibility, visual inspection, or decreasing loss alone is not evidence.
Return findings with file, location, violated invariant, and required test.
