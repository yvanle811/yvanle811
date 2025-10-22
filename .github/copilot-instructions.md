# Copilot Instructions for This Repository

Welcome to the repository! This document provides guidance for AI coding agents to be productive and aligned with the project's conventions and workflows.

## Project Overview

This repository includes a GitHub Actions workflow for pre-commit checks. The workflow ensures code quality by running pre-commit hooks on all files during pull requests.

### Key Components
- **GitHub Actions Workflow**: Located in `.github/workflows/`, the `pre-commit` workflow automates code quality checks.
- **Python Environment**: The project uses Python 3.x, set up via `actions/setup-python`.
- **Pre-commit Hooks**: Managed using the `pre-commit` Python package.

## Developer Workflows

### Pre-commit Workflow
1. **Install Pre-commit Locally**:
   ```bash
   pip install pre-commit
   pre-commit install --install-hooks
   ```
2. **Run Pre-commit Hooks Locally**:
   ```bash
   pre-commit run --all-files
   ```
3. **GitHub Actions**:
   - On every pull request, the `pre-commit` workflow runs automatically.

### Adding New Pre-commit Hooks
1. Update the `.pre-commit-config.yaml` file with the desired hooks.
2. Reinstall hooks:
   ```bash
   pre-commit install --install-hooks
   ```

## Project Conventions

- **Python Version**: Always use Python 3.x.
- **Pre-commit Configuration**: Define hooks in `.pre-commit-config.yaml`.
- **GitHub Actions**: Workflows are stored in `.github/workflows/`.

## External Dependencies

- **Pre-commit**: Installed via `pip`.
- **GitHub Actions**: Uses `actions/checkout` and `actions/setup-python`.

## Key Files and Directories

- `.github/workflows/pre-commit.yml`: Defines the pre-commit workflow.
- `.pre-commit-config.yaml`: Configuration for pre-commit hooks.

## Notes for AI Agents

- Follow the pre-commit workflow to ensure code quality.
- When modifying workflows, ensure compatibility with GitHub Actions.
- Reference the `.pre-commit-config.yaml` file for hook details.

---

If you have questions or need clarification, feel free to ask!