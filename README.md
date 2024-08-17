# app-bootstrap-taskfiles
Collection of taskfiles for bootstrapping various applications types with one command

## Pre-requisites

Install the following dependencies prior to use

- [Taskfile](https://taskfile.dev/): Feature rich task runner used to build task dependencies and stages
- [DevBox](https://www.jetify.com/devbox): Create an isolated local dev environment for each project

## Usage

Each task file in labeled as `LANGUAGE-taskfile.dist.yaml`. For example, for **PYTHON** it will be `Python-taskfile.dist.yaml`. You have to:

- Move the taskfile to a directory of your choice
- Rename the file from `LANGUAGE-taskfile.dist.yaml` to `taskfile.dist.yaml`
- Run `task` to see all the available targets

### Example

```bash
$ mv ~/Downloads/Python-taskfile.dist.yaml <project-path>/Taskfile.dist.yaml
$ task
```

```bash
task: Available tasks for this project:
* install:       Install dev dependencies
* format:        Format code in python source files
* lint:          Lint code in python source files
* check:         Check type annotation in python source files
* test:          Run defined tests
* init:          Initialize local dev environment
```
### Setting Up a Project

Run:

```bash
$ task init
```
After completion, run,
```bash
$ task install
```

