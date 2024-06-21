Easily install Python, pipenv and Pipfile packages in your GitHub Action

## Features

- 🐍 Installs Python
- 🔨 Installs pipenv
- 📦 Installs Pipfile packages
- 💽 Caches packages for future use

## Inputs

* `python-version`: The version of Python to install

## Usage

```yaml
name: Example action
jobs:
  job:
    name: My job
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v4

      - name: Install Python, pipenv and Pipfile packages
        uses: palewire/install-python-pipenv-pipfile@v4
        with:
          python-version: 3.11

      - name: Do my thing
        run: make
```
