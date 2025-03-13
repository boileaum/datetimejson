# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.8] - 2025-03-12

### Added

- Added Python 3.12 to the testing matrix in GitHub Actions workflow.

### Changed

- Updated the publish github action.

### Fixed

- Fix test failure due to changes in faker library (faker version is now fixed)
- Fix github actions not installing the target python version (#3)

### Removed

- Removed Python 3.6, 3.7 and 3.8 from the testing matrix in GitHub Actions workflow (not compatible with Ubuntu 24.04).