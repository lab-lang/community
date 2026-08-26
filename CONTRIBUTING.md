# Contributing to Lab Community

This repository documents project strategy. Code changes, bug reports, and implementation proposals normally belong in the source repository that owns the affected component.

## Improving strategy documents

Before proposing a change:

1. Read [the shared strategy](STRATEGY.md), [governance](GOVERNANCE.md), and the affected [SIG charter](GROUPS.md#special-interest-groups).
2. Inspect the current implementation and its authoritative support documentation.
3. Identify whether the proposal changes durable direction, SIG scope, a technical boundary, or the definition of success.
4. Link to the source, issue, experiment, or external evidence that motivates the change.

A focused pull request should update the smallest coherent set of documents. Cross-SIG changes should update every affected charter and, when necessary, the shared strategy. A temporary cross-SIG effort with a concrete deliverable may be better expressed as a Working Group.

This repository is not the place for quarterly plans, release checklists, issue inventories, or changing status snapshots. Put those in the relevant GitHub tracker or source repository.

## Writing expectations

- Describe visible project behavior and scientific or technical outcomes in direct language.
- Separate current behavior from intended direction.
- Distinguish parsing, checking, lowering, simulation, execution, and hardware validation.
- State important non-goals and ownership boundaries.
- Avoid turning an issue backlog into strategy prose.
- Prefer objectives and success conditions that will remain meaningful across several releases.
- Preserve open questions when the project has not made a decision.
- Link to canonical technical decisions rather than duplicating their full contents here.

## Implementation contributions

- Compiler, language, Python, CLI, editor, runtime, and instrument work belongs in [lab-lang/lab](https://github.com/lab-lang/lab).
- Simulation, visualization, physics, training, and compute work belongs in [lab-lang/robotics](https://github.com/lab-lang/robotics).
- Public website and documentation-rendering work belongs in [lab-lang/website](https://github.com/lab-lang/website).
- Instrument protocol changes belong in the relevant repository in the [lab-lang organization](https://github.com/orgs/lab-lang/repositories).

New contributors can start with the current [`good first issue` backlog](https://github.com/lab-lang/lab/issues?q=is%3Aissue%20state%3Aopen%20label%3A%22good%20first%20issue%22). Each source repository defines its own validation commands; run the complete relevant gate before presenting a change as finished.

## Reviewing a strategy change

Review should ask:

- Does this match the owning SIG's boundary?
- Is the stated current condition verified?
- Does the direction preserve the shared architecture?
- Are downstream consequences and non-goals visible?
- Is the document likely to remain useful across several release cycles?
- Is the proposal strategic, or should it be an implementation issue instead?

Participation in SIGs and WGs is open. Chairs facilitate public issues and pull requests and record decisions in repository history; they do not replace technical review in the owning source repository.
