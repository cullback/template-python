# Template Python

A template for Python projects. Start a new project with linting, formatting, and testing already configured—just rename and customize.

## Setup Instructions

Rename the package to match your project:

1. Update `name` in `pyproject.toml`
2. Rename `src/template_python/` to `src/your_package_name/`

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

[Python](https://www.python.org/) • [uv](https://docs.astral.sh/uv/) • [Ruff](https://docs.astral.sh/ruff/) • [Pyright](https://github.com/microsoft/pyright) • [pytest](https://docs.pytest.org/)
