# Sphere Bot updates

Public Windows installer releases and update metadata for Sphere Bot.

## Current Windows release: v1.0.15

[Download Sphere Bot v1.0.15](https://github.com/ThembaMahlangu/sphere-bot-updates/releases/download/v1.0.15/Sphere_Bot_1.0.15_Setup.exe) · [Release notes](https://github.com/ThembaMahlangu/sphere-bot-updates/releases/tag/v1.0.15)

- Installer: `Sphere_Bot_1.0.15_Setup.exe`
- Size: 123,076,751 bytes
- SHA-256: `8a25f9d01754f9382855f78104845fb064f4adfced15c6b53710ac88dd81f7b5`

Only the current release is retained here. Application source is maintained separately. The installer is publicly downloadable without a GitHub token.

## Update feeds and versioning

`latest.json` describes the published Windows EXE release. Its version uses a `v` prefix, currently `v1.0.15`; the installer filename uses the same numeric version without the prefix. It includes the private application release URL and asset identity used by existing updater configurations. The corresponding installer is also published in this public repository. Sphere verifies its size and SHA-256 before installation. The release script publishes both installers before advancing the feed.

`store-latest.json` is a separate Microsoft Store channel. Its version is the last confirmed Microsoft-certified package, currently `1.0.14`, and uses no `v` prefix. Store ID: `9N7JZ3Z7XZ5B`. A newer EXE release or an unsigned Partner Center submission does not advance the certified Store feed. Microsoft supplies and installs Store updates.

Release tags follow `vMAJOR.MINOR.PATCH`, such as `v1.0.15`. EXE and Store versions can differ while certification is pending.
