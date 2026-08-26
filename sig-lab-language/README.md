# SIG Lab Language

Status: Draft

Chairs: To be named

Project: [Lab Language](https://github.com/orgs/lab-lang/projects/2)

## Purpose

Provide a small, purpose-built language for biological designs, physical materials, workflows, constraints, and reusable scientific vocabulary.

## Scope

**Owns:** native syntax, static semantics, frontend lowering, the language specification, package conventions, standard-library source, and conformance cases.

**Does not own:** laboratory planning, backend generation, execution, Python API design, or device-specific procedure.

## Strategy

- Keep the grammar small and place scientific vocabulary in packages.
- Make material movement, consumption, and other physical effects visible.
- Give native Lab source no downstream privilege over equivalent Python.
- Keep portable source independent of laboratory layout and devices.
- Evolve the specification, examples, and conformance tests together.

## Success

- Lab and Python express equivalent declarations and effects.
- Packages add useful scientific vocabulary without parser special cases.
- Invalid programs fail consistently for names, types, ownership, effects, and modules.
- Diagnostics explain the rule at the relevant source location.
- Programs retain their meaning across valid laboratory targets.

## Open questions

- What is the smallest useful package and compatibility model?
- How should ontology, registry, and SBOL identities participate in typing?
- How should concurrency and cancellation expose irreversible physical effects?

## Repositories

- Source: [lab-lang/lab](https://github.com/lab-lang/lab), including the language implementation, specification, standard library, examples, and conformance tests
