# Actions Test Go

Action for CI workflow for go applications

<!-- action-docs-description -->
## Description

Github Action to Build & Test go

RequiredEnv:
  GITHUB_TOKEN
  SONAR_TOKEN
<!-- action-docs-description -->

<!-- action-docs-inputs -->
## Inputs

| parameter | description | required | default |
| --- | --- | --- | --- |
| go-version | The go-version input is optional.
      If not supplied, the action will try to download latest go version Due to the peculiarities of YAML parsing, it is recommended to wrap the version in single quotation marks: | `false` |  |
| sonar_wait_flag | Says if Sonar has to wait for analysis | `false` |  |
<!-- action-docs-inputs -->

<!-- action-docs-outputs -->

<!-- action-docs-outputs -->

<!-- action-docs-runs -->
## Runs

This action is a `composite` action.
<!-- action-docs-runs -->
