# vi

> see https://aka.ms/autorest

This is the AutoRest configuration file for Azure Video Analyzer for Media.

## Getting Started

To build the SDKs for My API, simply install AutoRest via `npm` (`npm install -g autorest`) and then run:

> `autorest readme.md`

To see additional help and options, run:

> `autorest --help`

For other options on installation see [Installing AutoRest](https://aka.ms/autorest/install) on the AutoRest github page.

---

## Suppression

``` 
directive:
  - suppress: SECRET_PROPERTY
    from:
      - Microsoft.VideoIndexer/preview/2021-10-18-preview/vi.json
      - Microsoft.VideoIndexer/preview/2021-10-27-preview/vi.json
      - Microsoft.VideoIndexer/preview/2021-11-10-preview/vi.json
      - Microsoft.VideoIndexer/preview/2022-04-13-preview/vi.json
      - Microsoft.VideoIndexer/preview/2022-07-20-preview/vi.json
      - Microsoft.VideoIndexer/preview/2024-04-01-preview/vi.json
      - Microsoft.VideoIndexer/preview/2024-06-01-preview/vi.json
      - Microsoft.VideoIndexer/preview/2024-09-23-preview/vi.json
      - Microsoft.VideoIndexer/stable/2022-08-01/vi.json
      - Microsoft.VideoIndexer/stable/2025-04-01/vi.json

    where:
      - $.definitions.AccessToken.properties.accessToken
    reason: Secrets are OK to return in a POST response.
```

---

## Configuration

### Basic Information

These are the global settings for the adp.

``` yaml
title: ViManagementClient
openapi-type: arm
openapi-subtype: rpaas
tag: package-2025-04-01
```

### Tag: package-2025-04-01
These settings apply only when `--tag=2025-04-01` is specified on the command line.

``` yaml $(tag) == 'package-2025-04-01'
version-with-underscores: 2025_04_01
input-file:
  - Microsoft.VideoIndexer/stable/2025-04-01/vi.json
```

### Tag: package-2024-09-23-preview

These settings apply only when `--tag=2024-09-23-preview` is specified on the command line.

``` yaml $(tag) == 'package-2024-09-23-preview'
version-with-underscores: 2024_09_23_preview
input-file:
  - Microsoft.VideoIndexer/preview/2024-09-23-preview/vi.json
```

### Tag: package-2024-06-01-preview

These settings apply only when `--tag=2024-06-01-preview` is specified on the command line.

``` yaml $(tag) == 'package-2024-06-01-preview'
version-with-underscores: 2024_06_01_preview
input-file:
  - Microsoft.VideoIndexer/preview/2024-06-01-preview/vi.json
```

### Tag: package-2024-04-01-preview

These settings apply only when `--tag=2024-04-01-preview` is specified on the command line.

``` yaml $(tag) == 'package-2024-04-01-preview'
version-with-underscores: 2024_04_01_preview
input-file:
  - Microsoft.VideoIndexer/preview/2024-04-01-preview/vi.json
```

### Tag: package-2025-01-01
These settings apply only when `--tag=package-2025-01-01` is specified on the command line.

```yaml $(tag) == 'package-2025-01-01'
input-file:
  - Microsoft.VideoIndexer/stable/2025-01-01/vi.json
```

### Tag: package-2024-01

These settings apply only when `--tag=package-2024-01` is specified on the command line.

```yaml $(tag) == 'package-2024-01'
input-file:
  - Microsoft.VideoIndexer/stable/2024-01-01/vi.json
```
### Tag: package-2022-08-01

These settings apply only when `--tag=2022-08-01` is specified on the command line.

``` yaml $(tag) == 'package-2022-08-01'
version-with-underscores: 2022_08_01
input-file:
  - Microsoft.VideoIndexer/stable/2022-08-01/vi.json
```

### Tag: package-2022-07-20-preview

These settings apply only when `--tag=2022-07-20-preview` is specified on the command line.

``` yaml $(tag) == 'package-2022-07-20-preview'
version-with-underscores: 2022_07_20_preview
input-file:
  - Microsoft.VideoIndexer/preview/2022-07-20-preview/vi.json
```

### Tag: package-2022-04-13-preview

These settings apply only when `--tag=2022-04-13-preview` is specified on the command line.

``` yaml $(tag) == 'package-2022-04-13-preview'
version-with-underscores: 2022_04_13_preview
input-file:
  - Microsoft.VideoIndexer/preview/2022-04-13-preview/vi.json
```

### Tag: package-2021-11-10-preview

These settings apply only when `--tag=2021-11-10-preview` is specified on the command line.

``` yaml $(tag) == 'package-2021-11-10-preview'
version-with-underscores: 2021_11_10_preview
input-file:
  - Microsoft.VideoIndexer/preview/2021-11-10-preview/vi.json
```

### Tag: package-2021-10-27-preview

These settings apply only when `--tag=2021-10-27-preview` is specified on the command line.

``` yaml $(tag) == 'package-2021-10-27-preview'
version: 2021-10-27-preview
version-with-underscores: 2021_10_27_preview
input-file:
  - Microsoft.VideoIndexer/preview/2021-10-27-preview/vi.json
```

### Tag: package-2021-10-18-preview

These settings apply only when `--tag=2021-10-18-preview` is specified on the command line.

``` yaml $(tag) == 'package-2021-10-18-preview'
version: 2021-10-18-preview
version-with-underscores: 2021_10_18_preview
input-file:
  - Microsoft.VideoIndexer/preview/2021-10-18-preview/vi.json
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
  - repo: azure-sdk-for-ruby
  - repo: azure-cli-extensions
  - repo: azure-resource-manager-schemas
  - repo: azure-powershell
```

## Go

See configuration in [readme.go.md](./readme.go.md)

## Python

See configuration in [readme.python.md](./readme.python.md)

## Ruby

See configuration in [readme.ruby.md](./readme.ruby.md)

## TypeScript

See configuration in [readme.typescript.md](./readme.typescript.md)

## CSharp

See configuration in [readme.csharp.md](./readme.csharp.md)

## Node.js

See configuration in [readme.nodejs.md](./readme.nodejs.md)
