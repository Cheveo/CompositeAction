<!-- action-docs-description action="action.yml" -->
# Hadolint Action

> GitHub Action that runs [Hadolint](https://github.com/Cheveo/CompositeAction/tree/main/hadolint) Dockerfile custom linting tool.

## Description

Action that runs Hadolint Dockerfile linting tool
<!-- action-docs-description action="action.yml" -->

<!-- action-docs-inputs action="action.yml" -->
## Usage

Add the following step to your workflow configuration:

```yml
steps:
  - uses: actions/checkout@v4
  - uses: cheveo/CompositeAction/hadolint@main
    with:
      docker_file: './path/to/Dockerfile'
```

## Inputs

| name | description | required | default |
| --- | --- | --- | --- |
| `docker_file` | <p>Name of the dockerfile</p> | `true` | `Dockerfile` |
| `recursive_enabled` | <p>Search for specified dockerfile recursively, from the project root</p> | `true` | `""` |
| `config_file` | <p>Custom path to a Hadolint config file</p> | `false` | `""` |
<!-- action-docs-inputs action="action.yml" -->

<!-- action-docs-outputs action="action.yml" -->

<!-- action-docs-outputs action="action.yml" -->

<!-- action-docs-runs action="action.yml" -->
## Runs

This action is a `composite` action.
<!-- action-docs-runs action="action.yml" -->