<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/brand/wordmark-full-dark.svg">
    <img alt="The Lab Compiler" src="assets/brand/wordmark-full-light.svg" width="520">
  </picture>
</p>

# Lab Community

This repository records Lab's durable strategy and lightweight community structure. It explains why Lab exists, how its Special Interest Groups fit together, and how temporary Working Groups coordinate work across them.

Lab is a compiler for portable biological work. Scientists describe the biological result they want, the constraints that must hold, and the evidence needed to accept it in Python or the Lab Language; the compiler specializes that intent for a laboratory, its policies, and its instruments.

## Start here

- [Strategy](STRATEGY.md) states the shared mission, principles, and architectural direction.
- [Governance](GOVERNANCE.md) defines SIGs, WGs, chairs, decisions, and group lifecycle.
- [Community Groups](GROUPS.md) lists SIGs, WGs, chairs, and canonical GitHub Projects.
- [Contributing](CONTRIBUTING.md) explains how to improve these documents and where to take implementation work.

## Special Interest Groups (SIGs)

- [SIG Compiler](sig-compiler/)
- [SIG Instruments](sig-instruments/)
- [SIG Lab Language](sig-lab-language/)
- [SIG Python](sig-python/)
- [SIG Developer Tools](sig-developer-tools/)
- [SIG Docs](sig-docs/)
- [SIG Robotics](sig-robotics/)
- [SIG Release](sig-release/)

SIGs are persistent and own technical scope. Each SIG has one or two chairs who organize its work and communication.

## Working Groups

- [WG Experimental Validation](wg-experimental-validation/)

WGs are temporary, have chairs and sponsoring SIGs, and close when their stated deliverables are complete.

Milestones, issue backlogs, sequencing, and delivery status belong in GitHub trackers and source repositories. SIG charters should remain useful across many releases.

## Where work happens

Strategy, group charters, and governance belong here. Source code, implementation issues, and technical decision records remain in their owning repositories:

- [lab-lang/lab](https://github.com/lab-lang/lab) contains the compiler, both frontends, packages, runtime, instrument integrations, CLI, and editor infrastructure.
- [lab-lang/robotics](https://github.com/lab-lang/robotics) contains downstream simulation, visualization, physics, and robot-learning work.
- [lab-lang/website](https://github.com/lab-lang/website) contains the public website, documentation renderer, and browser playground.
- The remaining [lab-lang repositories](https://github.com/orgs/lab-lang/repositories) contain independently testable instrument protocols and related components.

The detailed implementation status in those repositories is authoritative. A strategy document describes direction; it does not make an unfinished feature real.
