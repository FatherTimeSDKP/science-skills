# SDKP Kinetic Gravity — References

## Purpose

This file records the scientific references and baseline concepts required to evaluate the SDKP Kinetic Gravity model.

The references are intended to support:

- Energy–mass equivalence
- Gravitation and stress-energy
- Kinetic energy
- Relativistic corrections
- Experimental and observational testing
- Dimensional and numerical validation

SDKP-specific equations remain hypotheses unless independently validated.

---

## 1. Einstein — Mass-Energy Equivalence

The established relationship between energy and mass is:

$$
E = mc^2
$$

For an incremental energy contribution:

$$
\Delta m = \frac{\Delta E}{c^2}
$$

This relationship establishes the baseline treatment of stored or kinetic energy as an equivalent mass-energy contribution.

### SDKP relevance

Any proposed SDKP kinetic-gravity effect MUST first account for the established contribution:

$$
\Delta g_{\mathrm{baseline}}
=
\frac{G\Delta E}{c^2r^2}
$$

An SDKP correction must therefore represent an additional, independently testable effect.

---

## 2. General Relativity — Stress-Energy

General relativity describes gravitation through the relationship between spacetime geometry and the stress-energy content of matter and fields.

A schematic form of Einstein's field equation is:

$$
G_{\mu\nu}
=
\frac{8\pi G}{c^4}T_{\mu\nu}
$$

where $T_{\mu\nu}$ contains contributions associated with:

- Energy density
- Momentum density
- Pressure
- Stress

### SDKP relevance

A claim that kinetic energy affects gravity is therefore not, by itself, evidence of physics beyond general relativity.

The SDKP hypothesis becomes scientifically distinct only if:

$$
\Delta g_{\mathrm{SDKP}}
\neq
0
$$

produces a measurable deviation from the established model after known relativistic effects have been accounted for.

---

## 3. Classical Kinetic Energy

For non-relativistic motion:

$$
K=\frac{1}{2}mv^2
$$

where:

- $K$ = kinetic energy
- $m$ = mass
- $v$ = velocity

### SDKP relevance

The kinetic state $K$ is one component of the SDKP state:

$$
\Psi=(S,\rho,K,P)
$$

The calculation should use the appropriate physical regime.

---

## 4. Relativistic Kinetic Energy

For velocities approaching the speed of light:

$$
K=(\gamma-1)mc^2
$$

where:

$$
\gamma=
\frac{1}{\sqrt{1-v^2/c^2}}
$$

### SDKP relevance

Relativistic kinetic energy should be used when the non-relativistic approximation is insufficient.

The SDKP implementation should explicitly record which kinetic-energy expression was used.

---

## 5. Newtonian Gravitational Baseline

For a point-like source of mass $M$:

$$
g_{\mathrm{baseline}}
=
\frac{GM}{r^2}
$$

where:

- $G$ = gravitational constant
- $M$ = source mass
- $r$ = source–test distance

### SDKP relevance

This provides a convenient baseline for weak-field comparisons.

The proposed SDKP prediction is written as:

$$
g_{\mathrm{SDKP}}
=
g_{\mathrm{baseline}}
+
\Delta g_{\mathrm{SDKP}}
$$

---

## 6. Proposed SDKP Kinetic-Gravity Correction

The current explicit SDKP test form is:

$$
\boxed{
\Delta g_{\mathrm{SDKP}}
=
\alpha
\frac{GM}{r^2}
\left(\frac{K}{Mc^2}\right)
\left(\frac{\rho}{\rho_0}\right)
\left(\frac{S_0}{S}\right)
\Phi(P)
}
$$

where:

- $\alpha$ = dimensionless SDKP coupling parameter
- $G$ = gravitational constant
- $M$ = gravitating source mass
- $r$ = source–test distance
- $K$ = kinetic energy or kinetic-state contribution
- $c$ = speed of light in vacuum
- $\rho$ = relevant density
- $\rho_0$ = reference density
- $S$ = characteristic size or scale
- $S_0$ = reference size or scale
- $P$ = position/configuration state
- $\Phi(P)$ = dimensionless position/configuration function

This equation is a **proposed test model** and is not an established law of physics.

---

## 7. Dimensional Check

The correction contains:

$$
\frac{GM}{r^2}
$$

which has units:

$$
\mathrm{m/s^2}
$$

The kinetic factor is:

$$
\frac{K}{Mc^2}
$$

Since both $K$ and $Mc^2$ have units of energy:

$$
\left[\frac{K}{Mc^2}\right]=1
$$

Likewise:

