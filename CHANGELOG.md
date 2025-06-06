# Changelog

## [2.4.3] - 2025-03-11

### Added

- Added additional parameters to build-map-layers script for creating rectangular map bounding areas

### Changed

- Adjust range for auto-orbit camera vertical and horizontal speed settings from -0.2 to 0.2

## [2.4.2] - 2025-03-10

### Changed

- Fixed typo in maps/build-map-layers.py

## [2.4.1] - 2025-03-10

### Changed

- Fixed bug in UTILS.setOrigin and UTILS.getXY calculations for lat/lon offsets

## [2.4.0] - 2025-03-06

### Added

- Added aerodrome and runway elevation visualization with ground projections
- Added `SKIES_ADSB_DEFAULT_ORIGIN_ELEVATION_METERS_OPTIONAL` environment variable
- Updated orbit and auto-orbit cameras to handle origin elevation
- Enhanced runway visibility with contrasting white material

### Changed

- Adjust height of origin labels
- Adjust starting default orbit camera settings
- Modified maps.js origins creation to include elevation data
- Modified build-map-layers script to include spatial join of aerodrome and runway data for elevation information

## [2.3.2] - 2025-03-05

### Changed

- Fixed typos in INSTALL.md

## [2.3.1] - 2025-03-05

### Changed

- Update project documentation

## [2.3.0] - 2025-03-02

### Added

- Added basic flight information to aircraft dialog using planespotters.net aircraft registration data

### Changed

- Hide FlightAware Flight info section in flight info dialog on empty JSON response
- Adjusted aircraft flight info dialog header text
- Fixed typo in update_flask_app.sh script
- Updated Flask app to return empty json response for flightInfo on failure to find FlightAware AeroAPI key
- Update docs with explanation of changes

## [2.2.1] - 2025-03-01

### Changed

- Changed build-map-layer.sh default environment variables prefix from `VITE_` to `SKIES_ADSB_`

## [2.2.0] - 2025-03-01

### Added

- Added "Auto-Orbit" camera mode
- Added "Auto-Orbit" camera controls to dat-gui settings
- Added new gif recording of v2.2.0

### Changed

- Changed default environment variables prefix from `VITE_` to `SKIES_ADSB_`
- Adjusted urban layer Y position
- Updated automation + build scripts to use `SKIES_ADSB_` environment variables
- Updated docs
- Misc clean up

## [2.1.8] - 2025-02-24

### Changed

- Updated troika-three-text library to 0.52.3
- Fixed bug in Aircraft.hasExpired() causing incorrect aircraft expiration

## [2.1.7] - 2025-02-20

### Changed

- Fixed error in UTILS.getXY due to typo

## [2.1.6] - 2025-02-20

### Changed

- Misc documentation clean up

## [2.1.5] - 2025-02-20

### Changed

- Update project README.md with link to SDR Enthusiasts compatible Docker container

## [2.1.4] - 2025-02-19

### Changed

- Update project README.md with Docker container notice.

## [2.1.3] - 2025-02-19

### Changed

- Misc documentation clean up

## [2.1.2] - 2025-02-19

### Changed

- Update DEVELOPMENT.md Flask app update instructions

## [2.1.1] - 2025-02-19

### Changed

- Fixed script initialization issue in install-skies-adsb.sh

## [2.1.0] - 2025-02-19

### Added

- Added readsb RTL-SDR driver option in installation process

### Changed

- Fixed aircraft TTL bug caused by improper type check
- Simplified Raspberry Pi installation process
  - Removed need for manual script editing
  - Added command line options
  - Renamed `install.sh` to `install-skies-adsb.sh`
- Updated documentation
  - Updated INSTALL.md and RPI-INSTALL-GUIDE.md
  - Renamed LOCALHOST-SETUP-GUIDE.md to LOCALHOST-HEADLESS-SETUP-GUIDE.md

## [2.0.9] - 2025-02-16

## Changed

- Fixed INSTALL.md table of contents.

## [2.0.8] - 2025-02-16

