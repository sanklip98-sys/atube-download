# atube

Public download repository for atube. Application source code and technical documentation are maintained in a separate private repository.

## Download

[Download atube 1.4.1 for Windows](https://github.com/sanklip98-sys/atube-download/releases/download/v1.4.1/atube-Setup.exe)

[Latest release](https://github.com/sanklip98-sys/atube-download/releases/latest)

## Current Version

Version: 1.4.1

Installer: `atube-Setup.exe` (146337640 bytes)

Installer SHA-256:

`D7DB8156751EFA8A2E013ECDB7C87CD3176C3D40580EEDB2BDB4C088D86F6637`

## Release Notes

- Fixed the “Missing JavaScript runtime” error when downloading video or audio with Node.js or Deno installed but missing from the application's PATH. Standard installation folders are now checked as well.
- Added Azure OpenAI for audio description and related content, including endpoint/deployment validation, a Windows-protected API key, and an accessible connection test.
- Preserved screen-reader support, MP4/MP3 downloads, and synchronized SRT/TXT audio-description files.

Node.js or Deno must still be installed. Azure requires the user's own resource and image-capable deployment and may incur charges. The installer is not Authenticode-signed.

## Publication Policy

This public repository contains only `README.md` and `latest.json`. Releases provide only the installer; application source code, tests, build scripts, and technical documentation are not uploaded here.

GitHub's automatically generated “Source code” archives contain only these public metadata files, not the application's source code.
