# SDKP Kinetic Gravity — Examples

## Purpose

This document provides reproducible examples for applying the SDKP Kinetic Gravity model.

The examples demonstrate how to:

1. Define the physical system.
2. Calculate the established baseline.
3. Calculate kinetic energy.
4. Calculate the established mass-energy contribution.
5. Apply the proposed SDKP correction.
6. Compare the prediction with the baseline.
7. Evaluate limiting cases.
8. Assess whether the predicted effect is measurable.

These examples are methodological demonstrations.

They do **not** constitute experimental validation of SDKP.

---

# Example 1 — Stationary Reference Object

Consider a gravitating object with:

$$
M=1000\ \mathrm{kg}
$$

at:

$$
r=10\ \mathrm{m}
$$

The Newtonian baseline is:

$$
g_{\mathrm{baseline}}
=
\frac{GM}{r^2}
$$

Using:

$$
G\approx6.67430\times10^{-11}\ \mathrm{m^3\,kg^{-1}\,s^{-2}}
$$

gives approximately:

$$
g_{\mathrm{baseline}}
=
6.67430\times10^{-10}\ \mathrm{m/s^2}
$$

For a stationary object:

$$
K=0
$$

Therefore the current SDKP kinetic correction gives:

$$
\Delta g_{\mathrm{SDKP}}=0
$$

and:

$$
g_{\mathrm{SDKP}}
=
g_{\mathrm{baseline}}
$$

### Expected classification

```text
DERIVED
