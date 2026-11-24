# How to publish a new DORA version

Full steps (building, version numbers, signing key) are in `GPS TRACKER\RELEASING.md`. In short:

1. Go to https://github.com/braekstudio/dora-releases/releases/new
2. **Tag**: `v` plus the version, for example `v4.17`. Phones compare this with their own version.
3. **Title**: `DORA 4.17`
4. **Description**: fill in the template below.
5. **Attach** `GPS TRACKER\apk\DORA.apk`. Do not rename it.
6. Leave "Set as a pre-release" unticked, keep "Set as the latest release" ticked, then Publish.

The download page needs no change. Its button always gives the newest release.

About a minute after publishing, GitHub hides all older releases by itself (turns them into drafts
that only you can see). Nothing is deleted. This is done by `.github/workflows/hide-old-releases.yml`.

This page is deliberately **not** listed on https://braekstudio.github.io/ (All apps). Don't add it there.

## Description template

```
What's new
- ...

For Android 8.0 or newer. Download the APK below and open it to install.
```

## Description for the first release (v4.17)

```
First release with automatic updates.

- Updates itself from now on (checked when DORA is opened, downloaded on Wi-Fi)
- Much smaller download: the offline map is now downloaded once inside the app
- Only the genuine DORA can connect to the family server

If you have an older DORA, uninstall it first, then install this one and rejoin your family by scanning their QR code.

For Android 8.0 or newer. Download the APK below and open it to install.
```
