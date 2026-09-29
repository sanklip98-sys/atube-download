# atube

Public download repository for atube. Application source code and technical documentation are maintained in a separate private repository.

## Download

[Download atube 1.4.3 for Windows](https://github.com/sanklip98-sys/atube-download/releases/download/v1.4.3/atube-Setup.exe)

[Latest release](https://github.com/sanklip98-sys/atube-download/releases/latest)

## Current Version

Version: 1.4.3

Installer: `atube-Setup.exe` (146353133 bytes)

Installer SHA-256:

`CF081AC1D323E373EC99496629DCCE2600E496B27ECB2C7B7CF84D4A331D8522`

## Release Notes

- New Live result filter searches active YouTube broadcasts. Select a stream and press Enter to watch.
- Ctrl+Shift+J opens video comments; Ctrl+Shift+K opens live chat. Both are also available in the application menu.
- Discussions reuse the connected YouTube account from the playlist manager. Check the displayed channel before publishing; playback cookie imports alone do not enable posting.
- Send explicitly publishes a comment or chat message. Enter in the message editor adds a line. Drafts remain after errors, duplicate sends are blocked, and uncertain writes are not automatically retried.
- Chat refresh preserves keyboard focus and unchanged reading position. Moderation events remove deleted content in server order.
- Includes the direct-video-link, JavaScript-runtime discovery and Azure OpenAI improvements from 1.4.2.

Offline regression tests and public read-only comment/chat checks passed. Actual signed-in posting and a new manual NVDA/JAWS listening test were not performed. YouTube account/channel restrictions and moderation still apply.

Node.js or Deno must still be installed for yt-dlp. Azure requires the user's own resource and may incur charges. The installer is not Authenticode-signed.

## Publication Policy

This public repository contains only `README.md` and `latest.json`. Releases provide only the installer; application source code, tests, build scripts, technical documentation, user settings and credentials are not uploaded here.

GitHub's automatically generated “Source code” archives contain only these public metadata files, not the application's source code. Executable binaries can still be analyzed or decompiled.
