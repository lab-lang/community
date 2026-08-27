# SIG Compiler

Status: Draft

Chairs: [Mike Arpaia (@marpaia)](https://github.com/marpaia)

Project: [Compiler](https://github.com/orgs/lab-lang/projects/1)

## Purpose

Turn portable scientific intent into explicit, reviewable artifacts for a particular laboratory without changing what the scientist meant.

## Scope

**Owns:** checked representations, target-independent lowering, method and resource planning, generic target and backend contracts, run-document semantics, and generic runtime interpretation.

**Does not own:** concrete instrument profiles and backends, vendor protocols and transports, live device and workcell control, frontend syntax, Python APIs, editor hosts, robot-policy training, or unreviewed changes to biological intent.

## Strategy

- Bring Lab and Python into one shared checked representation before planning.
- Specialize intent in visible stages: methods, inventory, resources, scheduling, and target operations.
- Treat material identity, quantity, custody, location, and lineage as planning inputs.
- Make the reviewed, versioned run document the boundary for physical execution.
- Define stable capability and artifact contracts; [SIG Instruments](../sig-instruments/) owns their concrete instrument implementations.
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

- Source: [lab-lang/lab](https://github.com/lab-lang/lab), including the compiler, shared runtime semantics, target contracts, and run-document formats
