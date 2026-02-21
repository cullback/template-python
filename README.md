# Template Python

A starting point for Python projects that constrains LLM-assisted development to a known-good structure. Without a template, every new repo gets a different project layout, different tooling choices, and different dependency decisions. This template locks in [uv](https://docs.astral.sh/uv/) for packaging, [Ruff](https://docs.astral.sh/ruff/) for linting, [Pyright](https://github.com/microsoft/pyright) for type checking, and [pytest](https://docs.pytest.org/) for testing — rename and customize.

## Setup Instructions

Rename the package to match your project:

1. Update `name` in `pyproject.toml`
2. Rename `src/template_python/` to `src/your_package_name/`
3. Run `direnv allow && just bootstrap && just check`

Then start building:

- Add modules to `src/your_package_name/`
- Add tests to `tests/`
- Add dependencies with `uv add`

## Development

```bash
just              # Show available recipes
just bootstrap    # Install dependencies
just check        # Lint and format check
just fmt          # Auto-format code
just test         # Run tests
```

## Tech Stack

[Python](https://www.python.org/) • [uv](https://docs.astral.sh/uv/) • [Ruff](https://docs.astral.sh/ruff/) • [Pyright](https://github.com/microsoft/pyright) • [pytest](https://docs.pytest.org/) • [direnv](https://direnv.net/) • [just](https://github.com/casey/just)
