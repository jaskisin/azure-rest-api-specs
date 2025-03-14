# workloads

> see https://aka.ms/autorest

This is the AutoRest configuration file for workloads.

## Getting Started

To build the SDKs for My API, simply install AutoRest via `npm` (`npm install -g autorest`) and then run:

> `autorest readme.md`

To see additional help and options, run:

> `autorest --help`

For other options on installation see [Installing AutoRest](https://aka.ms/autorest/install) on the AutoRest github page.

---

## Configuration

### Basic Information

These are the global settings for the workloads.

``` yaml
openapi-type: arm
openapi-subtype: rpaas
tag: package-2023-04
```

### Tag: package-preview-2023-10

These settings apply only when `--tag=package-preview-2023-10` is specified on the command line.

```yaml $(tag) == 'package-preview-2023-10'
input-file:
  - Microsoft.Workloads/common-types/v1/commonTypes.json
  - Microsoft.Workloads/operations/preview/2023-10-01-preview/operations.json
  - Microsoft.Workloads/stable/2023-04-01/monitors.json
```

### Tag: package-2023-04

These settings apply only when `--tag=package-2023-04` is specified on the command line.

```yaml $(tag) == 'package-2023-04'
input-file:
  - Microsoft.Workloads/stable/2023-04-01/SAPVirtualInstance.json
  - Microsoft.Workloads/stable/2023-04-01/commonTypes.json
  - Microsoft.Workloads/stable/2023-04-01/monitors.json
  - Microsoft.Workloads/stable/2023-04-01/operations.json
```
### Tag: package-preview-2022-11

These settings apply only when `--tag=package-preview-2022-11` is specified on the command line.

``` yaml $(tag) == 'package-preview-2022-11'
input-file:
  - Microsoft.Workloads/preview/2022-11-01-preview/SAPVirtualInstance.json
  - Microsoft.Workloads/preview/2022-11-01-preview/commonTypes.json
  - Microsoft.Workloads/preview/2022-11-01-preview/monitors.json
  - Microsoft.Workloads/preview/2022-11-01-preview/operations.json
```

### Tag: package-2021-12-01-preview

These settings apply only when `--tag=package-2021-12-01-preview` is specified on the command line.

``` yaml $(tag) == 'package-2021-12-01-preview'
input-file:
  - Microsoft.Workloads/preview/2021-12-01-preview/phpWorkloads.json
  - Microsoft.Workloads/preview/2021-12-01-preview/SAPVirtualInstance.json
  - Microsoft.Workloads/preview/2021-12-01-preview/operations.json
  - Microsoft.Workloads/preview/2021-12-01-preview/monitors.json
  - Microsoft.Workloads/preview/2021-12-01-preview/skus.json
```

---

# Code Generation

## Swagger to SDK

This section describes what SDK should be generated by the automatic system.
This is not used by Autorest itself.

``` yaml $(swagger-to-sdk)
swagger-to-sdk:
  - repo: azure-sdk-for-python
  - repo: azure-sdk-for-java
  - repo: azure-sdk-for-go
  - repo: azure-sdk-for-js
  - repo: azure-sdk-for-net
  - repo: azure-resource-manager-schemas
  - repo: azure-cli-extensions
```

## Az

See configuration in [readme.az.md](./readme.az.md)

## Go

See configuration in [readme.go.md](./readme.go.md)

## Python

See configuration in [readme.python.md](./readme.python.md)

## TypeScript

See configuration in [readme.typescript.md](./readme.typescript.md)

## CSharp

See configuration in [readme.csharp.md](./readme.csharp.md)
