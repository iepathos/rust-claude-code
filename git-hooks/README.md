# Git Hooks

This directory contains git hooks for the project. These hooks help maintain code quality by automatically running checks before commits.

## Available Hooks

- **pre-commit**: Runs `just fmt` to ensure code is properly formatted before committing

## Installation

To install the git hooks, run:

```bash
just install-hooks
```

This will copy all hooks from this directory to `.git/hooks/` and make them executable.

## Bypassing Hooks

If you need to bypass the pre-commit hook temporarily, you can use:

```bash
git commit --no-verify
```

However, this should be used sparingly as the hooks help maintain code quality.