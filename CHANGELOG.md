# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Added
- Add new make target to support recovery test for FS stacks with disabled chaos monkey #32

## [1.0.0] - 2019-05-23

## [0.16.0] - 2019-05-23
### Added
- Add make target to check provisioning state
- Add make target to check provisioning state & readiness

### Changed
- Changed recovery make target to test orchestrator first
- Undo changes to the readiness make target

## [0.15.0] - 2019-05-23
### Added
- New Checks for checking EC2 Tag ComponentInitStatus

### Changed
- Extend existing readiness check to check for the ec2 tag ComponentInitStatus
- Add new Make targets to check provisioning state
- Restructured Make targets for readiness check
- Upgrade ruby_aem_aws to 1.3.0

## [0.14.1] - 2019-05-18
### Fixed
- Fix frozen string literal Rubocop violations

## [0.14.0] - 2019-04-23
### Changed
- Upgrade ruby_aem_aws to 1.2.1

### Removed
- Removed acceptance test for AEM logfiles access.log & request.log [#25]

### Fixed
- Fixed make targets for recovery test [#20] [#21]
- Fixed failing recovery test for Chaosmonkey & Orchestrator [#22]

## [0.13.0] - 2019-04-03
### Changed
- Modify test make targets to execute inspec binary from the PATH instead of via bundler
- Upgrade ruby_aem to 2.5.1, change deps versions to be exact

## [0.12.0] - 2019-04-01
### Added
- Add feature to terminate author-primary instance
- Add readiness check for AEM OpenCloud components Chaos Monkey & Orchestrator
- Add recovery testing for AEM OpenCloud components Chaos Monkey & Orchestrator

## [0.11.6] - 2018-11-05
### Added
- Add new checks for un/scheduling live-snapshots shinesolutions/aem-aws-stack-builder#212

## [0.11.5] - 2018-10-10
### Removed
- Remove test stack prefix in default config

## [0.11.4] - 2018-10-10
### Added
- Introduce dependencies bundle vendoring

## [0.11.3] - 2018-06-14
### Removed
- Remove default profile, move inspec check out of lint to avoid IO during CI run

## [0.11.2] - 2018-06-13
### Changed
- Content health check should fail when there is no instance

## [0.11.1] - 2018-06-01
### Added
- Add check for alarm states
- Add Checks for alarm state of contentHealthCheck

## [0.11.0] - 2018-05-31
### Added
- Add acceptance test support

## [0.10.0] - 2018-05-31
### Changed
- Set InSpec version to ~> 1.51.6 in order to use aws-sdk 3
- Drop support for Ruby 2.2

## 0.9.0 - 2018-05-20
### Added
- Initial version

[#20]: https://github.com/shinesolutions/inspec-aem-aws/issues/20
[#21]: https://github.com/shinesolutions/inspec-aem-aws/issues/21
[#22]: https://github.com/shinesolutions/inspec-aem-aws/issues/22
[#25]: https://github.com/shinesolutions/inspec-aem-aws/issues/25

[Unreleased]: https://github.com/shinesolutions/inspec-aem-aws/compare/1.0.0...HEAD
[1.0.0]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.16.0...1.0.0
[0.16.0]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.15.0...0.16.0
[0.15.0]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.14.1...0.15.0
[0.14.1]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.14.0...0.14.1
[0.14.0]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.13.0...0.14.0
[0.13.0]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.12.0...0.13.0
[0.12.0]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.11.6...0.12.0
[0.11.6]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.11.5...0.11.6
[0.11.5]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.11.4...0.11.5
[0.11.4]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.11.3...0.11.4
[0.11.3]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.11.2...0.11.3
[0.11.2]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.11.1...0.11.2
[0.11.1]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.11.0...0.11.1
[0.11.0]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.10.0...0.11.0
[0.10.0]: https://github.com/shinesolutions/inspec-aem-aws/compare/0.9.0...0.10.0
