# Agency Website Studio - releases

Installer downloads and update metadata for **Agency Website Studio**, a
private Windows desktop app. This repository contains release binaries only:
no source code and no project data.

## Install

1. Open the [latest release](https://github.com/tabf9933/agency-website-studio-releases/releases/latest).
2. Download `Agency-Website-Studio-Setup-<version>.exe`.
3. Run it. Windows SmartScreen may show "Windows protected your PC" because
   the build is not code-signed: choose **More info**, then **Run anyway**.

The installed app checks this page for new stable versions at start-up and
every four hours, and offers **Download & install** when one is available.
Each download is verified against the SHA-512 in `latest.yml`.

## Files in each release

| File | Purpose |
| --- | --- |
| `Agency-Website-Studio-Setup-<version>.exe` | Installer (auto-updating) |
| `Agency-Website-Studio-Setup-<version>.exe.blockmap` | Differential-update index |
| `latest.yml` | Update metadata read by installed apps |
| `Agency-Website-Studio-Portable-<version>.exe` | Portable build (no installation, no auto-update) |

All project data stays on the PC it was created on, in
`%APPDATA%\Agency Website Studio\studio`. Updates never touch that folder.
