# WG Experimental Validation

Status: Draft

Chairs: To be named

Sponsoring SIGs:

- [SIG Compiler](../sig-compiler/)
- [SIG Instruments](../sig-instruments/)
- [SIG Release](../sig-release/)

Project: [Experimental Validation](https://github.com/orgs/lab-lang/projects/8)

## Problem

Software checks can show that Lab parses, type-checks, lowers, or produces an artifact. They do not by themselves show that the artifact is faithful to the stated biological intent, executable in a named laboratory, or capable of producing the evidence required by its acceptance criteria.

These claims span compiler behavior, instrument integrations, physical experiments, and release qualification. They need shared definitions and reproducible evidence.

## Deliverables

- A claim-and-evidence matrix that distinguishes checking, lowering, dry-run, hardware execution, and biological outcome validation.
- A small set of reference experiments authored through both frontends and run in named laboratory contexts.
- Reproducible validation packages containing source, versions, target context, compiled artifacts, materials, observations, acceptance results, and limitations.
- Public validation reports and clear handoffs for defects, support claims, and continuing ownership.

## Scope

**In scope:** Experimental design, end-to-end validation of representative Lab programs and integrations, evidence capture, acceptance criteria, and reporting conventions.

**Out of scope:** Permanent ownership of compiler or integration code, routine component testing, general validation of biological claims not exercised by a reference experiment, and treating simulation as physical evidence.

## Operation

- Decision record: this directory and linked Project issues
- Source repositories affected: [lab-lang/lab](https://github.com/lab-lang/lab), relevant instrument repositories, and [lab-lang/website](https://github.com/lab-lang/website)

Code review and ownership remain with the sponsoring SIGs and owning source repositories.

## Completion

The WG closes when sponsoring SIGs have accepted the evidence model and validation-package format, the initial reference experiments and reports are public, and recurring validation responsibilities have been transferred to their permanent owners.
