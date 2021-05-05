# Changelog

## [1.0.18]

## Changed

- `AccountSettings` component: attribute renamed (and connected) for hiding the profile settings button. Attribute name is called now: `hideProfileSettings`. It is an optional attribute accepting boolean values.
- Updating dependecies.

## [1.0.17]

## Added

- New environment variable `REACT_APP_DISABLE_SIGNUP`. If defined as "true", nav-link from the navbar and from the login dialog is removed. If not defined or has any other value, it won't have any effect.

## Changed

- *BREAKING*: at signup request sent to the backend, it will send the instanceID as http header. This requires a participant-api (api-gateway) with v0.13.0 or later. This header field was included for providing the instanceID for reCaptcha validation.
- Updating project dependencies (case-web-ui), with minor improvements.

## [1.0.16]

### Changed

- Parse survey's validFrom and validUntil properties correctly. (gRPC sends them as strings, needs conversion)

- Updated case-web-ui dependency to deal with missing options in the single or multiple choice survey components more gracefully.

## [1.0.15]

### Changed

- Updated project dependecies

## [1.0.14]

### Added

- Store language selection into localStorage. When opening an other tab, reloading or revisiting the page, this selection will be picked up and used. If the item is not available in the local storage, the default language defined by the environment variable will be used.

### Changed

- Updated dependencies - case-web-ui's new version with support for multiple choice subtitles and markdown survey component