# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.1.0] - 2022-07-08

### Changed

- Added `namespace: tempo` to [values.yaml](chart/values.yaml) as required by [Karavel CLI 0.4](https://github.com/karavel-io/cli/releases/tag/v0.4.0)
- Updated to [tempo v1.4.1](https://github.com/grafana/tempo/releases/tag/v1.4.1)

## [1.0.1] - 2022-03-28

### Changed

- Switch from the official `docker.io/grafana/tempo` image to the vendored `quay.io/karavel/tempo` to avoid Docker Hub's rate limits.

## [1.0.0] - 2022-03-22

Initial release

[unreleased]: https://github.com/karavel-io/platform-component-tempo/compare/1.0.1...HEAD
[1.0.1]: https://github.com/karavel-io/platform-component-tempo/compare/1.0.0...1.0.1
[1.0.0]: https://github.com/karavel-io/platform-component-tempo/releases/tag/1.0.0
