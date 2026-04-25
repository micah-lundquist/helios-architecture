# helios-architecture

Redacted public version of an internal architecture document for a self-improving memory system. Specific paths, commit identifiers, calibrated thresholds, and personal data references have been replaced with functional descriptions while preserving the architectural reasoning, decision traces, and design patterns. Submitted as a work artifact.

See [architecture.md](./architecture.md) for the document.

## Supporting analysis

[chaperone-fire-rate-convergence.svg](./chaperone-fire-rate-convergence.svg) — fire-rate decay across 273 production traces. The chaperone gate fires at ~41% on a fact's first evaluation and converges to ~16-25% on subsequent evaluations of the same fact, as the perplexity delta collapses once the model has integrated it into context expectations. Aggregate fire-rate decline (38.7% → 22.1% over the window) decomposes to ~11pp from population maturation and ~5.5pp from turn-class mix shift. The chart is the empirical signature of the dual-channel design working as intended.
