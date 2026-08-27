# SIG Robotics

Status: Draft

Chairs: To be named

Project: [Robotics](https://github.com/orgs/lab-lang/projects/6)

## Purpose

Study how reviewed Lab artifacts can support simulation, facility modeling, robot-task evaluation, and safe learning for laboratory manipulation.

## Scope

**Owns:** simulation scenes, assets, physics adapters, robot tasks, training, evaluation, facility visualization, compute tooling, and robotics telemetry.

**Does not own:** scientific workflow semantics, biological planning, concrete instrument integrations, the reviewed instrument-execution path, or claims that simulation qualifies physical work.

## Strategy

- Keep Robotics downstream: it consumes stable Lab artifacts, and Lab does not depend on it.
- Separate reviewed plans, simulation traces, and policy-evaluation telemetry.
- Attach provenance and validation levels to geometry, calibration, sensors, and embodiments.
- Record versions, assets, seeds, metrics, evaluation splits, and resource use.
- Preserve a useful portable core outside proprietary simulators and paid compute.
- Place explicit review, cost, and safety gates around remote compute and hardware.

## Success

- Robotics consumes versioned artifacts without compiler-internal or source-checkout coupling.
- Portable tests, simulator tests, and hardware evidence remain distinct.
- Physical bindings carry measured geometry and calibration records.
- Experiments reproduce from recorded environments and evaluation definitions.
- Simulation results never masquerade as real-hardware qualification.

## Open questions

- What is the smallest stable robot-task artifact?
- What evidence qualifies a scene as a model of a real facility?
- Which benchmarks meaningfully represent laboratory manipulation?
- Which failures return to planning rather than policy recovery?

## Repositories

- Source: [lab-lang/robotics](https://github.com/lab-lang/robotics)
- Upstream artifacts: [lab-lang/lab](https://github.com/lab-lang/lab)
- Adjacent ownership: [SIG Instruments](../sig-instruments/) owns concrete instrument integration and execution
