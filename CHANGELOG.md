# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.3] - 2023-11-14
### Fixed
- Fixed launch install folder

## [0.1.2] - 2023-09-25
### Added
- Added `pose_publisher_bringup.launch` with environment variables use and namespace

### Fixed
- Creation of binaries on install and deb files 

### Changed
- Moved the launch file from `pose_publisher_launch.launch` to `pose_publisher.launch`

## [0.1.2-rc01] - 2023-09-25
### Added
- Added `pose_publisher_bringup.launch` with environment variables use and namespace

### Fixed
- Creation of binaries on install and deb files 

### Changed
- Moved the launch file from `pose_publisher_launch.launch` to `pose_publisher.launch`

## [0.1.1] - 2023-05-31
### Changed
- Changed prefix to id_robot
- Added map suffix
- Added base frame suffix
- Added `node_name` argument to launch

## [0.1.1-rc02] - 2023-05-31
### Changed
- Changed prefix to id_robot
- Added map suffix
- Added base frame suffix

## [0.1.1-rc01] - 2023-05-31
### Changed
- Added `node_name` argument to launch

## [0.1.0] - 2023-05-22

### Added

- The `launch` folder.
- The `.launch` file called `pose_publisher_launch.launch`.
-  The `CHANGELOG.md` file.
- Github actions for generation of the release
- Added github actions

### Changed

- Improved the code of the `pose_publisher.cpp` file, to provide the current position and orientation of the robot in the map with `PoseWithCovarianceStamped` format.
  - Changed the node name to `node_pose_publisher`. 
  - The parameters can be read and modified from the launch (`publish_frequency`, `map_frame`, `base_frame` and `topic_republish`).
  - Changed the type of the robot pose message to the format `PoseWithCovarianceStamped`.

- Updated the installation section of the`CMakeLists.txt` to be able to install the launch file of the `launch` folder.
- Updated the data of the `package.xml` file.

## [0.0.1] - 2020-05-20

### Added

- Original release.
