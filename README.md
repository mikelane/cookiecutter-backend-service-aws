# Cookiecutter Backend Service with AWS and Python
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Overview
This is a cookiecutter template for a backend web service which runs on AWS.
The service itself is defined with AWS CDK and it uses Python throughout
(including in the AWS CDK infrastructure code). This is intended to be used in 
place of running `npx cdk init --app=sample-app --language=python`. The cdk
init script generates a python project, yes, but it does not use poetry or 
modern linting. This template comes with dependencies for testing, linting, and 
code quality checks.

## Usage
### Pre-Requisites
- Install [git](https://git-scm.com/)
- Install [poetry](https://python-poetry.org/)
- Install [cookiecutter](https://cookiecutter.readthedocs.io/)

### Setup a new project
```shell
cookiecutter gh:mikelane/cookiecutter-backend-service-aws
```

Answer the questions that cookiecutter asks you. You can accept the defaults by
pressing enter.

Cookiecutter will create a new project as a subdirectory of the current working
directory with the name you specified. It will also create a git repository and
it will install some basic dependencies. Additionally, it will set up pre-
commit hooks for linting and formatting.
