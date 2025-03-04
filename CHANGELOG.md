# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- CHANGELOG.
- CODE_OF_CONDUCT.

## [0.4.5] - 2019-05-15

### Changed
- Logging to use string format + params rather than interpolation.

### Fixed
- CommittedSnapshot name from ComittedSnapshot.
- AggregateRoot.EmitAll(...) to allow for more generic cases to be handled.

## [0.4.4] - 2019-05-09

### Added
- DomainEventMapper that maps from journal events to.
- AggregateTestFixture support for asserting aggregate root replies.

### Changed
- Access levels for aggregate root properties to be more private.

### Fixed
- Many hygienic  code factors reported by sonar cloud.

## [0.4.3] - 2019-04-28

### Added
- Akkatecture.TestFixture, a project for making testing your domain easier.

### Changed
- Akka versions from 1.3.11 to 1.3.12
- Tests from using test probe actors to use test probes.

### Fixed
- EventDefinition loading, thanks to [Damian-P](https://github.com/Damian-P)

## [0.4.2] - 2019-03-08

### Added
- SonarCloud code analysis on build.
- Full Azure Pipeline builds.
- Aggregate Event Tagger that tags persisted events as they get written to the journal.
- EmitAll(...) for aggregates to persist a sequence of events in a single transaction.

## [0.4.1] - 2019-01-22

### Changed
- Akka versions from 1.3.9 to 1.3.11.

## [0.4.0] - 2019-01-15

### Added
- Support for snapshots.

### Changed
- License headers for 2019.
- Package copyright for 2019.

### Removed
- IDE files from repository, thanks [siudeks](https://github.com/siudeks)

### Fixed
- Spelling errors in readme, thankes [Jacek Kuc](https://github.com/jk1980)



## [0.3.0] - 2018-11-11

### Added
- AspNet Core web sample in the examples folder.
- ISubscribeToAsync interface for Task returning receives for domain subscribers.
- Sourcelink so consumers can debug the package.
- Base64 GUID type, called Quid.
- Comitted Event serialization tests.
- AggregateName model.

### Changed
- Build status badges from appveyor to azure dev ops.

### Removed
- JetBrains Rider contentModel.xml from repository.

## [0.1.5] - 2018-09-15

### Added
- Azure Pipelines build definition.

## [0.1.4] - 2018-09-12

### Added
- Coverlet for code coverage metrics.
- CommittedEvent as the storage model for events.
- CorrelationId, and CausationId to Metadata container.
- VersionedTypeDefinitionService for obtaining definitions from varios message types. 

### Changed
- AggregateRoot message forwarding using Forward() instead of tell, thanks [@MarkEwer](https://github.com/MarkEwer).
- Akka package version to 1.3.9.


## [0.1.3] - 2018-05-23

### Fixed
- [Issue 21](https://github.com/Lutando/Akkatecture/issues/21) - Repository instantiated with a null parameter.

## [0.1.2] - 2018-05-20

### Added
- License headers to project source files with attributions to [EventFlow](https://github.com/eventflow/EventFlow).

### Changed
- Folder location of Simple example domain .

### Fixed
- Project vector graphics logo.
- Cluster README text.

## [0.1.1] - 2018-05-14

### Changed
- Explanation of akkatecture's features.
- Cluster example README.md.
- Simple example README.md.

### Fixed
- Walkthrough repository spawning.

## [0.0.25] - 2018-05-13

### Added
- Identity model.
- Entity model.
- AggregateRoot model which will be modeled as an actor.
- AggregateManager model to ensure singleton aggregate incarnations.
- Saga model which is modelled similarly to the AggregateRoot.
- SagaManager model to ensure singleton saga incarnations.
- Tests for all of the framework constructs.
- README containing the projects outlines.
- Examples that show how the framework works.
- Build definitions for appveyor and travis.
- MIT License.
- Project logo.

[Unreleased]: https://github.com/Lutando/Akkatecture/compare/0.4.5...HEAD
[0.4.5]: https://github.com/Lutando/Akkatecture/compare/0.4.4...0.4.5
[0.4.4]: https://github.com/Lutando/Akkatecture/compare/0.4.3...0.4.4
[0.4.3]: https://github.com/Lutando/Akkatecture/compare/0.4.2...0.4.3
[0.4.2]: https://github.com/Lutando/Akkatecture/compare/0.4.1...0.4.2
[0.4.1]: https://github.com/Lutando/Akkatecture/compare/0.4.0...0.4.1
[0.4.0]: https://github.com/Lutando/Akkatecture/compare/0.3.0...0.4.0
[0.3.0]: https://github.com/Lutando/Akkatecture/compare/0.1.5...0.3.0
[0.1.5]: https://github.com/Lutando/Akkatecture/compare/0.1.4...0.1.5
[0.1.4]: https://github.com/Lutando/Akkatecture/compare/0.1.3...0.1.4
[0.1.3]: https://github.com/Lutando/Akkatecture/compare/0.1.2...0.1.3
[0.1.2]: https://github.com/Lutando/Akkatecture/compare/0.1.1...0.1.2
[0.1.1]: https://github.com/Lutando/Akkatecture/compare/0.0.25...0.1.1
[0.0.25]: https://github.com/Lutando/Akkatecture/releases/tag/0.0.25
