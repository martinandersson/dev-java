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

### Fixed

- GitKraken installs not thru `apt`, but rather, thru `snap`
  ([issue #1][unreleased-1]).

[unreleased-1]: https://github.com/martinanderssondotcom/dev-java-9/issues/1

## 2.0.0 - 2018-03-23

First tag.

### Files present

- `provisioning/playbook.yml`
- `.gitignore`
- `Vagrantfile`
- `CHANGELOG.md`
- `LICENSE`
- `README.md`

[Unreleased]: https://github.com/martinanderssondotcom/dev-java-9/compare/v2.0.0...HEAD