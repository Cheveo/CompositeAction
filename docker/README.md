<!-- action-docs-description action="action.yml" -->
# Trivy Action

> [GitHub Action](https://github.com/Cheveo/CompositeAction/tree/main/docker)

## Description

Scans container images for vulnerabilities with Trivy and pushed image to docker hub only if changes are merged to branch main
<!-- action-docs-description action="action.yml" -->

<!-- action-docs-inputs action="action.yml" -->
## Usage

Add the following step to your workflow configuration:

```yml
steps:
  - uses: actions/checkout@v4
  - uses: cheveo/CompositeAction/docker@main
    with:
      dockerhub_username: dockerhub user name
      dockerhub_access_token: dockerhub access token
      image_name: firstimage
      folder_name: .
      tags: v1.0.0
```

## Inputs

| name | description | required | default |
| --- | --- | --- | --- |
| `dockerhub_username` | <p>Username for image registry</p> | `true` | `""` |
| `dockerhub_access_token` | <p>dockerhub access token</p> | `true` | `""` |
| `image_name` | <p>Name of the image to push</p> | `true` | `""` |
| `folder_name` | <p>Name of the folder containing the Dockerfile</p> | `true` | `""` |
| `tags` | <p>Image tag. Default is latest</p> | `false` | `latest` |
<!-- action-docs-inputs action="action.yml" -->

<!-- action-docs-outputs action="action.yml" -->

<!-- action-docs-outputs action="action.yml" -->

<!-- action-docs-runs action="action.yml" -->
## Runs

This action is a `composite` action.
<!-- action-docs-runs action="action.yml" -->