## Changed

- Misc documentation clean up

## [2.0.7] - 2025-02-16

## Changed

- Updated use_existing_adsb.sh script
  - added --host option when launching Vite in order to automatically setup Network IP for development server
  - removed --open option in order to prevent failure if run in a headless setup
- Updated utils.js to use window.location.hostname instead of hardcoded localhost string for Localhost setups
- Updated RPI and Localhost installation guides and consolidated redundant sections into the docs/INSTALL.md guide
- Misc documentation clean up

## [2.0.6] - 2025-02-15

## Changed

- Update docs/INSTALL.md repo url

## [2.0.5] - 2025-02-15

## Changed

- Updated project README.md

## [2.0.4] - 2025-02-15

## Added

- Added documentation for enabling remote access to Raspberry Pi dump1090-mutability
- Added documentation for customizing default visualization settings
- Added documentation for create map layers for larger coverage areas
- Added --skip-aerodromes option to build-map-layers.py script

## Changed

- Refactored many default settings to be user configurable via src/utils.js file
- Updated instructions on how to work with existing ADS-B receivers
- Updated project README.md
- Update Vite to 5.4.14
- Update @mapbox/sphericalmercator to 2.0.1

## [2.0.3] - 2025-02-11

### Changed

- Updated project README.md
- Updated DEVELOPMENT.md

## [2.0.2] - 2025-02-11

### Changed

- Fixed typo in BUILD-MAPS.md

## [2.0.1] - 2025-02-11

### Added

- Build-map-layers.sh bash automation script

### Changed

- Misc documentation typo fixes
- Updated map layer building instructions to use build-map-layers.sh script

## [2.0.0] - 2025-02-02

### Added

- Generate custom GeoJSON map layers from Natural Earth, FAA, and OpenStreetMap data
- Aircraft trails visualization
- Enhanced map renderer with multi-layer vector support:
  - Aerodromes
  - Airspaces
  - States / Provinces
  - Counties
  - Urban areas
  - Roads
  - Rivers
  - Lakes
- New aircraft follow camera controls
- Added project sponsor button via Buy Me a Coffee

### Changed

- Major codebase refactoring and simplification
- Simplified setup and build process
- Updated documentation to reflect migration to Raspberry Pi OS 64-bit
- Update project screenshots and recordings
- Updated the project README
- Updated METAR api call to use new aviationweather.gov JSON endpoint

### Removed

- Removed outdated CLOUDFLARE-TUNNEL.md documentation

## [1.3.2] - 2024-12-24

### Changed

- Misc refactoring of main.js

## [1.3.1] - 2024-12-24

### Changed

- Misc refactoring of aircraft.js

## [1.3.0] - 2024-12-23

### Changed

- Refactored aircraft follow camera logic and controls

## [1.2.5] - 2024-03-19

### Removed

- Removed TODO

## [1.2.4] - 2024-03-12

### Changed

- Updated Raspberry Pi Install Guide

## [1.2.3] - 2024-03-12

### Changed

- Updated localhost Install Guide

## [1.2.2] - 2024-03-10

### Changed

- Updated Raspberry Pi Install Guide with additional Vite environment variable usage instructions

## [1.2.1] - 2024-03-10

### Changed

- Updated Raspberry Pi Install Guide with Vite environment variable usage instructions

## [1.2.0] - 2024-03-10

### Changed

- Migrated project build system to use Vite instead of webpack
- Updated project documentation to reflect usage of Vite

## [1.1.1] - 2023-11-22

### Changed

- Misc updates to project README

## [1.1.0] - 2023-11-18

### Changed

- Migrated flask app to use FlightAware AeroAPI v4

## [1.0.2] - 2022-05-22

### Changed

- Disable user-select CSS on aircraft dialog to prevent loss of focus on main rendering widow

## [1.0.1] - 2022-05-15

### Changed

- Disable user-select CSS on HUD buttons to prevent loss of focus on main rendering widow

## [1.0.0] - 2022-05-14

- First stable release
