# Mathematical Correctness Policy

Every mathematical change needs explicit invariants and executable checks.

- Document input, output, parameter, and intermediate tensor shapes.
- Fix random seeds and state numerical tolerances.
- Compare autograd gradients with central finite differences:
  `(f(x + eps) - f(x - eps)) / (2 * eps)`.
- Test attention masks for both retained and suppressed positions.
- Assert each softmax row sums to one within tolerance.
- Assert `perplexity = exp(mean cross-entropy loss)` using the same reduction.
- Use hand-computed or trusted reference cases where practical.
- Test invalid shapes according to established repository behavior.

Plausible output, visual similarity, or training progress never replaces these
checks.
