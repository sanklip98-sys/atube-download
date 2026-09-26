# atube

Public download repository for atube. Application source code and technical documentation are maintained in a separate private repository.

## Download

[Download atube 1.4.2 for Windows](https://github.com/sanklip98-sys/atube-download/releases/download/v1.4.2/atube-Setup.exe)

[Latest release](https://github.com/sanklip98-sys/atube-download/releases/latest)

## Current Version

Version: 1.4.2

Installer: `atube-Setup.exe` (146338117 bytes)

Installer SHA-256:

`62EBB5FBE303CF9CDBA23BD6A30EB858EB22231009D3C396B15C1681F74F3F3A`

## Release Notes

- Pasting a concrete YouTube video link shows only that video and creates a one-video playback queue. Playlist/radio parameters do not add unrelated videos. Date sorting keeps the single result, and Play Next stops at its end.
- Unchanged playlist/mix links do not reload when returning to and leaving the search field. Normal text searches and pure playlists still support multiple results.
- Autoplay follows the existing preference. If disabled, press Enter to play the selected video.
- Includes the JavaScript-runtime discovery fix: Node.js and Deno are found in standard installation folders even when absent from the application's PATH.
- Includes Azure OpenAI for audio description and related content, with endpoint/deployment validation, a Windows-protected API key, and an accessible connection test.

Version 1.4.1 remained an unpublished draft. Version 1.4.2 includes its prepared changes as well as the direct-link fixes.

Node.js or Deno must still be installed. Azure requires the user's own resource and image-capable deployment and may incur charges. The installer is not Authenticode-signed.

## Publication Policy

This public repository contains only `README.md` and `latest.json`. Releases provide only the installer; application source code, tests, build scripts, and technical documentation are not uploaded here.

GitHub's automatically generated “Source code” archives contain only these public metadata files, not the application's source code.
