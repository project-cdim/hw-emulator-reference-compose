# Changelog 0.2

## [0.2.1](https://github.com/project-cdim/hw-emulator-reference-compose/compare/v0.2.0...v0.2.1) - 2026-11-02

The changes from v0.2.0 are as follows:

### Features

- Updated `hw-emulator-reference` to v0.2.1, adding secure erase (`Drive.SecureErase`) to Drive actions.
- Updated the following POST requests to return the status code specified by `POST_RETURN_CODE` in the config file:
	- `Drive.Reset`
	- `Drive.SecureErase`
	- `Memory.Reset`
	- `NetworkAdapter.Reset`
	- `Processor.Reset`

### Breaking Change

- Changed NIC metric calculation to use the maximum speed (`MaxSpeedGbps`) instead of port data volume (`BitRate`).
- Unified CPU information obtained from ComputerSystem and Chassis.

## [0.2.0](https://github.com/project-cdim/hw-emulator-reference-compose/compare/v0.1.0...v0.2.0) - 2026-03-24

The changes from v0.1.0 are as follows:

### Other Changes

- Adopted Gunicorn for running the Python application
