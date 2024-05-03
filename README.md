# Actions Go

Action for CI workflow for go applications

<!-- action-docs-description -->
## Description

Github Action to perform build, test , scan and generate Image for go

## Permissions

Add the following permissions to the job

```yaml
permissions:
  id-token: write
  contents: read
```

## Usage

```yaml
    - name: Actions Go
      uses: variant-inc/actions-go@v1
      with:
        ecr_repository: 'demo/example'
        go-version: '1.22.2'
```

## Locating Container Images

ECR containers can be located with this URI.

```text
064859874041.dkr.ecr.us-east-2.amazonaws.com/<ecr_repository>
```
<!-- action-docs-description -->

<!-- action-docs-inputs -->
## Inputs

| parameter | description | required | default |
| --- | --- | --- | --- |
| dockerfile_dir_path | Directory Path to the dockerfile. | `false` | . |
| ecr_repository | ECR Repository Name. If this is empty, then container image will not be created.  | `false` |  |
| cloud_region | Region where the image will be created.  | `false` | us-east-2 |
| go-version | The go-version input is optional. If not supplied, the action will try to download latest go version Due to the peculiarities of YAML parsing, it is recommended to wrap the version in single quotation marks:  | `false` |  |
<!-- action-docs-inputs -->

<!-- action-docs-outputs -->

<!-- action-docs-outputs -->

<!-- action-docs-runs -->
## Runs

This action is a `composite` action.
<!-- action-docs-runs -->
