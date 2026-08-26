# SIG Release

Status: Draft

Chairs: To be named

Project: [Release](https://github.com/orgs/lab-lang/projects/7)

## Purpose

Turn tested source into artifacts that users can identify, install, verify, and reproduce across Lab's distributed components.

## Scope

**Owns:** qualification, packaging coordination, publication, integrity metadata, version policy, compatibility policy, installation tests, and release corrections.

**Does not own:** feature-readiness decisions for technical areas, substitutes for component tests, or support promises the project cannot maintain.

## Strategy

- Qualify the exact source revision and exact bytes that will be published.
- Test installation and representative use from clean supported environments.
- State compatibility among the compiler, Python package, editor tools, and shared schemas.
- Preserve checksums, provenance, and appropriate signing or attestations.
- Publish documentation only after its artifacts and commands are available.
- Treat rollback, yanking, supersession, and communication as part of release design.

## Success

- Every claimed platform and runtime has an installation and smoke-test gate.
- Published metadata resolves to immutable artifacts and their source revision.
- Supported component combinations pass compatibility tests.
- Documentation describes the release users can actually obtain.
- A faulty release can be corrected through an exercised procedure.

## Open questions

- Should user-facing components share a version or publish compatibility ranges?
- Which platforms and runtimes can be supported on every release?
- What signing and attestation model is proportionate for this project?
- Which cross-repository schemas need independent versions?

## Repositories

- Source and packaging: [lab-lang/lab](https://github.com/lab-lang/lab)
- Installation presentation: [lab-lang/website](https://github.com/lab-lang/website)
