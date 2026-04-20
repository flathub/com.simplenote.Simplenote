# com.simplenote.Simplenote

Flatpak build recipe for **Simplenote**, the simplest way to keep notes across all your devices.

## Build Status
[![Flathub Status](https://img.shields.io/flatpak/v/com.simplenote.Simplenote?label=Flathub)](https://flathub.org/apps/details/com.simplenote.Simplenote)
![Build passing](https://img.shields.io/badge/build-passing-brightgreen)

## Description
This repository contains the manifest and necessary files to package Simplenote for [Flathub](https://flathub.org). Simplenote features:
* **Automatic Syncing:** Keep your notes updated on all devices.
* **Organization:** Custom tags and quick search.
* **Collaboration:** Share notes or publish them online.
* **Markdown Support:** Preview and publish in Markdown format.

## Maintenance Notes
This package uses the official AppImage from Automattic to ensure maximum compatibility and stability.

### Technical Details:
* **Runtime:** Freedesktop 24.08
* **Base:** Electron
* **Architecture:** x86_64 and aarch64

## How to build locally
If you want to test this build on your local machine (e.g., Linux Mint), ensure you have `flatpak-builder` installed:

```zsh
# Clone the repository
git clone --recursive [https://github.com/tuo-username/com.simplenote.Simplenote.git](https://github.com/tuo-username/com.simplenote.Simplenote.git)
cd com.simplenote.Simplenote

# Build and install locally
flatpak-builder --user --install --force-clean build com.simplenote.Simpleno
te.yaml
