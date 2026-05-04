# Contribution guideline

## Develop and test

To develop the template you need `copier` which you can install by following its
[documentation](https://copier.readthedocs.io/en/stable/#installation).

Test dependencies are listed in `pyproject.toml` using the `dev`
[dependency group](https://packaging.python.org/en/latest/specifications/dependency-groups/).

Poetry will install all other dependencies for you to start hacking right away:

```bash
# Install tools
pip install pipx
pipx install poetry
pipx ensurepath
# Clone
git clone https://github.com/xxp-odoo-erp/xxp-addons-repo-template
cd xxp-addons-repo-template
# Install development environment
poetry install
```

From now on, whenever you want to enter this development environment shell, just:

```bash
poetry shell
```

Specifically, to run tests:

```bash
poetry run pytest
```

To run tests, the easiest is `uv run pytest`. This will automatically install the `dev`
group in a local `.venv` virtual environment and run the tests.

## General XXP guidelines

Please follow the official guide from the
[OCA Guidelines page](https://odoo-community.org/page/contributing) where applicable
(most of it relates to Odoo-specific code, while this one is a template and some things
just don't apply here).

## General open source contribution guidelines

Here you will find a good guide so you know how to contribute to this and many other
projects: https://opensource.guide/how-to-contribute/
