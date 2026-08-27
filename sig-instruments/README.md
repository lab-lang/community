# SIG Instruments

Status: Draft

Chairs: [Mike Arpaia (@marpaia)](https://github.com/marpaia)

Project: [Instruments](https://github.com/orgs/lab-lang/projects/9)

## Purpose

Connect reviewed Lab artifacts to concrete laboratory instruments through explicit, testable, and safe execution boundaries.

## Scope

**Owns:** concrete instrument capability profiles, target-specific planning and backends, vendor protocols and transports, device lifecycle, workcell execution, telemetry, and recovery.

**Does not own:** portable scientific semantics, target-independent compiler passes, generic backend and run-document contracts, frontend APIs, robotics simulation or learning, or cross-SIG validation standards.

## Strategy

- Implement instruments against declared capabilities and artifacts rather than frontend-specific behavior.
- Keep vendor protocols and transports typed, isolated, and independently testable.
- Support compilation and dry-run without a device connection, then execute the exact reviewed artifact on hardware.
- Make labware, deck layout, modules, calibration, and target configuration explicit and versioned.
- Reject unsupported or unsafe work before device action and preserve configured human-review boundaries.
- Record commands, responses, failures, recovery decisions, and provenance.

## Success

- A new instrument can integrate without changing either frontend or the portable representation.
- Dry-run and live execution interpret the same reviewed artifact.
- Vendor behavior can be tested offline and qualified separately on physical hardware.
- Device failures are diagnosable and recoverable without silently changing reviewed intent.
- Every physical action is traceable to its target configuration and compiled artifact.

## Open questions

- Where is the stable boundary between generic target lowering and device-specific planning?
- Which capabilities should be shared across liquid handlers, analytical instruments, and workcells?
- How should laboratories package, version, and review calibration and target configuration?
- Which recovery decisions require recompilation or renewed human review?

## Repositories

- Compiler backends, runtime, instrument traits, and workcells: [lab-lang/lab](https://github.com/lab-lang/lab)
- Opentrons protocol model: [lab-lang/opentrons-protocol](https://github.com/lab-lang/opentrons-protocol)
- Hamilton STAR transport: [lab-lang/hamilton-star](https://github.com/lab-lang/hamilton-star)
- Inheco SiLA integration: [lab-lang/inheco-sila](https://github.com/lab-lang/inheco-sila)
- Byonoy HID integration: [lab-lang/byonoy-hid](https://github.com/lab-lang/byonoy-hid)
