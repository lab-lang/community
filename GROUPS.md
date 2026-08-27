# Community Groups

Lab uses persistent Special Interest Groups and temporary Working Groups. Group material lives in a top-level directory named `sig-*` or `wg-*`.

## Special Interest Groups

| SIG | Responsibility | Chairs | GitHub Project |
| --- | --- | --- | --- |
| [Compiler](sig-compiler/) | Planning, lowering, target contracts, and run documents | [Mike Arpaia (@marpaia)](https://github.com/marpaia) | [Compiler](https://github.com/orgs/lab-lang/projects/1) |
| [Instruments](sig-instruments/) | Instrument backends, device control, and workcell execution | [Mike Arpaia (@marpaia)](https://github.com/marpaia) | [Instruments](https://github.com/orgs/lab-lang/projects/9) |
| [Lab Language](sig-lab-language/) | Native syntax, semantics, and scientific packages | [Mike Arpaia (@marpaia)](https://github.com/marpaia) | [Lab Language](https://github.com/orgs/lab-lang/projects/2) |
| [Python](sig-python/) | Equal Python authoring through the shared compiler | [Gonzalo Vidal (@Gonza10V)](https://github.com/Gonza10V) | [Python](https://github.com/orgs/lab-lang/projects/3) |
| [Docs](sig-docs/) | Public explanation, learning, and browser playground | [Mike Arpaia (@marpaia)](https://github.com/marpaia) | [Website & Docs](https://github.com/orgs/lab-lang/projects/4) |
| [Developer Tools](sig-developer-tools/) | CLI, language services, WebAssembly, and editors | [Mike Arpaia (@marpaia)](https://github.com/marpaia) | [Developer Tools](https://github.com/orgs/lab-lang/projects/5) |
| [Robotics](sig-robotics/) | Simulation, robot learning, and evaluation | [Mike Arpaia (@marpaia)](https://github.com/marpaia) | [Robotics](https://github.com/orgs/lab-lang/projects/6) |
| [Release](sig-release/) | Qualification, packaging, and publication | [Mike Arpaia (@marpaia)](https://github.com/marpaia) | [Release](https://github.com/orgs/lab-lang/projects/7) |

## SIG directories

Each SIG directory begins with a README that serves as its charter and landing page. New SIGs start from the [SIG template](templates/special-interest-group.md). A SIG may add proposals, decisions, meeting notes, reports, or other durable material beside it. Current priorities and delivery status belong on the SIG's linked GitHub Project.

## Working Groups

| WG | Purpose | Sponsoring SIGs | Chairs | GitHub Project |
| --- | --- | --- | --- | --- |
| [Experimental Validation](wg-experimental-validation/) | Validate compiler capabilities and integrations with reproducible experimental evidence | Compiler, Instruments, Release | [Jackson Fairborn (@jdfdragon)](https://github.com/jdfdragon) | [Experimental Validation](https://github.com/orgs/lab-lang/projects/8) |

A new WG uses a top-level `wg-*` directory and starts from the [WG template](templates/working-group.md). Its charter names chairs, sponsoring SIGs, deliverables, a tracker, and closure conditions.

WGs coordinate work but do not own code or permanent technical scope. Continuing responsibility remains with or returns to the sponsoring SIGs.
