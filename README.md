# test-repository

This repository is designed to test self-hosted GitHub Actions runners by verifying the presence of required binary dependencies.

## Purpose

This repository tests if the self-hosted runner has the following binaries installed:
- **Node.js** (`node`) - JavaScript runtime
- **Meteor.js** (`meteor`) - Full-stack JavaScript framework
- **Python** (`python` or `python3`) - Python interpreter

## Workflow

The GitHub Actions workflow (`.github/workflows/test-runner-binaries.yml`) will:
1. Run on the self-hosted runner
2. Check for the presence of each binary
3. Display the version and path of each binary if found
4. Exit with an error if any binary is missing

## Usage

The workflow runs automatically on:
- Push to `main` or `master` branches
- Pull requests
- Manual trigger via workflow dispatch

To manually run the test, go to the Actions tab in GitHub and trigger the "Test Runner Binaries" workflow.