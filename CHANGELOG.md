# Changelog

All noteworthy changes to this project will be documented in this file.

The format is based on [Keep a Changelog][1].

This project **tries to** adhere to [Semantic Versioning][2]. More specifically,
the major version follows that of the [upstream][3] repository. If these version
numbers are the same, then the configuration model "should" also be the same.
Software and runtimes added/removed will bump the minor version. Other
miscellaneous changes will bump the patch version.

[1]: http://keepachangelog.com/en/1.0.0/
[2]: http://semver.org/spec/v2.0.0.html
[3]: https://github.com/martinanderssondotcom/dev-mini

## [Unreleased]

Changed

- Nothing, yet!

## [2.1.0] - 2018-04-22

### Changed

- Merged `v2.1.0` from `martinanderssondotcom/dev-mini` (see [upstream changelog][2.1.0-1]).

[2.1.0-1]: https://github.com/martinanderssondotcom/dev-mini/blob/master/CHANGELOG.md#210---2018-04-22

### Fixed

- GitKraken installs not thru `apt`, but rather, thru `snap`
  ([issue #1][unreleased-1]).

[unreleased-1]: https://github.com/martinanderssondotcom/dev-java/issues/1

## 2.0.0 - 2018-03-23

First tag.

### Files present

- `provisioning/playbook.yml`
- `.gitignore`
- `Vagrantfile`
- `CHANGELOG.md`
- `LICENSE`
- `README.md`

[Unreleased]: https://github.com/martinanderssondotcom/dev-java/compare/v2.1.0...HEAD
[2.1.0]: https://github.com/martinanderssondotcom/dev-java/compare/v2.0.0...v2.1.0