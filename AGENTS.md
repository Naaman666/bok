# AGENTS.md

This file provides guidance to AI coding agents (e.g. ChatGPT Codex) when working with this repository.

## Project Overview

<!-- Describe the project purpose and goals here. -->

## Development Setup

```bash
# Install dependencies
```

## Common Commands

```bash
# Run tests

# Lint / format
```

## Code Style

- Follow the existing patterns and conventions in the codebase.
- Keep functions small and focused on a single responsibility.
- Write clear, self-documenting code; only add comments where the logic is non-obvious.
- Do not add unnecessary error handling, logging, or abstractions.

## Architecture Notes

<!-- Describe key architectural decisions and important modules here. -->

## Git Workflow

Only two persistent branches exist: `develop` (active work) and `main` (stable releases).

- **Humans:** always commit directly to `develop`. Never commit or push to `main`.
- **AI agents (Claude, Codex, etc.):** open pull requests from a short-lived `claude/*` or `codex/* ` branch. The PR must always target `develop`, never `main`. Delete branch after merge.

Do not create feature or topic branches.
