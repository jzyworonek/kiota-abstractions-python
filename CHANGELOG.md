# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.3.1] - 2024-03-05

### Added

### Changed

- Fixed a bug with serialization of parsable multipart body due to unsubscriptable argument type.

## [1.3.0] - 2024-02-28

### Added
- Added multipart body class to support multipart serialization. [microsoft/kiota#3030](https://github.com/microsoft/kiota/issues/3030)

### Changed

## [1.2.0] - 2024-01-31

### Added
- Added methods in request information to reduce the amount of code being generated. [microsoft/kiota#3695](https://github.com/microsoft/kiota/issues/3695)

### Changed
- Fixed an issue where path and query parameters of enum type would not be expanded properly. [microsoft/kiota#3783](https://github.com/microsoft/kiota/issues/3783)

## [1.1.0] - 2024-01-25

### Added
- Added an abstract class to mark composed type wrappers and facilitate serialization.

### Changed

## [1.0.0] - 2023-10-31

### Added

### Changed
- GA release

## [0.9.1] - 2023-10-25

### Added

### Changed
- Initialize headers in BaseRequestConfiguration to a HeadersCollection instance

## [0.9.0] - 2023-10-10

### Added
- Added a content type parameter to the set stream content method in request information.

### Changed
- Added dedicated HeadersCollection class to manage request headers.

## [0.8.7] - 2023-10-05

### Added
- Added a try_add method for request headers

### Changed

## [0.8.6] - 2023-09-19

### Added

### Changed
- Updated BaseRequestBuilder to set the raw url value if provided.

## [0.8.5] - 2023-09-15

### Added

### Changed
- Fix error where updating an attribute of a nested backed model marks all other attributes as changed.

## [0.8.4] - 2023-09-14

### Added

### Changed
- Fix error when instantiating BackedModel using positional and keyword arguments

## [0.8.3] - 2023-09-13

### Added

### Changed
- Fix error representation when APIError class has no error attribute.

## [0.8.2] - 2023-09-13

### Added

### Changed
- Switched from uritemplate to std-uritemplate for URI templating.
- Handles exception thrown when APIError class has no error attribute.

## [0.8.1] - 2023-09-01

### Added
- Added opentelemetry to project dependencies.

### Changed

## [0.8.0] - 2023-08-24

### Added
- Added opentelemetry to support observability.
- Added an additional parameter to authentication methods to carry contextual information.

### Changed

## [0.7.1] - 2023-08-09

### Added

### Changed
- Set the default value for the `is_initialization_completed` parameter in the `InMemoryBackingStore` class to be `False` and use the
`__post_init__` method of backed model to set it to `True`.
- Changed the string representation of the `APIError` class to be more descriptive.

## [0.7.0] - 2023-07-27

### Added
- Added an abstract translator method that should convert a `RequestInformation` object into the native client HTTP request object.
- Enable backing store for Python.

### Changed

## [0.6.0] - 2023-06-27

### Added
- API key authentication provider.

### Changed

## [0.5.5] - 2023-06-26

### Added

### Changed

- Changed BaseRequesBuilder class to be instantiable.
- Renamed RequestConfiguration class to BaseRequestConfiguration.

## [0.5.4] - 2023-06-22

### Added

- Added a base request builder and a request configuration class to reduce the amount of code being generated.

### Changed

## [0.5.2] - 2023-06-05

### Added

### Changed

- Changed Parsable and APIError to dataclasses.
- Added support for merging of object values for intersection types

## [0.5.1] - 2023-04-29

### Added

- Adds the response headers to the APIError class.

### Changed

## [0.5.0] - 2023-02-07

### Added

- Added support for multi-valued request headers.

### Changed


## [0.4.0] - 2023-02-06

### Added

### Changed

- Added a response status code property to the API exception class.

## [0.2.3] - 2023-01-17

### Added

### Changed
- Changes the ResponseHandler parameter in RequestAdapter to be a RequestOption