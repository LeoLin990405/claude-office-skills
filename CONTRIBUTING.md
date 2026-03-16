# Contributing to Claude Office Skills

Thank you for your interest in contributing! This document provides guidelines for contributing to this project.

## How to Contribute

### Reporting Bugs

1. Check the [existing issues](https://github.com/LeoLin990405/claude-office-skills/issues) to avoid duplicates.
2. Use the [bug report template](https://github.com/LeoLin990405/claude-office-skills/issues/new?template=bug_report.yml) to file a new issue.
3. Include steps to reproduce, expected behavior, and actual behavior.

### Suggesting Features

1. Use the [feature request template](https://github.com/LeoLin990405/claude-office-skills/issues/new?template=feature_request.yml).
2. Describe the use case and why it would be valuable.

### Submitting Pull Requests

1. Fork the repository and create a branch from `main`.
2. Follow the existing code style and directory structure.
3. If adding a new skill, include a `SKILL.md` with the standard frontmatter:
   ```yaml
   ---
   name: skill-name
   description: Brief description
   version: 1.0.0
   ---
   ```
4. If adding scripts, include basic usage comments at the top of the file.
5. Update the root `SKILL.md` index if you add or rename a skill.
6. Fill out the pull request template completely.

## Project Structure Guidelines

- **Skills** go in `skills/<format-name>/` with a `SKILL.md` entry point.
- **Scripts** go in `skills/<format-name>/scripts/`.
- **OOXML schemas** go in `skills/<format-name>/ooxml/schemas/`.
- **Workflows** (cross-format guides) go in `workflows/`.
- **Templates** (document structure starters) go in `templates/`.

## Code of Conduct

Be respectful and constructive. We are all here to build useful tools together.

## Questions?

Open a [discussion](https://github.com/LeoLin990405/claude-office-skills/issues) or reach out to the maintainers.
