# Rundown of `ci.yaml` workflow

Before running jobs, be sure to provide the required inputs.

## Lint job

1. Set up GO
2. Clone the repository
3. Go mod tidy
4. Run go linter using a pre-made GitHub action

Uses .golangci.yaml (from the caller workflow root directory) as its config file.

## Editorconfig job

1. Clone the repository
2. Install Editorconfig and run it

Uses .editorconfig (from the caller workflow root directory) as its config file.

## Go test job

1. Set up GO
2. Clone the repository
3. Go mod tidy
4. Run go tests

## Licenses check

1. Clone repository
2. Set up GO
3. Install go-licenses
4. Run go-licenses

This step prints out a comma-separated report (CSV) listing the libraries used by a binary/package, the URL where their
licenses can be viewed and the type of license.

## Sonarcloud check

1. Clone repository
2. Run sonarcloud check
