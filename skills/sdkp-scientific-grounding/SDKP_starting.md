SDKP Scientific Grounding — References

Purpose

This document defines the reference hierarchy and evidence-handling rules used with the SDKP Scientific Grounding skill.

The objective is to ensure that scientific agents distinguish authoritative external evidence from SDKP-derived material and clearly preserve provenance.

Reference Hierarchy

When evaluating a scientific claim, agents SHOULD prioritize sources in the following order:

1. Primary peer-reviewed literature
2. Official scientific institutions and agencies
3. Authoritative scientific databases
4. Curated datasets and established repositories
5. Preprints and technical reports
6. Open-source scientific software documentation
7. Secondary scientific literature and reviews
8. Community discussions or informal sources

Lower-ranked sources may be useful for discovery but SHOULD NOT be treated as definitive evidence when a higher-quality source is available.

Recommended Scientific Sources

Literature

Agents SHOULD consider established scholarly indexes and publisher repositories when locating primary research.

Examples include:

* PubMed
* Crossref
* arXiv
* NASA ADS
* Semantic Scholar
* Web of Science
* Google Scholar

Scientific Databases

Depending on the scientific domain, agents SHOULD prefer authoritative databases such as:

* NIST
* NASA
* ESA
* NOAA
* USGS
* NIH
* UniProt
* Protein Data Bank
* AlphaFold Database
* Materials Project
* PubChem

The appropriate database SHOULD be selected according to the scientific question rather than convenience.

Evidence Classification

Retrieved information SHOULD be assigned an evidence category.

PRIMARY

Direct experimental, observational, or computational evidence from the original research.

AUTHORITATIVE

Information maintained by a recognized scientific institution, agency, or curated scientific database.

SECONDARY

Reviews, summaries, meta-analyses, or other sources interpreting primary evidence.

SDKP_DERIVED

A result calculated directly from an SDKP equation, algorithm, simulation, or repository implementation.

HYPOTHESIS

A proposed mechanism or prediction that has not yet received independent validation.

UNVERIFIED

A claim for which adequate supporting evidence has not yet been established.

Provenance Requirements

For each externally sourced scientific value, agents SHOULD preserve:

* Source name
* Source type
* Dataset or publication identifier
* Retrieval date
* Relevant version
* Units
* Original definition
* Transformation or conversion applied
* Any uncertainty associated with the value

For computational results, agents SHOULD additionally preserve:

* Code version or commit
* Input parameters
* Model assumptions
* Numerical method
* Software environment where relevant
* Output values
* Validation procedure

Baseline-First Requirement

SDKP calculations SHOULD be compared against an established baseline whenever one exists.

For physical models, the workflow SHOULD be:

ESTABLISHED MODEL
       ↓
BASELINE CALCULATION
       ↓
SDKP EXTENSION
       ↓
DIFFERENCE
       ↓
OBSERVATIONAL / EXPERIMENTAL TEST

A numerical agreement between an SDKP calculation and an established equation does not, by itself, demonstrate that SDKP provides a new physical mechanism.

Units and Dimensional Analysis

Every physical equation SHOULD undergo dimensional analysis.

For example:

$$
\Delta m = \frac{\Delta E}{c^2}
$$

has dimensions:

$$
\frac{\mathrm{J}}{\mathrm{m^2/s^2}} = \mathrm{kg}
$$

An SDKP expression SHOULD likewise have dimensions consistent with the physical quantity it claims to calculate.

Dimensionally inconsistent expressions MUST NOT be presented as physically validated results.

Independent Verification

Important scientific claims SHOULD be checked against at least one independent authoritative source whenever practical.

Particular attention SHOULD be given to:

* Physical constants
* Experimental measurements
* Astronomical observations
* Biological sequences
* Materials properties
* Published performance claims
* Statistical significance
* Claimed prediction accuracy

If independent verification is unavailable, the result SHOULD be explicitly labeled UNVERIFIED.

Handling SDKP Claims

SDKP repository material is a source for documenting the framework itself.

It is not automatically independent evidence validating the framework.

Agents SHOULD distinguish:

SDKP DOCUMENTATION
        ≠
INDEPENDENT EXPERIMENTAL VALIDATION

A claim may be accurately documented as an SDKP prediction while still requiring experimental or observational testing.

Reproducibility Standard

A scientifically useful SDKP result SHOULD allow another researcher to reconstruct the calculation from the available information.

At minimum:

INPUTS
  +
EQUATIONS
  +
CONSTANTS
  +
ASSUMPTIONS
  +
METHOD
  =
REPRODUCIBLE RESULT

If any critical component is unavailable, the limitation SHOULD be reported.

Conflict Resolution

When authoritative sources disagree, agents SHOULD:

1. Identify the exact quantities being compared.
2. Check units and definitions.
3. Check publication or dataset versions.
4. Check measurement uncertainty.
5. Determine whether the disagreement is methodological.
6. Prefer the most current authoritative source when appropriate.
7. Preserve the disagreement rather than silently selecting a preferred value.

Reporting Standard

Scientific outputs SHOULD distinguish clearly between:

* What is known
* What was measured
* What was calculated
* What was simulated
* What SDKP predicts
* What remains uncertain
* What experiment could distinguish competing explanations

The final report SHOULD avoid presenting a hypothesis as an established scientific fact.

Core Principle

The SDKP scientific-agent workflow follows:

$$
\boxed{
\text{Ground}
\rightarrow
\text{Calculate}
\rightarrow
\text{Compare}
\rightarrow
\text{Test}
\rightarrow
\text{Falsify or Support}
}
$$

Scientific credibility depends on the evidence and reproducibility of the result, not on the terminology used to describe the model.
