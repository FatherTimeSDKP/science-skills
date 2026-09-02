Contributing to FatherTimeSDKP Scientific Skills

Thank you for contributing to the FatherTimeSDKP scientific-agent workflow.

This repository contains scientific software, computational models, AI-agent skills, research documentation, and experimental SDKP concepts. Contributions should prioritize reproducibility, scientific grounding, transparency, and clear separation between established science and proposed models.

Contribution Principles

Contributors SHOULD:

1. Preserve scientific provenance.
2. Prefer authoritative scientific sources.
3. Clearly distinguish established results from hypotheses.
4. Include units and dimensional analysis for physical equations.
5. Provide reproducible computational methods.
6. Document assumptions and model limitations.
7. Include tests when adding computational functionality.
8. Avoid presenting simulations as experimental validation.
9. Avoid introducing unsupported scientific claims as established facts.
10. Preserve existing functionality unless a change intentionally modifies it.

Scientific Status

Scientific statements and computational results SHOULD be classified where appropriate as:

* ESTABLISHED — supported by established scientific evidence.
* DERIVED — mathematically derived from stated assumptions.
* SIMULATION — generated computationally.
* HYPOTHESIS — proposed mechanism requiring validation.
* UNVERIFIED — insufficient independent evidence.
* FALSIFIED — contradicted by reproducible testing.

Adding an SDKP Model

A proposed SDKP model SHOULD define:

* SDKP state variables
* Mathematical equations
* Physical meaning of each variable
* Units
* Constants
* Initial conditions
* Boundary conditions
* Reference values
* Model assumptions
* Baseline comparison
* Predicted observable
* Falsification condition

The minimum SDKP state representation is:

$$
\Psi=(S,\rho,K,P)
$$

where:

* $S$ = size or geometric scale
* $\rho$ = density
* $K$ = kinetic state or kinetic-energy contribution
* $P$ = position or spatial configuration

Baseline Requirement

When an SDKP model modifies an established physical relationship, the established model SHOULD be calculated first.

For example:

$$
g_{\mathrm{baseline}}

\frac{GM}{r^2}
$$

An additional SDKP contribution should then be defined separately:

$$
g_{\mathrm{SDKP}}

g_{\mathrm{baseline}}
+
\Delta g_{\mathrm{SDKP}}
$$

This makes the proposed effect directly testable against the baseline.

Explicit SDKP Correction

When the kinetic-gravity model is used, the current explicitly defined test form is:

$$
\Delta g_{\mathrm{SDKP}}

\alpha
\frac{GM}{r^2}
\left(\frac{K}{Mc^2}\right)
\left(\frac{\rho}{\rho_0}\right)
\left(\frac{S_0}{S}\right)
\Phi(P)
$$

This expression is a proposed SDKP test model, not an established physical law.

Contributors MUST NOT describe this equation as experimentally validated unless independent evidence supports that claim.

Every symbol MUST be defined before the equation is used in a scientific calculation.

Dimensional Analysis

New physical equations SHOULD pass dimensional analysis before implementation.

For example:

$$
[\Delta g_{\mathrm{SDKP}}]

\mathrm{m/s^2}
$$

Dimensionally inconsistent expressions SHOULD NOT be merged without a documented mathematical reason.

Computational Contributions

New code SHOULD include:

* Clear variable names
* Unit conventions
* Reproducible inputs
* Deterministic calculations where practical
* Error handling
* Documentation
* Tests for important calculations

Numerical output SHOULD identify the model and parameters used to generate it.

Data and Sources

External scientific data SHOULD retain provenance.

Where practical, document:

SOURCE
DATASET / PUBLICATION
VERSION
RETRIEVAL DATE
PARAMETER
UNIT
TRANSFORMATION
UNCERTAINTY

Sources should be independently verifiable whenever possible.

Pull Requests

Pull requests SHOULD explain:

1. What was changed.
2. Why the change was necessary.
3. Which files were modified.
4. Whether scientific equations changed.
5. Whether new dependencies were introduced.
6. How the change was tested.
7. Any known limitations.

Scientific claims requiring external validation SHOULD be identified explicitly.

Review Expectations

Reviewers SHOULD check:

* Mathematical correctness
* Dimensional consistency
* Unit consistency
* Reproducibility
* Source provenance
* Baseline comparison
* Falsifiability
* Computational tests
* Documentation quality

A contribution may be rejected or returned for revision if a scientific claim cannot be reproduced or adequately supported.

Experimental Validation

Computational agreement with an established model is not, by itself, evidence for a new physical mechanism.

A proposed SDKP effect should ultimately be evaluated through:

$$
\text{Prediction}
\rightarrow
\text{Measurement}
\rightarrow
\text{Comparison}
\rightarrow
\text{Falsification}
$$

Independent experimental or observational evidence SHOULD be identified separately from repository-generated results.

Changes to Scientific Claims

Changes that strengthen, weaken, or materially alter a scientific claim SHOULD include an explanation of the evidence supporting the change.

Historical results SHOULD NOT be silently overwritten when doing so would remove information needed for reproducibility.

When practical, preserve:

* Previous equations
* Previous model versions
* Simulation parameters
* Validation results
* Commit history

AI-Agent Contributions

AI-generated scientific contributions SHOULD be reviewed by a human before being treated as validated scientific results.

AI agents SHOULD:

* Verify external claims.
* Preserve citations and provenance.
* Check dimensions.
* Check units.
* Identify assumptions.
* Compare against established models.
* Report uncertainty.
* Distinguish hypothesis from evidence.

AI-generated text MUST NOT be treated as independent scientific validation.

Security and Safety

Do not commit:

* Passwords
* API keys
* Access tokens
* Private credentials
* Personal authentication information
* Proprietary data without authorization

Security-sensitive information SHOULD be handled through appropriate secret-management mechanisms rather than repository files.

Reproducibility Standard

A contribution should, where practical, allow another researcher to reconstruct the result from:

$$
\boxed{
\text{Data}
+
\text{Equations}
+
\text{Parameters}
+
\text{Code}
+
\text{Method}
}
$$

If reconstruction is not possible, the limitation SHOULD be documented.

Core Contribution Standard

The repository follows a simple principle:

