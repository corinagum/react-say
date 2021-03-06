# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.1.1] - 2018-10-31
### Changed
- Bump to [`event-as-promise@1.0.5`](https://npmjs.com/package/event-as-promise/v/1.0.5)

## [1.1.0] - 2018-10-28
### Added
- Utterance queue are now controlled by `<Composer>` instance, instead of native `speechSynthesis` for better browser compatibility
   - Chrome: does not fire `start` and `end` events if `speak`/`cancel` are called too fast
   - Safari: does not play audio or `start` event if the first utterance is not triggered by user event
- Unmounting elements will cancel the speech in progress or pending speech

### Changed
- Lerna bootstrap will no longer hoist
- Playground: Bump to [`react@16.6.0`](https://npmjs.com/package/react/v/16.6.0), [`react-dom@16.6.0`](https://npmjs.com/package/react-dom/v/16.6.0), and [`react-scripts@2.0.5`](https://npmjs.com/package/react-scripts/v/2.0.5)

### Fixed
- Null reference on `props.speechSynthesis`

## [1.0.0] - 2018-07-09
### Added
- Initial release
