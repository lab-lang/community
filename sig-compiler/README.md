# SIG Compiler

Status: Draft

Chairs: To be named

Project: [Compiler](https://github.com/orgs/lab-lang/projects/1)

## Purpose

Turn portable scientific intent into explicit, reviewable artifacts for a particular laboratory without changing what the scientist meant.

## Scope

**Owns:** checked representations, lowering, method and resource planning, target validation, backends, run documents, and runtime interpretation. Instrument integrations live here provisionally.

**Does not own:** frontend syntax, Python APIs, editor hosts, robot-policy training, or unreviewed changes to biological intent.

## Strategy

- Bring Lab and Python into one shared checked representation before planning.
- Specialize intent in visible stages: methods, inventory, resources, scheduling, and target operations.
- Treat material identity, quantity, custody, location, and lineage as planning inputs.
- Make the reviewed, versioned run document the boundary for physical execution.
- Integrate laboratories and instruments through capability and artifact contracts, not frontend changes.
- Record every consequential decision and any permitted nondeterminism.

## Success

- Equivalent Lab and Python programs produce equivalent plans.
- One program can target materially different laboratories without semantic drift.
- Impossible ownership, inventory, resource, and target constraints fail before execution.
- A new target can integrate without modifying either frontend.
- Runtime effects are traceable to the exact reviewed artifact.

## Open questions

- Which planning choices must be deterministic, and which may be policy-driven?
- Where is the stable boundary between portable planning and laboratory specialization?
- Which recovery decisions require renewed human review?

## Repositories

- Source: [lab-lang/lab](https://github.com/lab-lang/lab), including the compiler, runtime, targets, and instrument integrations
