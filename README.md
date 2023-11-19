# Recursive Package Size

Learn after-install weight of any Python package including its dependencies.

The tool will **loop over your project dependencies**, install each dependency in its own venv and report the actual size including dependency tree.

This is useful for optimizing dependencies of your large applications, libraries or containers.

This is **especially useful in machine learning** context, where dependencies easily explode into gigabates.

## Installation

`pip install python-package-size`

## Usage

`python-package-size -r pyproject.toml`

or

`python-package-size -r requirements.txt`

## Example output

```
        mypy:   43.7 MB
      awscli:   34.0 MB
       black:    6.7 MB
      pylint:    6.5 MB
      pytest:    2.5 MB
```
