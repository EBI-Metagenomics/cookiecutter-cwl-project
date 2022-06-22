[![Testing](https://github.com/EBI-Metagenomics/{{cookiecutter.project_slug}}/actions/workflows/test.yml/badge.svg)](https://github.com/EBI-Metagenomics/{{cookiecutter.project_slug}}/actions/workflows/test.yml)

# {{cookiecutter.project_slug}}

{{cookiecutter.project_short_description}}

## Setup

To install the pipeline we recommend Conda to manage the enviroment.

## Python dependencies

```python
$ pip install -r requirements-dev.txt
```

### Pre-commit hooks

Setup the git [pre-commit hook](https://pre-commit.com/):

```bash
pre-commit install
```

*Why?*

pre-commit will run a set of pre-configured tools before allowing you to commit files. You can find the currently configure hooks and configurations in [.pre-commit-config.yaml](./.pre-commit-config.yaml)

## Workflow

Pipeline diagram built with [cwlviewer](https://view.commonwl.org/) or similar.

# Tests

CWL tests are executed with [cwltest](https://github.com/common-workflow-language/cwltest).

Run:
```bash
cd tests
./run-tests.sh
```