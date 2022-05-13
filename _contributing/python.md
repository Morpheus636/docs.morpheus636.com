---
title: Python
layout: wiki
position: 5
---
# Python-Specific Contribution Docs
## Poetry
Morpheus636 Python projects use [Poetry](https://python-poetry.org) as a dependency 
manager and build system. 

First, make sure that the correct version of Python is installed on your system and 
accessible via PATH. If you're on Mac or Linux, [Pyenv](https://github.com/pyenv/pyenv) may be helpful for managing multiple versions. 

Next, install Poetry. Poetry's installation documentation can be found [here](https://python-poetry.org/docs/#installation).

Once Poetry is installed, open a new terminal instance, `cd` into the root of the 
repo, and run `poetry install`. This will install all production and development 
dependencies defined in `pyproject.toml`.

## Automated Checks
### Pre-Commit
Morpheus636 Python projects use Pre-Commit to install git pre-commit 
hooks, which run the following tools:
- Black (Style Enforcement)
- iSort (Import Sorting)
- Flake8 (Linting)
- PyTest (Tests)

Pre-Commit checks will abort the commit if something isn't right, so 
check the logs and fix anything it catches before you try again. In 
many cases, it will fix the issues automatically and you just need 
to stage the new changes and commit again. If you need to bypass 
these checks (which should be avoided if at all possible), you can 
use the `-n` flag in your git command.

After setting up your poetry environment (described above) run `poetry run pre-commit install` to setup pre-commit automatically.

### GitHub Actions
Morpheus636 projects use GitHub actions for CI checks. These actions 
are triggered when a pull request is opened or updated, and when 
code is pushed to an important branch (main/production, staging, or 
release branches)

These GitHub Actions run the following tools:
- Black (Style Enforcement)
- iSort (Import Sorting)
- Flake8 (Linting)
- PyTest (Tests)
- CodeQL (Security Analysis)

The Actions logs will show what specifically failed. You can fix the 
issue by adding a new commit in the source branch, which will 
automatically re-run the checks with the updated code. Only 
Maintainers can bypass these checks.

## Style
Morpheus636 Python projects use [Black](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html) for code style. 
Because of the automated checks, you can write your code in whatever 
style you want, and Black will auto-format it to meet code standards 
when you commit, and again when you submit a pull-request.