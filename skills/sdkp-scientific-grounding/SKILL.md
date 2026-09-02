SDKP Scientific Grounding

Purpose

SDKP Scientific Grounding provides an evidence-first workflow for scientific AI agents working with the Size–Density–Kinetic–Position (SDKP) representation.

The representation is:

$$
\Psi = (S,\rho,K,P)
$$

where:

* $S$ = size or geometric scale
* $\rho$ = density
* $K$ = kinetic state or kinetic-energy contribution
* $P$ = position or spatial configuration

This skill is designed to improve scientific-agent grounding, reduce unnecessary context expansion, and maintain a strict distinction between established scientific results, computational results, hypotheses, and unsupported claims.

Scientific Grounding Rules

Agents using this skill SHOULD:

1. Identify the scientific question before retrieving evidence.
2. Prefer primary literature, institutional databases, validated datasets, and authoritative documentation.
3. Retrieve only the information necessary to answer the question.
4. Preserve provenance for retrieved data.
5. Separate observations from interpretations.
6. Perform dimensional and unit checks before interpreting equations.
7. Compare new hypotheses against established physical models.
8. State assumptions explicitly.
9. Report uncertainty and numerical precision honestly.
10. Identify conditions under which the hypothesis could be falsified.

SDKP Status Classification

Every SDKP-derived result SHOULD be classified as one of:

* ESTABLISHED — supported by established scientific theory or independently validated evidence.
* DERIVED — mathematically derived from explicitly stated assumptions.
* SIMULATION — produced by a computational model.
* HYPOTHESIS — proposed SDKP mechanism requiring experimental or observational validation.
* UNVERIFIED — insufficient evidence currently available.
* FALSIFIED — contradicted by a reproducible test under the stated conditions.

SDKP terminology MUST NOT be presented as experimentally established merely because it appears in an SDKP document or repository.

Baseline Comparison

When an SDKP model modifies an established physical relationship, the agent SHOULD calculate the baseline first.

For example, when investigating kinetic contributions to gravitation:

$$
\Delta m = \frac{\Delta E}{c^2}
$$

should be evaluated before introducing an additional SDKP coupling.

A proposed SDKP correction should then be expressed separately:

$$
G_{\mathrm{SDKP}} = G_{\mathrm{baseline}} + \Delta G_{\mathrm{SDKP}}
$$

This prevents an ordinary relativistic energy contribution from being incorrectly interpreted as evidence for a new gravitational interaction.

Reproducibility

Scientific calculations SHOULD include:

* input parameters
* units
* equations
* constants
* numerical precision
* computational method
* baseline model
* SDKP modification
* output
* uncertainty or sensitivity analysis

Where possible, calculations SHOULD be deterministic and reproducible from the repository contents.

Falsifiability

An SDKP hypothesis SHOULD specify a measurable quantity that could distinguish it from an established model.

For example:

$$
R = G_{\mathrm{observed}} - G_{\mathrm{baseline}}
$$

If the predicted SDKP contribution is not distinguishable from zero within experimental uncertainty, the result SHOULD NOT be described as evidence for a new physical interaction.

Agent Workflow

Use the following compact workflow:

QUESTION
   ↓
IDENTIFY VARIABLES
   ↓
RETRIEVE AUTHORITATIVE EVIDENCE
   ↓
ESTABLISH BASELINE
   ↓
DIMENSIONAL CHECK
   ↓
RUN SDKP MODEL
   ↓
COMPARE WITH BASELINE
   ↓
UNCERTAINTY / SENSITIVITY
   ↓
FALSIFICATION TEST
   ↓
REPORT RESULT + PROVENANCE

Token-Efficient Retrieval

Agents SHOULD retrieve information in layers:

Layer 1 — Discovery

Identify relevant databases, papers, datasets, and tools.

Layer 2 — Targeted Retrieval

Retrieve only records relevant to the current scientific question.

Layer 3 — Verification

Cross-check critical claims against an independent authoritative source.

Layer 4 — Computation

Use the minimum necessary context to perform the calculation.

Layer 5 — Reporting

Return the result with provenance, assumptions, and uncertainty.

The objective is not to maximize retrieved context. The objective is to maximize scientific information per token.

Scientific Integrity

This skill does not establish SDKP as a replacement for existing scientific theories.

SDKP models are to be evaluated through:

$$
\text{Prediction}
\rightarrow
\text{Measurement}
\rightarrow
\text{Comparison}
\rightarrow
\text{Falsification}
$$

The same standard applies to SDKP as to any other proposed scientific framework.
