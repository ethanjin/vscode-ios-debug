# Change Log

All notable changes to the "ios-debug" extension will be documented in this file.

## v0.4.1
### Changed
- Fix and enable debugging support for iOS 17+
  - Note the additional requirement of setting correct lldb path to `lldb.library` setting.
- Fix issue with non-ascii character in logs.
- Other minor fixes

## v0.4.0
### Added
- Debug on local devices when VS Code is connected to Remote Development via SSH.
  - Automatically prompt to install companion and ask if local devices should be shared when running in remote.
  - List and debug on locally connected physical iOS devices without any extraneous setup
- Add new option `iosInstallApp` to launch config to enable/disable installing app before launching.

### Changed
- Better error handling and logging at a few places.

## v0.3.3
### Changed
- Fix attach behavior on device. Properly attach to running app when targeting a device.
- A bunch of underlying changes and refactoring.

## v0.3.2
### Changed
- Minor improvements in logging and error handling while launching Simulator

## v0.3.1
### Changed
- Disable `ios-debug.focusSimulator` by default, since it was causing some unwanted behaviour and crashes.

## v0.3.0
### Added
- Focus the simulator window automatically when attaching or continuing from breakpoints.
- Added an configuration option `ios-debug.focusSimulator` to disable/enable the new focus behaviour. 

## v0.2.2
### Added
- Logging support for Simulator, logs now appear for simulator launches as well

### Changed
- Fix: NSLog was not appearing earlier in device launches
- Open Simulator app when booting if not already open


## v0.2.1
### Added
- Better cleanup of ios-debug debugserver instances
- Support booted simulators with missing runtime

### Changed
- Minor fixes in logging


## v0.2.0
### Added
- Add support for attach request.
- Better logging in vscode output panel for troubleshooting.

### Removed
- Removed some undocumented commands exposed earlier.


## v0.1.0
### Added
- New command: `targetSdk`, which returns `iphoneos` or `iphonesimulator` depending on the selected target.
- A new sample project with vscode configuration example.

### Changed
- Update changelog
- Update readme


## v0.0.1
- Initial release