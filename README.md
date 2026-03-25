# HA IDASEN Desk

Custom Home Assistant integration for IKEA IDASEN desks.

This repository vendors the `idasen_desk` integration so it can be installed via HACS
while depending on a patched `idasen-ha` fork that improves BLE proxy connectivity.

## What it changes

- installs `idasen-ha` from `pedropombeiro/idasen-ha`
- keeps the integration override in `custom_components/idasen_desk`
- works around BLE proxy authentication issues seen with ESPHome Bluetooth proxies

## Install with HACS

1. Open HACS in Home Assistant
2. Add this repository as a custom repository
3. Category: `Integration`
4. Install `HA IDASEN Desk`
5. Restart Home Assistant

## Notes

- This overrides Home Assistant's built-in `idasen_desk` integration
- The Python dependency is pulled from `pedropombeiro/idasen-ha`
- Intended as a temporary workaround until upstream fixes land
