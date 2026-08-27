# Community Groups

Lab uses persistent Special Interest Groups and temporary Working Groups. Group material lives in a top-level directory named `sig-*` or `wg-*`.

## Special Interest Groups

| SIG | Responsibility | Chairs | GitHub Project |
| --- | --- | --- | --- |
| [Compiler](sig-compiler/) | Planning, lowering, run documents, and execution | To be named | [Compiler](https://github.com/orgs/lab-lang/projects/1) |
| [Lab Language](sig-lab-language/) | Native syntax, semantics, and scientific packages | To be named | [Lab Language](https://github.com/orgs/lab-lang/projects/2) |
| [Python](sig-python/) | Equal Python authoring through the shared compiler | To be named | [Python](https://github.com/orgs/lab-lang/projects/3) |
| [Website & Docs](sig-website-docs/) | Public explanation, learning, and browser playground | To be named | [Website & Docs](https://github.com/orgs/lab-lang/projects/4) |
| [Developer Tools](sig-developer-tools/) | CLI, language services, WebAssembly, and editors | To be named | [Developer Tools](https://github.com/orgs/lab-lang/projects/5) |
| [Robotics](sig-robotics/) | Simulation, robot learning, and evaluation | To be named | [Robotics](https://github.com/orgs/lab-lang/projects/6) |
| [Release](sig-release/) | Qualification, packaging, and publication | To be named | [Release](https://github.com/orgs/lab-lang/projects/7) |

The initial SIGs remain drafts until their chairs are named.

## SIG directories

Each SIG directory begins with a README that serves as its charter and landing page. New SIGs start from the [SIG template](templates/special-interest-group.md). A SIG may add proposals, decisions, meeting notes, reports, or other durable material beside it. Current priorities and delivery status belong on the SIG's linked GitHub Project.

## Working Groups

| WG | Purpose | Sponsoring SIGs | Chairs | GitHub Project |
| --- | --- | --- | --- | --- |
| [Experimental Validation](wg-experimental-validation/) | Validate compiler capabilities and integrations with reproducible experimental evidence | Compiler, Release | To be named | [Experimental Validation](https://github.com/orgs/lab-lang/projects/8) |

WG Experimental Validation remains a draft until its chairs are named. A new WG uses a top-level `wg-*` directory and starts from the [WG template](templates/working-group.md). Its charter names chairs, sponsoring SIGs, deliverables, a tracker, and closure conditions.

WGs coordinate work but do not own code or permanent technical scope. Continuing responsibility remains with or returns to the sponsoring SIGs.
