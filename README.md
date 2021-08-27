# install-python-pipenv-pipfile

Easily install Python, pipenv and Pipfile packages in your GitHub Action

## Features

* Installs Python
* Install pipenv
* Installs Pipfile packages with pipenv
* Caches packages for future use

## Inputs

* `python-version`: The version of Python to install

## Example usage

```yaml
name: Example job
jobs:
  job:
    name: My job
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v2

      - name: Install Python, pipenv and Pipfile packages
        uses: palewire/install-python-pipenv-pipfile@v1
        with:
            python-version: 3.8

      - name: Do my thing
        run: make
```
