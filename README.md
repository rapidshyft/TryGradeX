# GradeX

Official release downloads for **GradeX** (Android). Website: [trygradex.app](https://trygradex.app)

[![Latest release](https://img.shields.io/github/v/release/rapidshyft/TryGradeX?label=latest)](https://github.com/rapidshyft/TryGradeX/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/rapidshyft/TryGradeX/total)](https://github.com/rapidshyft/TryGradeX/releases)

This repository only hosts builds, release notes and issue tracking. It does not contain the app's source code.

## Download

Get the latest build from the [Releases page](https://github.com/rapidshyft/TryGradeX/releases/latest).

### Which APK do I need?

Each release ships a universal APK and one smaller APK per CPU architecture.

| File | Use it when |
| --- | --- |
| `gradex-<version>-universal.apk` | You are not sure. Works on every supported device, but is the largest file. |
| `gradex-<version>-arm64-v8a.apk` | Almost all phones made since about 2017 (64-bit ARM). **Best choice for most people.** |
| `gradex-<version>-armeabi-v7a.apk` | Older or low-end phones (32-bit ARM). |
| `gradex-<version>-x86_64.apk` | Emulators and Chromebooks, and a few rare x86 tablets. |

Not sure about your phone? Install the universal APK.

## Install

1. Download the APK you need from the latest release.
2. Open the file on your phone. If Android asks, allow your browser or file manager to **install unknown apps**.
3. Tap **Install**. To update, install a newer APK over the old one. Your data is kept because all official releases use the same signing key.

### Verify your download (recommended)

Every release includes `SHA256SUMS.txt`. Compare the checksum of your download against it:

```bash
sha256sum gradex-<version>-arm64-v8a.apk
# or, to check everything you downloaded at once:
sha256sum -c SHA256SUMS.txt --ignore-missing
```

On Windows PowerShell: `Get-FileHash .\gradex-<version>-arm64-v8a.apk -Algorithm SHA256`

If the checksum doesn't match, delete the file and download it again from this repository. Only install GradeX from this repository or trygradex.app.

## Check for the latest version programmatically

[`latest.json`](latest.json) always describes the newest stable release: version, build number, download URLs and checksums for every APK. Its format is documented in [`latest.schema.json`](latest.schema.json).

```
https://raw.githubusercontent.com/rapidshyft/TryGradeX/main/latest.json
```

## Changelog

See [CHANGELOG.md](CHANGELOG.md) or the notes on each release.

## Support

- Found a bug or want a feature? [Open an issue](https://github.com/rapidshyft/TryGradeX/issues/new/choose).
- Security problem? Please don't open a public issue. See [SECURITY.md](SECURITY.md).

## Legal

GradeX is proprietary software. All rights reserved. The APKs in this repository are provided for installation and personal use only. Redistribution, modification and reverse engineering are not permitted without written permission. Privacy policy and terms: [trygradex.app](https://trygradex.app).
