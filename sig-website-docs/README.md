# SIG Website & Docs

Status: Draft

Chairs: To be named

Project: [Website & Docs](https://github.com/orgs/lab-lang/projects/4)

## Purpose

Explain Lab clearly, teach people how to use it, present its maturity honestly, and provide a low-friction browser playground.

## Scope

**Owns:** public information architecture, teaching, presentation, accessibility, search, documentation rendering, and the playground host.

**Does not own:** technical specifications, compiler support claims, release qualification, or a browser-only implementation of Lab.

## Strategy

- Derive technical claims from canonical source repositories.
- Distinguish parsing, checking, lowering, simulation, execution, and hardware validation.
- Teach the project model through progressive examples rather than a feature inventory.
- Identify the version behind examples, install commands, and playground behavior.
- Use the real public compiler contracts in interactive experiences.

## Success

- Every technical claim traces to a specification, test, or release artifact.
- Examples and install instructions work against the version shown.
- The playground agrees with other compiler hosts.
- New readers can explain Lab and complete the intended learning path.
- Links, search, accessibility, builds, and version references are checked automatically.

## Open questions

- Which canonical sources should the website render directly?
- How should experimental research be shown without implying product support?
- What belongs on the website rather than in source-repository documentation?

## Repositories

- Source: [lab-lang/website](https://github.com/lab-lang/website)
- Technical sources: [lab-lang/lab](https://github.com/lab-lang/lab)
