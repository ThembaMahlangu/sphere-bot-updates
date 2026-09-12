# sphere-bot-updates

The update manifest for Sphere Bot, and nothing else.

Sphere Bot is a private application. This repository exists only so an
installed copy can ask whether a newer version has been published, without the
application carrying a credential to read a private repository.

`latest.json` holds the published version, a link to its release, and the
identity of its installer:

```json
{
  "version": "v0.0.0",
  "url": "https://github.com/…/releases/tag/v0.0.0",
  "notes": "…",
  "asset": { "id": 0, "name": "Sphere_Bot_0.18.0_Setup.exe", "size": 0, "sha256": "…" }
}
```

That link resolves only for someone signed in with access to the release. The
application itself, its installer and its source are not here and are not
public. Downloading the installer from inside the app needs the user's own
GitHub token with read access to the release; the app checks the exact size and
SHA-256 above before it will run anything.

`latest.json` is written by the app repository's `npm run release`, after the
release and its installer exist, so it never names a release that is not there.
Until the first release it does not exist, and the app says so.
