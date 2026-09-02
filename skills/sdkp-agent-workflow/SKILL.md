SDKP Agent Workflow

Purpose

SDKP Agent Workflow defines a structured workflow for scientific AI agents applying the Size–Density–Kinetic–Position (SDKP) framework.

The workflow is designed to maximize scientific grounding, computational reproducibility, token efficiency, and falsifiability.

SDKP State Representation

An SDKP state is represented as:

$$
\Psi = (S,\rho,K,P)
$$

where:

* $S$ = size or geometric scale
* $\rho$ = density
* $K$ = kinetic state or kinetic-energy contribution
* $P$ = position or spatial configuration

The agent SHOULD preserve these variables explicitly rather than collapsing them into an unspecified latent representation.

Workflow

The standard workflow is:

QUESTION
   ↓
DEFINE SDKP STATE
   ↓
IDENTIFY REQUIRED DATA
   ↓
RETRIEVE AUTHORITATIVE SOURCES
   ↓
ESTABLISH BASELINE MODEL
   ↓
CHECK UNITS / DIMENSIONS
   ↓
APPLY SDKP MODEL
   ↓
RUN COMPUTATION
   ↓
COMPARE AGAINST BASELINE
   ↓
SENSITIVITY ANALYSIS
   ↓
FALSIFICATION TEST
   ↓
REPORT RESULT + PROVENANCE

Step 1 — Define the Question

The agent SHOULD convert the user’s request into a specific scientific question.

The question SHOULD identify:

* Physical system
* Observable
* Independent variables
* Dependent variables
* Relevant time or spatial scale
* Required precision

Avoid beginning computation before the quantity being tested has been defined.

Step 2 — Define the SDKP State

Identify the relevant:

$$
S,\rho,K,P
$$

values.

If a variable is not relevant to the model, the agent SHOULD state why.

If a required variable is unknown, the agent SHOULD NOT silently invent a value.

Step 3 — Retrieve Evidence

The agent SHOULD retrieve only evidence required for the calculation.

Priority SHOULD be given to:

1. Primary scientific literature
2. Government and institutional sources
3. Curated scientific databases
4. Validated datasets
5. Technical documentation
6. Secondary sources

Every externally sourced parameter SHOULD retain provenance.

Step 4 — Establish the Baseline

Before applying SDKP, calculate the corresponding established model.

For a gravitational calculation, for example:

$$
g_{\mathrm{baseline}}

\frac{GM}{r^2}
$$

If kinetic energy contributes through established mass-energy equivalence:

$$
\Delta m

\frac{K}{c^2}
$$

and:

$$
\Delta g_{\mathrm{baseline}}

\frac{GK}{c^2r^2}
$$

The baseline MUST be preserved separately from any proposed SDKP correction.

Step 5 — Dimensional Validation

Every new equation MUST pass dimensional analysis before being simulated.

For an acceleration prediction:

$$
[g]

\mathrm{m/s^2}
$$

Dimensionally invalid equations SHOULD be rejected before numerical execution.

Step 6 — Apply the SDKP Model

The agent MAY apply the explicitly defined SDKP correction:

$$
\Delta g_{\mathrm{SDKP}}

\alpha
\frac{GM}{r^2}
\left(\frac{K}{Mc^2}\right)
\left(\frac{\rho}{\rho_0}\right)
\left(\frac{S_0}{S}\right)
\Phi(P)
$$

The complete prediction becomes:

$$
g_{\mathrm{SDKP}}

g_{\mathrm{baseline}}
+
\Delta g_{\mathrm{SDKP}}
$$

All parameters MUST be defined before the calculation.

Step 7 — Computation

The computational implementation SHOULD record:

INPUTS
CONSTANTS
EQUATIONS
UNITS
INITIAL CONDITIONS
BOUNDARY CONDITIONS
NUMERICAL METHOD
SDKP PARAMETERS
OUTPUT

Where possible, computations SHOULD be deterministic and executable from repository-controlled code.

Step 8 — Baseline Comparison

The agent SHOULD calculate the residual:

$$
R =
g_{\mathrm{SDKP}}

g_{\mathrm{baseline}}
$$

and, where useful:

$$
R_{\mathrm{relative}}

\frac{R}{g_{\mathrm{baseline}}}
$$

The residual is the quantity that must ultimately be compared with measurement uncertainty.

Step 9 — Sensitivity Analysis

The agent SHOULD vary important parameters independently.

At minimum, test:

* $S$
* $\rho$
* $K$
* $P$
* $\alpha$
* $r$

The objective is to determine whether the prediction is robust or dependent on fine-tuned parameters.

Step 10 — Limiting-Case Testing

The model SHOULD be tested under limiting conditions.

Zero kinetic state

$$
K\rightarrow0
$$

Zero coupling

$$
\alpha\rightarrow0
$$

Reference density

$$
\rho\rightarrow\rho_0
$$

Reference size

$$
S\rightarrow S_0
$$

Low velocity

The model SHOULD approach the appropriate classical kinetic-energy limit.

A model that produces unexpected behavior in a known physical limit SHOULD be flagged for review.

Step 11 — Falsification

The agent MUST identify a measurable prediction that could disprove the SDKP correction.

The fundamental comparison is:

$$
H_0:
g_{\mathrm{observed}}

g_{\mathrm{baseline}}
$$

versus:

$$
H_1:
g_{\mathrm{observed}}

g_{\mathrm{baseline}}
+
\Delta g_{\mathrm{SDKP}}
$$

If the observed residual is consistent with zero within uncertainty, the SDKP correction has not been demonstrated.

Step 12 — Classification

The final result SHOULD receive one status:

ESTABLISHED
DERIVED
SIMULATION
HYPOTHESIS
UNVERIFIED
FALSIFIED

The classification describes the evidence supporting the result, not the importance of the result.

Step 13 — Reporting

The final report SHOULD contain:

1. Scientific question
2. SDKP state
3. External evidence
4. Baseline model
5. SDKP equation
6. Inputs and units
7. Computational method
8. Results
9. Residual
10. Uncertainty
11. Sensitivity analysis
12. Falsification condition
13. Evidence classification
14. Source provenance

Token-Efficient Scientific Reasoning

The agent SHOULD avoid retrieving entire datasets, papers, or repositories when only a small portion is required.

Use:

DISCOVER
   ↓
FILTER
   ↓
VERIFY
   ↓
COMPUTE
   ↓
REPORT

The objective is:

$$
\text{Scientific Information}
\div
\text{Tokens Used}
$$

rather than maximum context size.

Reproducibility Principle

A scientific result SHOULD be reconstructable from:

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

If a result cannot be reconstructed, the missing information SHOULD be explicitly identified.

Scientific Integrity

SDKP Agent Workflow MUST maintain the distinction between:

OBSERVATION
CALCULATION
SIMULATION
INTERPRETATION
HYPOTHESIS
VALIDATION

An SDKP prediction is not automatically an observation.

A simulation is not automatically experimental validation.

A numerical match is not automatically proof of a new mechanism.

Core Principle

The SDKP scientific-agent workflow is:

$$
\boxed{
\text{Ground}
\rightarrow
\text{Model}
\rightarrow
\text{Calculate}
\rightarrow
\text{Compare}
\rightarrow
\text{Test}
\rightarrow
\text{Falsify}
}
$$

This workflow allows SDKP hypotheses to be evaluated using the same reproducibility and falsifiability standards applied to other scientific models.
