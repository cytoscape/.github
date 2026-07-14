# Contributing to Cytoscape

The Cytoscape ecosystem is a family of open source projects that welcomes
contributions from the community. Whether you're fixing a bug, adding a feature,
improving documentation, or helping others, your contributions are appreciated.

This document covers general guidelines that apply across the ecosystem. Each
project also has its own contributing guide with project-specific details —
please read the relevant one before starting work.

## Projects

- **[Cytoscape](https://github.com/cytoscape/cytoscape)** — the desktop platform
  for network analysis and visualization, extensible through apps.
  See its [CONTRIBUTING.md](https://github.com/cytoscape/cytoscape/blob/develop/CONTRIBUTING.md).
- **[Cytoscape Web](https://github.com/cytoscape/cytoscape-web)** — a
  browser-based implementation of Cytoscape that runs entirely in your browser.
  See its [CONTRIBUTING.md](https://github.com/cytoscape/cytoscape-web/blob/development/CONTRIBUTING.md).
- **[Cytoscape.js](https://github.com/cytoscape/cytoscape.js)** — a JavaScript
  graph theory library for network visualization and analysis.
  See its [CONTRIBUTING.md](https://github.com/cytoscape/cytoscape.js/blob/unstable/CONTRIBUTING.md).

## Getting Started

New contributors unsure about what to work on can explore a project's open
milestones or issues tagged `help-wanted` and `good-first-issue`. Original ideas
are also welcome — the best place to float them is the project's GitHub
Discussions or issue tracker, so maintainers can help shape the approach before
you invest time in code.

## Submitting Issues

Before writing code, file a short, descriptive issue on the relevant project's
issue tracker (or an extension/app's own tracker if the problem is specific to
it). A good issue clearly describes the bug or the feature being proposed. This
gives maintainers and the community a chance to discuss the change, and it gives
your later pull request something concrete to reference.

## Making Changes via Pull Request

The general workflow is the same across projects:

1. Fork the repository and create a branch for your change.
2. Target the correct base branch. Projects follow semantic versioning: new
   features generally target the development/unstable branch (major/minor
   releases), while bugfixes target the stable/release branch (patch releases).
   Check the project's own guide for its exact branch names.
3. Make your change, keeping commits focused and readable.
4. Include tests and documentation updates where applicable (see below).
5. Open a pull request referencing the related issue, and respond to review
   feedback.

Update documentation as part of your change rather than editing generated output
directly. Each project documents where its source docs live.

## Code Style

Favor readability and clarity over strict adherence to rules. Match the style of
the surrounding code, and use each project's configured linter/formatter (for
example, `eslint --fix` in the JavaScript projects) to keep formatting
consistent. The goal is code that is easy for others to read and understand.

## Testing

Bugfixes should come with a test that fails without the fix and passes with it.
New features should come with tests that cover the new behavior. Run the
project's test suite locally and make sure it passes before opening a pull
request. Visual or rendering changes may be better verified through a project's
debug/demo pages than through unit tests — follow the project's guidance.

## Code of Conduct

All participation in the Cytoscape ecosystem is governed by our
[Code of Conduct](https://github.com/cytoscape/cytoscape.js/blob/unstable/CODE_OF_CONDUCT.md).
By contributing, you agree to uphold it.
