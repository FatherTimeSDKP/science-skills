# SDKP Kinetic Gravity — Tests

## Purpose

This document defines the mathematical and computational tests used to evaluate the proposed SDKP Kinetic Gravity model.

The purpose is to determine whether the model:

- is mathematically consistent;
- is dimensionally consistent;
- behaves correctly in limiting cases;
- produces predictions distinguishable from the established baseline;
- remains stable under changes of units and parameters;
- can be independently reproduced;
- generalizes to data not used during model construction; and
- produces a genuinely falsifiable physical prediction.

These tests evaluate the **model and workflow**.

Passing a computational test does not establish SDKP as experimentally validated physics.

---

# 1. SDKP State

The SDKP state is:

$$
\boxed{
\Psi=(S,\rho,K,P)
}
$$

where:

$$
S=\text{size or geometric scale}
$$

$$
\rho=\text{density}
$$

$$
K=\text{kinetic state or kinetic-energy contribution}
$$

$$
P=\text{position or spatial configuration}
$$

---

# 2. Proposed SDKP Kinetic-Gravity Equation

The current test form is:

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

The total predicted gravitational acceleration is:

$$
\boxed{
g_{\mathrm{SDKP}}
=
g_{\mathrm{baseline}}
+
\Delta g_{\mathrm{SDKP}}
}
$$

with:

$$
g_{\mathrm{baseline}}
=
\frac{GM}{r^2}
$$

Therefore:

$$
\boxed{
g_{\mathrm{SDKP}}
=
\frac{GM}{r^2}
+
\alpha
\frac{GM}{r^2}
\left(\frac{K}{Mc^2}\right)
\left(\frac{\rho}{\rho_0}\right)
\left(\frac{S_0}{S}\right)
\Phi(P)
}
$$

This equation is a **proposed SDKP hypothesis**.

It is not an established physical law.

---

# 3. Test 1 — Dimensional Consistency

The Newtonian gravitational term is:

$$
\frac{GM}{r^2}
$$

with dimensions:

$$
[G]
=
\mathrm{m^3\,kg^{-1}\,s^{-2}}
$$

$$
[M]=\mathrm{kg}
$$

$$
[r^2]=\mathrm{m^2}
$$

Therefore:

$$
\left[
\frac{GM}{r^2}
\right]
=
\mathrm{m/s^2}
$$

The kinetic factor is:

$$
\frac{K}{Mc^2}
$$

Since:

$$
[K]=\mathrm{J}
$$

and:

$$
[Mc^2]=\mathrm{kg}\cdot\mathrm{m^2/s^2}
=\mathrm{J}
$$

then:

$$
\left[
\frac{K}{Mc^2}
\right]
=1
$$

The density factor is:

$$
\left[
\frac{\rho}{\rho_0}
\right]=1
$$

The scale factor is:

$$
\left[
\frac{S_0}{S}
\right]=1
$$

If:

$$
[\alpha]=1
$$

and:

$$
[\Phi(P)]=1
$$

then:

$$
\boxed{
[\Delta g_{\mathrm{SDKP}}]
=
\mathrm{m/s^2}
}
$$

### PASS condition

The complete SDKP correction has dimensions of acceleration.

### FAIL condition

Any unresolved dimensional factor remains.

---

# 4. Test 2 — Zero Kinetic Energy

Set:

$$
K=0
$$

Then:

$$
\frac{K}{Mc^2}=0
$$

and therefore:

$$
\boxed{
\Delta g_{\mathrm{SDKP}}=0
}
$$

The total model becomes:

$$
\boxed{
g_{\mathrm{SDKP}}
=
g_{\mathrm{baseline}}
}
$$

### Expected result

```text
PASS
