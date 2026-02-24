# Template Python

A starting point for Python projects that constrains LLM-assisted development to a known-good structure.

## Setup Instructions

Rename the package to match your project:

1. Update `name` in `pyproject.toml`
2. Rename `template_python/` to your package name
3. Run `nix develop --command just bootstrap && nix develop --command just check`

## Project Structure

```
template_python/         # Rename to your package name
├── __init__.py
└── __main__.py
tests/
└── test_example.py
```

## Development

Run `just` to see available recipes.

## Tech Stack

- [uv](https://docs.astral.sh/uv/)
- [Ruff](https://docs.astral.sh/ruff/)
- [Pyright](https://github.com/microsoft/pyright)
- [direnv](https://direnv.net/)
- [just](https://github.com/casey/just)
