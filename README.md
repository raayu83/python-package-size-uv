# Recursive Package Size

This is a fork of https://github.com/qertoip/python-package-size.

Learn after-install weight of any Python package including its dependencies.

The tool will **loop over your project dependencies**, install each dependency in its own venv and report the actual size including dependency tree.

This is useful for optimizing dependencies of your large applications, libraries or containers.

This is **especially useful in machine learning** context, where dependencies easily explode into gigabytes.

## Installation

`pip install uv-package-size`

## Usage

`uv-package-size -r pyproject.toml`

or

`uv-package-size -r requirements.txt`

## Example output

```
        mypy:   43.7 MB
      awscli:   34.0 MB
       black:    6.7 MB
      pylint:    6.5 MB
      pytest:    2.5 MB
```
