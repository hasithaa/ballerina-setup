# Notice

Please note that this repository is no longer active. The code has been moved to [ballerina-platform/setup-ballerina](https://github.com/ballerina-platform/setup-ballerina/), which is now the official Ballerina repository for the setup-ballerina GitHub Action. Please update any references or links to the new repository location to ensure you are using the latest version of the action. Thank you for your cooperation in keeping up-to-date with the Ballerina community's latest developments.

----


[![Test Ubuntu](https://github.com/hasithaa/setup-ballerina/actions/workflows/test-ubuntu.yml/badge.svg?branch=main)](https://github.com/hasithaa/setup-ballerina/actions/workflows/test-ubuntu.yml)
[![Test Windows](https://github.com/hasithaa/setup-ballerina/actions/workflows/test-windows.yml/badge.svg?branch=main)](https://github.com/hasithaa/setup-ballerina/actions/workflows/test-windows.yml)
[![Test Action](https://github.com/hasithaa/setup-ballerina/actions/workflows/test-macos.yml/badge.svg?branch=main)](https://github.com/hasithaa/setup-ballerina/actions/workflows/test-macos.yml)
[![GitHub license](https://img.shields.io/github/license/hasithaa/setup-ballerina)](https://github.com/hasithaa/setup-ballerina/blob/main/LICENSE)
[![GitHub issues](https://img.shields.io/github/issues/hasithaa/setup-ballerina)](https://github.com/hasithaa/setup-ballerina/issues)

# Setup Ballerina

This Github action installs [Ballerina](https://ballerina.io)'s build system and package manager command; the `bal` command.

## Inputs

|Input| Description|Required|
|---|---|---|
|_version_|Ballerina SwanLake Version|yes|

## Usage

_**Note**: This action is supported on all operating systems (`ubuntu`, `macos`, `windows`)_

### Ubuntu

```yaml
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: hasithaa/setup-ballerina@v1
        name: Install Ballerina
        with:
          version: 2201.1.1
      - run: bal version
      - run: bal run hello.bal
```

[![Test Ubuntu](https://github.com/hasithaa/setup-ballerina/actions/workflows/test-ubuntu.yml/badge.svg?branch=main)](https://github.com/hasithaa/setup-ballerina/actions/workflows/test-ubuntu.yml)
[![Source](https://img.shields.io/badge/-Source-blue)](https://github.com/hasithaa/setup-ballerina/blob/main/.github/workflows/test-ubuntu.yml)

### MacOs

```yaml
    runs-on: macos-latest
    steps:
      - uses: actions/checkout@v2
      - uses: hasithaa/setup-ballerina@v1
        name: Install Ballerina
        with:
          version: 2201.1.1
      - run: bal version
      - run: bal run hello.bal
```

[![Test Action](https://github.com/hasithaa/setup-ballerina/actions/workflows/test-macos.yml/badge.svg?branch=main)](https://github.com/hasithaa/setup-ballerina/actions/workflows/test-macos.yml)
[![Source](https://img.shields.io/badge/-Source-blue)](https://github.com/hasithaa/setup-ballerina/blob/main/.github/workflows/test-macos.yml)

### Windows

```yaml
    runs-on: windows-latest
    steps:
      - uses: actions/checkout@v2
      - uses: hasithaa/setup-ballerina@v1
        name: Install Ballerina
        with:
          version: 2201.1.1
      - run: bal version
      - run: bal run hello.bal
```

[![Test Windows](https://github.com/hasithaa/setup-ballerina/actions/workflows/test-windows.yml/badge.svg?branch=main)](https://github.com/hasithaa/setup-ballerina/actions/workflows/test-windows.yml)
[![Source](https://img.shields.io/badge/-Source-blue)](https://github.com/hasithaa/setup-ballerina/blob/main/.github/workflows/test-windows.yml)

## License
The scripts and documentation in this project are released under the [Apache License](https://github.com/hasithaa/setup-ballerina/blob/main/LICENSE).
