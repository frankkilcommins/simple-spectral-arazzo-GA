# Simple Spectral Arazzo GitHub Action

This repository demonstrates how to use a **GitHub Action** to lint API description files (OpenAPI, AsyncAPI, etc.) using the **Spectral CLI**.

## Purpose

The goal of this repository is to show how API files located in the `apis` folder can be automatically linted using **Spectral**, a tool for enforcing best practices and validating API descriptions. The linting process runs on each `push`, `pull_request`, and can also be triggered manually via GitHub Actions.

## How It Works

- **Spectral CLI**: Spectral is installed as part of the GitHub Action workflow and is used to lint all `.yaml` and `.json` files located in the `apis` directory.
- **GitHub Action**: The Action is triggered automatically on:
  - **Pushes** to the `main` branch
  - **Pull requests** targeting the `main` branch
  - **Manual dispatches** via the Actions tab in GitHub
- **Linting Results**: The results of the linting process, including any errors or warnings, are displayed directly in the Action logs, ensuring that API descriptions conform to best practices.
