# Lab Governance

Lab uses a lightweight version of the Kubernetes community model: persistent Special Interest Groups own technical areas, while temporary Working Groups coordinate bounded work across SIGs.

## Participation and decisions

- Participation is open and asynchronous by default.
- Technical discussion and decisions happen in public issues and pull requests.
- Chairs seek consensus, summarize decisions, and ensure material objections are recorded.
- Technical changes follow the review rules of the repository that owns the code.
- Charter, chair, and group-lifecycle changes are recorded through pull requests here.
- Cross-SIG questions are resolved by the affected chairs. If consensus is not possible, they document the alternatives for a scoped decision by the community repository maintainers.

No recurring meeting is required. If a group meets, it publishes an agenda, notes, and decisions.

## Special Interest Groups

A SIG is a persistent, open group responsible for a coherent technical area. It owns long-lived scope, direction, and the relationship among its repositories and components.

Each SIG has:

- A top-level `sig-*` directory with a concise README charter.
- One or two chairs.
- Exactly one canonical organization-level GitHub Project.
- Named source repositories.

SIGs may be created when a distinct responsibility needs durable ownership. A SIG may be retired only after its responsibilities and artifacts have been transferred or explicitly retired.

New SIGs begin with the [Special Interest Group template](templates/special-interest-group.md).

The GitHub Project is the operational source of truth for the SIG. Work represented as planned, accepted, or in progress by the SIG must be captured by an issue or pull request on that board. Exploratory and drive-by contributions do not require prior board entry.

## Working Groups

A WG is a temporary, open group formed around a concrete outcome that spans multiple SIGs. It does not own code or permanent technical scope; sponsoring SIGs retain that authority.

Each WG has:

- A top-level `wg-*` directory with a README charter.
- A specific problem and deliverables.
- One or two chairs.
- Two or more sponsoring SIGs.
- A public work tracker and decision record.
- Explicit completion or closure conditions.

A WG closes when its deliverables are accepted, its problem is no longer relevant, or it can no longer make progress. Its final record states the outcome and where any continuing responsibility belongs.

New WGs begin with the [Working Group template](templates/working-group.md).

## Chairs

Chairs are organizers and facilitators, not owners of every technical decision. SIG and WG chairs:

- Maintain the charter, scope, GitHub Project or WG tracker, and public decision record.
- Facilitate discussion, triage, and contributor onboarding.
- Coordinate with other SIGs and WGs.
- Keep work within the group's charter and identify when the group should change or close.
- Arrange succession when they step down.

Chair additions and removals use a public pull request after discussion with the affected group. There are no fixed terms or elections initially.

## Deliberate omissions

Lab does not initially define subprojects, membership tiers, technical-lead roles, annual reports, committees, or a steering committee. These should be added only when the community has a concrete need that SIG and WG chairs cannot meet.

## Inspiration

This model adopts the core distinctions in [Kubernetes governance](https://github.com/kubernetes/community/blob/main/governance.md) and its [Working Group governance](https://github.com/kubernetes/community/blob/main/committee-steering/governance/wg-governance.md), with substantially less process.
