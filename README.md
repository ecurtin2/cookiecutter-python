# Cookiecutter for python projects

- [poetry](https://python-poetry.org/) dependency management/building
- linting with [ruff](https://github.com/charliermarsh/ruff)
- type checking w [mypy](https://mypy.readthedocs.io/en/stable/)
- test with [pytest](https://docs.pytest.org/)
- Docs w/ [mkdocs](https://www.mkdocs.org/) 
    - [mkdocs-material](https://squidfunk.github.io/mkdocs-material/) 
    - [mkdocs-jupyter](https://github.com/danielfrg/mkdocs-jupyter)
- Docs hosting with gh pages
- CI via github actions
- docker image build
- [vscode devcontainer](https://code.visualstudio.com/docs/devcontainers/containers)
- [github codespaces](https://github.com/features/codespaces) compatible
- command running with [just](https://github.com/casey/just)


# Usage

Install [cookiecutter](https://cookiecutter.readthedocs.io/en/stable/installation.html)

```
cookiecutter https://github.com/ecurtin2/cookiecutter-python
```
Answer the questions to finish generating the code, which will be in a new folder.



## Run in local devcontainer 

Install [VSCode](https://code.visualstudio.com/docs/setup/setup-overview)

```
cd my_project
code .
```

A Pop-up will show and ask you to run in a devcontainer, click `Reopen in Container`. 
You will then be editing code inside a running docker container of your project.


## Run in github codespaces

You can also develop on a hosted container using github codespaces. You won't need to do any setup out of the box you will simply see a running vscode in the browser.
Read their docs [here](https://docs.github.com/en/codespaces/developing-in-codespaces/developing-in-a-codespace) for more information.


# Commands


When developing you're probably going to want to test your changes locally before pushing. To run the same tests locally as in CI, use. 

```
just ci
```
See the justfile for all available commands, or run 

```
just --list
```


# Users

If you use this cookiecutter, add yourself here :)

- https://github.com/ecurtin2/dagster_delta