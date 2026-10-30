# CLAUDE.md

Guidance for Claude Code when working in this repository.

## Project

EDF: a Python package (`src/edf`). Early scaffold; no domain code yet.

## Layout

- `src/edf/` — package source (src layout, built with hatchling)
- `tests/` — pytest tests

## Commands

Uses [uv](https://docs.astral.sh/uv/) for environments and dependencies.

- Install: `uv sync`
- Test: `uv run pytest`
- Single test: `uv run pytest tests/test_version.py::test_version`
- Lint: `uv run ruff check .`
- Format: `uv run ruff format .`

## Conventions

- Python >= 3.11, line length 100, ruff rules E/F/I/UP/B.
- Add runtime deps with `uv add <pkg>`, dev deps with `uv add --dev <pkg>`.
