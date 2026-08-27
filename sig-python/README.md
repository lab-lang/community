# SIG Python

Status: Active

Chairs: [Gonzalo Vidal (@Gonza10V)](https://github.com/Gonza10V)

Project: [Python](https://github.com/orgs/lab-lang/projects/3)

## Purpose

Provide an idiomatic, typed Python authoring path into the same Lab compiler used by the native language.

## Scope

**Owns:** the public Python package, Python authoring APIs, lowering into the checked representation, source mapping, typing support, examples, and scientific-Python interoperability.

**Does not own:** alternate compiler semantics, a Python-only backend, native Lab syntax, or device APIs that bypass reviewed artifacts.

## Strategy

- Preserve semantic parity with Lab rather than creating a second language model.
- Lower directly into the shared checked representation.
- Use familiar Python patterns only when they keep physical effects explicit.
- Combine Python typing with source-aware Lab diagnostics.
- Preserve identity and provenance when adapting external scientific objects.
- Keep interactive and notebook state out of implicit compilation inputs.

## Success

- Paired Python and Lab fixtures produce equivalent results and failures.
- Supported authoring patterns are accurately understood by static type checkers.
- Diagnostics point to the originating Python source.
- External scientific objects retain stable identity and provenance.
- Published packages work from clean supported environments.

## Open questions

- How should dynamic records expose precise static types?
- Which raw external-object escape hatches should be public?
- How should third-party packages declare compiler compatibility?

## Repositories

- Source: [lab-lang/lab](https://github.com/lab-lang/lab), including Python packages, bindings, generated vocabulary, examples, and tests
