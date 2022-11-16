# Python Package Cookiecutter

A [cookiecutter](https://github.com/cookiecutter/cookiecutter) template to quickly develop a new Python package.


# Features

## Python management

Despite a large variety of tools, we are still using the old-good [setuptools](https://github.com/pypa/setuptools) to manage the package.
This might change in the future, but for now, this is the tool that we know the best.
Other available options are: [flit](https://github.com/pypa/flit), [hatch](https://github.com/pypa/hatch), [poetry](https://github.com/python-poetry/poetry).


## Linting
We use [flake8](https://github.com/pycqa/flake8) for linting. Additional flake8-plugins:
  - [flake8-bugbear](https://pypi.org/project/flake8-bugbear/) for detecting bugs and potential design problems
  - [flake8-builtins](https://pypi.org/project/flake8-builtins/) for verifying that builtins are not used as variable names
  - [flake8-comprehensions](https://pypi.org/project/flake8-comprehensions/) for writing better and consistent comprehensions
  - [flake8-debugger](https://pypi.org/project/flake8-debugger/) for checking that there are no forgotten [breakpoints](https://docs.python.org/3/library/functions.html#breakpoint)
  - [flake8-eradicate](https://pypi.org/project/flake8-eradicate/) to avoid “dead” or commented code
  - [flake8-logging-format](https://github.com/globality-corp/flake8-logging-format) for consistent logging
  - [pep8-naming](https://pypi.org/project/pep8-naming/) for verifying that PEP8 naming conventions are followed
  - [tryceratops](https://pypi.org/project/tryceratops/) to avoid exception anti-patterns

## Type checking
[mypy](https://github.com/python/mypy).

## Auto-formatters
[isort](https://pycqa.github.io/isort/) for sorting imports, [autoflake](https://github.com/PyCQA/autoflake) for removing unused imports, and [black](https://github.com/psf/black) for formatting the rest of the code.

## Release automation
[bumpver](https://github.com/mbarkhau/bumpver).

## Testing
[pytest](https://github.com/pytest-dev/pytest).