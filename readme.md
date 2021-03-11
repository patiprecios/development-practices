# General Development Guidelines

This document contains the general development guidelines.

This guide intends to achieve consistency across the organization's projects.

The guidelines for specific languages and technologies are in [Specific guidelines](#specific-guidelines).

# Guidelines

## Languages

All the repository information (eg. tags, labels, description), code, commit messages and technical docs inside the repository _must_ be written in English.

All external documents, pull requests and issue discussions, final user documentation, and any resource that is not part of the repository _may_ be written in the local language.

## Code quality

All of the repositories _must_ implement automated code quality checks.

No merges to main branches _must_ be made if the code doesn't comply with quality requirements.

Some examples of quality checks are:

- Testing / Coverage
- Formatting / Linting
- Complexity / Metrics
- Typing (if apply)
- Outdated versions
- Security / Vulnerabilities / Known bugs
- Hardcoded Secrets / Keys / Tokens

## Testing & coverage

If you found a problem, you _must_ fix or delegate and create an issue with the details.

If a repository has tests, no broken tests _must_ be allowed to merge to main branches.

You _should_ write tests for all the code you write. Consider the code that is not tested, broken.

You _should_ make the coverage reach 100%, with a lower bound of 50% including branches.

For any bug, a test _must_ be written to check the existence and the fix.

Recommended tests:

- Unit tests
- Integration tests
- Acceptance tests
- Regression and requirements tests

## Text editors / IDEs

Repositories _may_ specify a default editor.

If a default editor is chosen, _must_ be specified in the project's `README.md` file.

All configuration for the default editor _may_ be under git dvcs in their respective folder (Eg. `.vscode`, `.idea`, etc).

If you use another editor, please don't commit configuration files, instead, update or create instructions for them under the `docs` folder in the respective repository. This is to avoid having a lot of different configurations for different IDEs.

## Branching model

Preferably use the [Github flow](https://guides.github.com/introduction/flow/) branching model. The names of the branches are at the discretion of the team. Use issues and pull requests to discuss and code reviews.

Don't let the branches get old. Keep branches simple, Is better to merge small features than risk a big branch be abandoned for a long time.

Write descriptive commit messages, which is the legacy you leave to other developers.

## Dependencies

You _should_ keep dependencies outdated with at most _1 major version_, _5 minor versions_, and _no outdated patch versions_ since the latest stable release.

## Specific guidelines

Here is a list of specific guidelines:

- [Python](languages/python.md)

# Contributing

Nothing here is written in stone, but the important thing is that something must be written. If there are better solutions & practices, consider implementing them.

To change the content in this document just create a pull request.