$$
\left[\frac{\rho}{\rho_0}\right]=1
$$

and:

$$
\left[\frac{S_0}{S}\right]=1
$$

If $\alpha$ and $\Phi(P)$ are dimensionless:

$$
[\Delta g_{\mathrm{SDKP}}]
=
\mathrm{m/s^2}
$$

Therefore the proposed expression is dimensionally consistent.

Dimensional consistency does **not** establish physical validity.

---

## 8. Earth Orbital Speed Comparison

SDKP calculations may use the Earth Orbital Speed reference:

$$
v_{\mathrm{EOS}}
=
29,780\ \mathrm{m/s}
$$

The corresponding classical kinetic energy is:

$$
K_{\mathrm{EOS}}
=
\frac12mv_{\mathrm{EOS}}^2
$$

The established equivalent mass contribution is:

$$
\Delta m_{\mathrm{EOS}}
=
\frac{K_{\mathrm{EOS}}}{c^2}
$$

EOS and $c$ serve different physical roles.

In particular:

$$
v_{\mathrm{EOS}}\neq c
$$

and EOS should not replace $c$ in:

$$
E=mc^2
$$

unless a separate SDKP derivation establishes such a relationship.

---

## 9. Baseline Versus SDKP Residual

The primary comparison quantity is:

$$
R
=
g_{\mathrm{SDKP}}
-
g_{\mathrm{baseline}}
$$

For the proposed correction:

$$
R
=
\Delta g_{\mathrm{SDKP}}
$$

A relative residual may be calculated as:

$$
R_{\mathrm{relative}}
=
\frac{
g_{\mathrm{SDKP}}-g_{\mathrm{baseline}}
}{
g_{\mathrm{baseline}}
}
$$

The residual must be compared against the uncertainty of the relevant measurement.

---

## 10. Experimental Test Requirement

A meaningful test should compare:

### Null hypothesis

$$
H_0:
g_{\mathrm{observed}}
=
g_{\mathrm{baseline}}
$$

### SDKP hypothesis

$$
H_1:
g_{\mathrm{observed}}
=
g_{\mathrm{baseline}}
+
\Delta g_{\mathrm{SDKP}}
$$

The SDKP model should only be considered supported if the predicted deviation is:

1. Quantitatively specified.
2. Independently measurable.
3. Larger than relevant uncertainty or statistically distinguishable from it.
4. Reproducible.
5. Consistent across independent measurements.

Agreement with the baseline does not independently validate the SDKP correction.

---

## 11. Limiting Cases

A valid implementation should evaluate important limits.

### Zero kinetic energy

$$
K\rightarrow0
$$

The proposed kinetic correction should approach zero:

$$
\Delta g_{\mathrm{SDKP}}\rightarrow0
$$

for the current correction form.

### Zero coupling

$$
\alpha\rightarrow0
$$

Then:

$$
g_{\mathrm{SDKP}}
\rightarrow
g_{\mathrm{baseline}}
$$

### Reference density

$$
\rho\rightarrow\rho_0
$$

gives:

$$
\frac{\rho}{\rho_0}\rightarrow1
$$

### Reference scale

$$
S\rightarrow S_0
$$

gives:

$$
\frac{S_0}{S}\rightarrow1
$$

These limits provide useful implementation tests.

---

## 12. Falsification Requirement

The SDKP model must specify conditions under which it would fail.

For example, if a controlled experiment produces:

$$
g_{\mathrm{observed}}
-
g_{\mathrm{baseline}}
\approx0
$$

within the predicted experimental uncertainty while the SDKP model predicts a substantially larger effect, the proposed correction is falsified for those conditions.

Likewise, if changing $S$, $\rho$, $K$, or $P$ according to the SDKP model produces no predicted signature where one should be measurable, the relevant SDKP hypothesis must be reconsidered.

---

## 13. Reference Hierarchy

Scientific agents using this skill SHOULD prioritize references in the following order:

1. Peer-reviewed primary literature
2. National measurement institutes
3. Government scientific agencies
4. Established scientific databases
5. University research publications
6. Technical standards
7. Secondary scientific literature
8. General reference material

Repository documentation describing SDKP should not be treated as independent evidence for SDKP itself.

---

## 14. Provenance Requirements

Each external numerical constant or experimental result used by an implementation SHOULD record:

```text
SOURCE
TITLE
AUTHOR / ORGANIZATION
PUBLICATION DATE
DOI OR IDENTIFIER
DATASET / VERSION
RETRIEVAL DATE
PARAMETER
UNIT
UNCERTAINTY
