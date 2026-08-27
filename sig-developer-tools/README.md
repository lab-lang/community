# SIG Developer Tools

Status: Draft

Chairs: [Mike Arpaia (@marpaia)](https://github.com/marpaia)

Project: [Developer Tools](https://github.com/orgs/lab-lang/projects/5)

## Purpose

Give people a consistent way to create, understand, check, compile, and inspect Lab projects across command-line, editor, browser, and embedded hosts.

## Scope

**Owns:** CLI experience, shared IDE services, language-server and WebAssembly APIs, editor extensions, workspace analysis, formatting, navigation, and artifact inspection.

**Does not own:** language semantics, compiler planning policy, separate parsers for each host, or silent live execution from an editor.

## Strategy

- Build every host on one shared analysis core.
- Make tools understand projects, imports, packages, generated declarations, and targets.
- Add incremental analysis without changing batch compiler meaning.
- Trace diagnostics and compiled artifacts back to source.
- Keep checking, dry-run, review, and live execution visibly distinct.

## Success

- CLI, language server, WebAssembly, and browser hosts agree on shared fixtures.
- Navigation and refactoring remain correct across complete projects.
- Formatting is syntax-preserving and idempotent.
- Representative projects receive responsive interactive analysis.
- Distributed tools complete clean installation and authoring journeys.

## Open questions

- What symbol and project-index model should both frontends share?
- How should generated and external declarations appear in navigation?
- Which capabilities belong in shared services versus host adapters?

## Repositories

- Source: [lab-lang/lab](https://github.com/lab-lang/lab), including the CLI, IDE core, WebAssembly, language server, and extensions
- Playground host: [lab-lang/website](https://github.com/lab-lang/website)
