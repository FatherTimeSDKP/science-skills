# SDKP Scientific Grounding — Tests

## Purpose

This document defines validation tests for AI agents and computational workflows using the Size–Density–Kinetic–Position (SDKP) scientific-grounding framework.

The purpose of these tests is to determine whether an implementation:

- correctly identifies SDKP variables;
- preserves scientific provenance;
- establishes an accepted baseline before applying an SDKP extension;
- performs dimensional and unit checks;
- distinguishes the speed of light from the Earth Orbital Speed reference;
- correctly handles limiting cases;
- reports uncertainty;
- distinguishes simulation from experimental validation;
- produces falsifiable predictions; and
- preserves reproducibility.

Passing these tests does **not** establish the physical validity of SDKP.

The tests establish whether the **scientific-agent workflow has been implemented correctly**.

---

# 1. Test Status Convention

Each test SHOULD return one of:

```text
PASS
FAIL
WARN
NOT_APPLICABLE
