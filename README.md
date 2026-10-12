# Sphere Bot updates

Public Windows installer releases and update metadata for Sphere Bot.

## Current Windows release: v1.2.1

[Download Sphere Bot v1.2.1](https://github.com/ThembaMahlangu/sphere-bot-updates/releases/download/v1.2.1/Sphere_Bot_1.2.1_Setup.exe) · [Release notes](https://github.com/ThembaMahlangu/sphere-bot-updates/releases/tag/v1.2.1)

- Installer: `Sphere_Bot_1.2.1_Setup.exe`
- Size: 123,113,725 bytes
- SHA-256: `3c870211da7f34eee55a8e72fbfd7c84434fa6f7424f1c7f8d1b1362a39b746f`

Only the current release is retained here. Application source is maintained separately. The installer is publicly downloadable without a GitHub token.

## Update feeds and versioning

`latest.json` describes the published Windows EXE release. Its version uses a `v` prefix, currently `v1.2.1`; the installer filename uses the same numeric version without the prefix. It includes the private application release URL and asset identity used by existing updater configurations. The corresponding installer is also published in this public repository. Sphere verifies its size and SHA-256 before installation. The release script publishes both installers before advancing the feed.

`store-latest.json` is a separate Microsoft Store channel. Its version is the last confirmed Microsoft-certified package, currently `1.0.14`, and uses no `v` prefix. Store ID: `9N7JZ3Z7XZ5B`. A newer EXE release or an unsigned Partner Center submission does not advance the certified Store feed. The v1.2.1 MSIX is prepared for submission; Microsoft supplies and installs Store updates after certification.

Release tags follow `vMAJOR.MINOR.PATCH`, such as `v1.2.1`. The MSIX manifest uses four numeric components, `1.2.1.0`. EXE and Store versions can differ while certification is pending.
