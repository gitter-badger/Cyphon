# Change log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/). This project adheres to [Semantic Versioning](http://semver.org/).


<a name="Unreleased"></a>
## [Unreleased]


<a name="1.4.2"></a>
## [1.4.2](https://github.com/dunbarcyber/cyphon/compare/1.4.1...1.4.2) (2017-08-21)

### Changed

- **monitors**: status of Monitors is updated on save [PR #186](https://github.com/dunbarcyber/cyphon/pull/186) ([18a4ab8](https://github.com/dunbarcyber/cyphon/commit/18a4ab8))

### Fixed

- **engines.elasticsearch**: fixed default value for Elasticsearch timeout ([22cd0b5](https://github.com/dunbarcyber/cyphon/commit/22cd0b5))


<a name="1.4.1"></a>
## [1.4.1](https://github.com/dunbarcyber/cyphon/compare/1.4.0...1.4.1) (2017-08-14)

### Fixed

- **monitors**: fixed bug that prevented red monitors from changing back to green [PR #184](https://github.com/dunbarcyber/cyphon/pull/184) ([28f1f64](https://github.com/dunbarcyber/cyphon/commit/28f1f64))


<a name="1.4.0"></a>
## [1.4.0](https://github.com/dunbarcyber/cyphon/compare/1.3.0...1.4.0) (2017-08-14)

### Added

- **alerts**: ``Alert.muzzle_hash`` field [PR #130](https://github.com/dunbarcyber/cyphon/pull/130) ([efaa627](https://github.com/dunbarcyber/cyphon/commit/efaa627))
- **alerts**: email notifications for Alert comments [PR #139](https://github.com/dunbarcyber/cyphon/pull/139) ([bd968c1](https://github.com/dunbarcyber/cyphon/commit/bd968c1))
- **cyphon.choices**: range choices ([1c414aa](https://github.com/dunbarcyber/cyphon/commit/1c414aa))
- **cyphon.version**: added Cyphon version to headers ([40c123f](https://github.com/dunbarcyber/cyphon/commit/40c123f), [08ff612](https://github.com/dunbarcyber/cyphon/commit/08ff612))
- **docs**: search query docs ([bfe06fd](https://github.com/dunbarcyber/cyphon/commit/bfe06fd))
- **docs**: Alert bulk admin docs ([3d963b1](https://github.com/dunbarcyber/cyphon/commit/3d963b1))
- **docs**: secrets management ([7cdddc2](https://github.com/dunbarcyber/cyphon/commit/7cdddc2), [4a110fc](https://github.com/dunbarcyber/cyphon/commit/4a110fc))
- **query.search**: search query classes ([76dac5d](https://github.com/dunbarcyber/cyphon/commit/76dac5d))
- **query.search**: search endpoint [PR #136](https://github.com/dunbarcyber/cyphon/pull/136) ([56bd2ce](https://github.com/dunbarcyber/cyphon/commit/56bd2ce))
- **requirements.txt**: boto3, django-s3-storage, and ec2-metadata packages [PR #134](https://github.com/dunbarcyber/cyphon/pull/134) ([62751ee](https://github.com/dunbarcyber/cyphon/commit/62751ee))
- **sifter.sieves**: numeric rules [PR #129](https://github.com/dunbarcyber/cyphon/pull/129) ([0fba6f4](https://github.com/dunbarcyber/cyphon/commit/0fba6f4))
- **utils.parserutils**: ``merge_dict()`` and ``abridge_dict()`` functions ([44e9fcd](https://github.com/dunbarcyber/cyphon/commit/44e9fcd))
- **utils.settings**: default configuration and pull secrets from SSM ([7796fc9](https://github.com/dunbarcyber/cyphon/commit/7796fc9))

### Changed

- **alerts**: only fields defined in Container are shown in Alert data [PR #127](https://github.com/dunbarcyber/cyphon/pull/127) ([cdd0c68](https://github.com/dunbarcyber/cyphon/commit/cdd0c68))
- **alerts**: doc_id field included in serialized Alert detail [PR #145](https://github.com/dunbarcyber/cyphon/pull/145) ([c62dca4](https://github.com/dunbarcyber/cyphon/commit/c62dca4))
- **cyphon.settings, engines.elasticsearch**: support more Elasticsearch configuration options [PR #170](https://github.com/dunbarcyber/cyphon/pull/170) ([91312dc](https://github.com/dunbarcyber/cyphon/commit/91312dc), [51a2a68](https://github.com/dunbarcyber/cyphon/commit/51a2a68))
- **watchdogs**: removed Alert table locking [PR #130](https://github.com/dunbarcyber/cyphon/pull/130) ([efaa627](https://github.com/dunbarcyber/cyphon/commit/efaa627))

### Fixed

- **cyphon.settings**: corrected ``backupCount`` setting for logging handlers ([e150db1](https://github.com/dunbarcyber/cyphon/commit/e150db1))

### Removed

- **docs**: removed Docker instructions ([87012e2](https://github.com/dunbarcyber/cyphon/commit/87012e2))


<a name="1.3.0"></a>
## [1.3.0](https://github.com/dunbarcyber/cyphon/compare/1.2.0...1.3.0) (2017-06-28)

### Added

- Tox configuration - [PR #92](https://github.com/dunbarcyber/cyphon/pull/92) ([1299f58](https://github.com/dunbarcyber/cyphon/commit/1299f58))
- **docs:** added screenshots to overview ([f807d4a](https://github.com/dunbarcyber/cyphon/commit/f807d4a))
- **docs:** added FAQs page ([7488729](https://github.com/dunbarcyber/cyphon/commit/7488729))
- **docs:** added support page ([f022900](https://github.com/dunbarcyber/cyphon/commit/f022900))
- **docs:** added testing page to dev guide ([a9e6a4e](https://github.com/dunbarcyber/cyphon/commit/a9e6a4e))
- **docs:** added Twitter tutorial - [PR #113](https://github.com/dunbarcyber/cyphon/pull/113) ([56e7e74](https://github.com/dunbarcyber/cyphon/commit/56e7e74))
- **lab.sentiment:** added sentiment analysis - [PR #108](https://github.com/dunbarcyber/cyphon/pull/108) ([859f9b7](https://github.com/dunbarcyber/cyphon/commit/859f9b7))

### Changed

- upgraded to Django 1.11 - [PR #101](https://github.com/dunbarcyber/cyphon/pull/101) ([d4cd82b](https://github.com/dunbarcyber/cyphon/commit/d4cd82b))
- **alerts:** Alerts can be filtered by Warehouse ([19c37e9](https://github.com/dunbarcyber/cyphon/commit/19c37e9))
- **ambassador.platforms:** Platforms are ordered by name ([0381433](https://github.com/dunbarcyber/cyphon/commit/0381433))
- **bottler.tastes**: Tastes are ordered by container ([972a35c](https://github.com/dunbarcyber/cyphon/commit/972a35c))
- **contexts:** Contexts are ordered by name ([174eb81](https://github.com/dunbarcyber/cyphon/commit/174eb81))
- **parsers:** Parsers are ordered by name ([4daf0fa](https://github.com/dunbarcyber/cyphon/commit/4daf0fa))
- **sifter.condensers:** Condensers are ordered by name ([4daf0fa](https://github.com/dunbarcyber/cyphon/commit/4daf0fa))

### Fixed

- **Dockerfile**: fixed issue with proj4 library - [PR #106](https://github.com/dunbarcyber/cyphon/pull/106) ([900760d](https://github.com/dunbarcyber/cyphon/commit/900760d))
- **docs**: mocked out GDAL in Sphinx build - [PR #107](https://github.com/dunbarcyber/cyphon/pull/107) ([d1ab82e](https://github.com/dunbarcyber/cyphon/commit/d1ab82e))
- **sifter.chutes**: added Chute ID to admin list display ([2abb5f0](https://github.com/dunbarcyber/cyphon/commit/2abb5f0))
- **tests**: fixed URL for SauceLabs - [PR #112](https://github.com/dunbarcyber/cyphon/pull/112) ([a2feddd](https://github.com/dunbarcyber/cyphon/commit/a2feddd))

### Removed

- **docs:** removed list of dependencies ([b2678bb](https://github.com/dunbarcyber/cyphon/commit/b2678bb))
- **docs:** removed testing env from starter-docker.txt ([cf766b8](https://github.com/dunbarcyber/cyphon/commit/cf766b8))


<a name="1.2.0"></a>
## [1.2.0](https://github.com/dunbarcyber/cyphon/compare/1.1.3...1.2.0) (2017-06-05)

### Added

- **cyclops:** added built-in Cyclops integration ([d4baf47](https://github.com/dunbarcyber/cyphon/commit/d4baf47), [2f7f574](https://github.com/dunbarcyber/cyphon/commit/2f7f574))
- **cyphon.dashboard:** added Categories to admin dashboard ([dbfb658](https://github.com/dunbarcyber/cyphon/commit/dbfb658))
- **cyphon.dashboard:** added "Latest Cyphon News" to admin dashboard ([910f2fd](https://github.com/dunbarcyber/cyphon/commit/910f2fd))
- **cyphon.settings:** added settings for Cyclops integration ([d4baf47](https://github.com/dunbarcyber/cyphon/commit/d4baf47), [2f7f574](https://github.com/dunbarcyber/cyphon/commit/2f7f574))
- **docs:** added docs for push notifications ([1c98e3b](https://github.com/dunbarcyber/cyphon/commit/1c98e3b))
- **docs:** added docs for configuring Cyclops ([1c98e3b](https://github.com/dunbarcyber/cyphon/commit/1c98e3b))

### Changed

- **Dockerfile:** Docker image is now based on Alpine Linux ([517af76](https://github.com/dunbarcyber/cyphon/commit/517af76))
- **alarms, monitors, watchdogs:** Monitors and Watchdogs are now sorted by name ([0c98fc9](https://github.com/dunbarcyber/cyphon/commit/0c98fc9))
- **sifter:** all Rules and SieveNodes are now sorted by name ([b9128f3](https://github.com/dunbarcyber/cyphon/commit/b9128f3))

### Fixed

- **ambassador.passports:** fixed storage directory for Passport file field ([e97fd33](https://github.com/dunbarcyber/cyphon/commit/e97fd33))


<a name="1.1.3"></a>
## [1.1.3](https://github.com/dunbarcyber/cyphon/compare/1.1.2...1.1.3) (2017-05-27)

### Added

- **categories:** added REST API endpoint for Categories ([360dc56](https://github.com/dunbarcyber/cyphon/commit/360dc56))
- **docs:** added email tutorial ([d8fd982](https://github.com/dunbarcyber/cyphon/commit/d8fd982))
- **docs:** added Logstash tutorial ([69769f9](https://github.com/dunbarcyber/cyphon/commit/69769f9), [1c56516](https://github.com/dunbarcyber/cyphon/commit/1c56516))
- **docs:** added minimum system requirements ([d00b95](https://github.com/dunbarcyber/cyphon/commit/d00b95))

### Fixed

- **.gitignore:** fixed directory for Cyphon settings ([e863c4a](https://github.com/dunbarcyber/cyphon/commit/e863c4a))
- **bottler.bottles:** fixed bug with EmbeddedDocumentFields ([6fd70f5](https://github.com/dunbarcyber/cyphon/commit/6fd70f5))
- **docs:** updated instructions for Elasticsearch data directory ([03c3446](https://github.com/dunbarcyber/cyphon/commit/03c3446))


<a name="1.1.2"></a>
## [1.1.2](https://github.com/dunbarcyber/cyphon/compare/1.1.1...1.1.2) (2017-05-16)

### Fixed

- **sifter.mungers:** modified `Munger.process()` to avoid errors when processing mail ([84f8871](https://github.com/dunbarcyber/cyphon/commit/84f8871))


<a name="1.1.1"></a>
## [1.1.1](https://github.com/dunbarcyber/cyphon/compare/1.1.0...1.1.1) (2017-05-16)

### Fixed

- **alerts:** modified `Alert.save()` so that `location` and `content_date` are added the Alert to even if the Alert already has `data`, and a `title` with a default value is refreshed ([a37d9eb](https://github.com/dunbarcyber/cyphon/commit/a37d9eb))
- **alerts:** `Alert.saved_data` is no longer cached ([9fdba5d](https://github.com/dunbarcyber/cyphon/commit/9fdba5d))
- **engines.elasticsearch.engine:** Elasticsearch indexes are refreshed prior to searching by id ([65d72e2](https://github.com/dunbarcyber/cyphon/commit/65d72e2))
- **watchdogs:** Watchdogs pass data directly to Muzzles instead of fetching saved data, avoiding race condition in Logstash ([7c5a53d](https://github.com/dunbarcyber/cyphon/commit/7c5a53d))


<a name="1.1.0"></a>
## [1.1.0](https://github.com/dunbarcyber/cyphon/compare/1.0.3...1.1.0) (2017-05-14)

### Added

- **cyphon.documents:** added `DocumentOj` class for handling document references ([d701762](https://github.com/dunbarcyber/cyphon/commit/d701762))
- **receiver.receiver:** added RabbitMQ queue consumers for DataChutes, Watchdogs, and Monitors ([d701762](https://github.com/dunbarcyber/cyphon/commit/d701762))
- **target.followees:** added `get_by_natural_key()` method for Followees, Accounts, LegalNames, and Aliases ([0f8f3b8](https://github.com/dunbarcyber/cyphon/commit/0f8f3b8))
- **target.locations:** added `get_by_natural_key()` method for Locations ([2b5199d](https://github.com/dunbarcyber/cyphon/commit/2b5199d))
- **target.searchterms:** added `get_by_natural_key()` method for SearchTerms ([813c1ca](https://github.com/dunbarcyber/cyphon/commit/813c1ca))

### Fixed

- **sifter.condensers:** removed extra inline Fitting form ([10f53ce](https://github.com/dunbarcyber/cyphon/commit/10f53ce))
- **sifter.logsifter:** fixed "Test this rule" tool on LogRule admin page ([751d55b](https://github.com/dunbarcyber/cyphon/commit/751d55b))


<a name="1.0.3"></a>
## [1.0.3](https://github.com/dunbarcyber/cyphon/compare/1.0.2...1.0.3) (2017-05-14)

### Added

- **bottler:** added `get_by_natural_key()` method for BottleFields and LabelFields ([68c2a15](https://github.com/dunbarcyber/cyphon/commit/68c2a15))
- **contexts:** added `get_by_natural_key()` method for Contexts and ContextFields ([09ff0b8](https://github.com/dunbarcyber/cyphon/commit/09ff0b8))
- **cyphon.dashboard:** added Protocols and Constance to admin dashboard ([ee34361](https://github.com/dunbarcyber/cyphon/commit/ee34361), [0cbbb15](https://github.com/dunbarcyber/cyphon/commit/0cbbb15))
- **entrypoints:** added conditional for loading example fixtures ([a0efa1f](https://github.com/dunbarcyber/cyphon/commit/a0efa1f))
- **watchdogs:** added `get_by_natural_key()` method for Triggers ([8312713](https://github.com/dunbarcyber/cyphon/commit/8312713))

### Changed

- **cyphon.tests.functional_tests:** enabled functional tests to run in a Selenium 3 Docker container ([fe170cc](https://github.com/dunbarcyber/cyphon/commit/fe170cc))
- **docs:** replaced install instructions for Docker Engine with those for Docker Community Edition ([4aa080c](https://github.com/dunbarcyber/cyphon/commit/4aa080c))

### Fixed

- **responder.actions.filters:** fixed ActionFilterBackend to allow access to Actions associated with public Passports ([952464b](https://github.com/dunbarcyber/cyphon/commit/952464b))

### Removed

- **fixtures:** removed default fixtures, since these are provided in [Cyphondock](https://github.com/dunbarcyber/cyphondock/) ([ba25363](https://github.com/dunbarcyber/cyphon/commit/ba25363))

### Security

* **entrypoints**: Celery beat and worker are now run without superuser privileges ([8f18b42](https://github.com/dunbarcyber/cyphon/commit/8f18b42))


<a name="1.0.2"></a>
## [1.0.2](https://github.com/dunbarcyber/cyphon/compare/1.0.1...1.0.2) (2017-04-07)

### Added

- **docs:** added CHANGELOG ([baf76ae](https://github.com/dunbarcyber/cyphon/commit/baf76ae))

### Changed

- **docs:** changed AUTHORS to markdown ([beb0d87](https://github.com/dunbarcyber/cyphon/commit/beb0d87))

### Fixed

- **contexts:** fixed issue with ContextFilters handling nested fields ([ac58553](https://github.com/dunbarcyber/cyphon/commit/ac58553))
- **cyphon.settings:** applied fix for [django-filter issue #562](https://github.com/carltongibson/django-filter/issues/562) ([7f09009](https://github.com/dunbarcyber/cyphon/commit/7f09009))
- **engine.mongodb.engine:** fixed issue with MongoDB queries ([ea1b043](https://github.com/dunbarcyber/cyphon/commit/ea1b043))
- **watchdogs:** fixed issue with Muzzles handling nested fields ([fe30e75](https://github.com/dunbarcyber/cyphon/commit/fe30e75))


<a name="1.0.1"></a>
## [1.0.1](https://github.com/dunbarcyber/cyphon/compare/1.0.0...1.0.1) (2017-04-05)

### Changed

- **docs:** added disclaimer to securing-cyphon.txt ([39e2d65](https://github.com/dunbarcyber/cyphon/commit/39e2d65), [4cdc5e2](https://github.com/dunbarcyber/cyphon/commit/4cdc5e2), [c811257](https://github.com/dunbarcyber/cyphon/commit/c811257), [b1722c3](https://github.com/dunbarcyber/cyphon/commit/b1722c3))
- **docs:** updated favicon ([14ab3ff](https://github.com/dunbarcyber/cyphon/commit/14ab3ff))

### Fixed

- **docs:** deleted obsolete appuser docs ([ea3e5f3](https://github.com/dunbarcyber/cyphon/commit/ea3e5f3))
- **query.reservoirqueries.reservoirqueries:** fixed bug affecting Followee-based Filters ([b6a8fd9](https://github.com/dunbarcyber/cyphon/commit/b6a8fd9))


<a name="1.0.0"></a>
## [1.0.0](https://github.com/dunbarcyber/cyphon/releases/tag/1.0.0) (2017-04-04)
