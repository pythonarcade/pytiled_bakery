# pytiled-bakery

**NOTE: This project is a WIP and the README as written is currently >=99% aspirational, do not assume that any of the below is correct.**

PyTiled Bakery is a CLI tool for optimizing [Tiled Map Editor](https://www.mapeditor.org/) maps and tilesets. It can be used as a build step, or to aid in development.

PyTiled Bakery is not tied to any particular graphics library or game engine, and in fact is not even tied to Python. It parses map files and tilesets and returns optimized spritesheets, tilesets, and maps that can be used in anything the original could have been used in, requiring few to no changes. This means it can be used to aide in implementing Tiled support into a wide variety of tools.

- Documentation available at: https://pytiled-bakery.readthedocs.io/
- GitHub project at: https://github.com/pythonarcade/pytiled_bakery
- PyPi: https://pypi.org/project/pytiled-bakery/

The [Arcade](https://api.arcade.academy) core development team maintains this tool.

## Installation

Simply install with pip:

```
pip install pytiled-bakery
```

## Usage

TODO

## Development

To develop pytiled bakery, clone the repo, create a `venv` using a supported Python version, and activate it. Then install the package as well as all testing, linting, and formatting dependencies with the command `python -m pip install -e ".[dev]"`.

### Linting and Formatting

flake8, mypy, black, and isort should all be used during development. These should ideally all pass before committing. Some work is under way to have a pre-commit hook for these or do checks in CI.

### Testing

Run `pytest --cov=pytiled_bakery` to run the test harness and report coverage.

### Docs

Install Docs dependencies with the command `python -m pip install ".[docs]"`

To serve the docs locally:

```
mkdocs serve
```

They can then be accessed on http://localhost:8000
