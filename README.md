# atube

Public download repository for atube. Application source code and technical documentation are maintained in a separate private repository.

## Download

[Download atube 1.4.4 for Windows](https://github.com/sanklip98-sys/atube-download/releases/download/v1.4.4/atube-Setup.exe)

[Latest release](https://github.com/sanklip98-sys/atube-download/releases/latest)

## Current Version

Version: 1.4.4

Installer: `atube-Setup.exe` (146356079 bytes)

Installer SHA-256:

`6B0CCC5EBED968CD4381692C4DD3FD4113EAF0248409D77F8CEB60036C64118B`

## Release Notes

- Pasting a single YouTube video link with Ctrl+V, Shift+Insert or Paste starts that video immediately, even when ordinary-search Autoplay is disabled.
- The result list and playback queue contain only the requested video, without additional search results.
- The application announces “Playing: [title]” (Polish: “Odtwarzam: [tytuł]”) using the real video title instead of a video identifier. Opening/loading announcements are suppressed for direct links.
- Focus moves to the player: Space pauses/resumes, Left/Right adjusts volume, Ctrl+Left/Right seeks and Up/Down selects a result.
- Includes the Live filter, video comments, live chat, playlist/account support and previous fixes from 1.4.3.

Offline regression tests, real public title resolution and an MP4 download with audio/video passed. The new paste path has keyboard-preprocessing coverage; full system-clipboard E2E and a manual NVDA/JAWS listening test remain unverified. Actual signed-in comment/chat posting was not tested.

Node.js or Deno must still be installed for yt-dlp. Azure requires the user's own resource and may incur charges. The installer is not Authenticode-signed.

## Publication Policy

This public repository contains only `README.md` and `latest.json`. Releases provide only the installer; application source files, tests, build scripts, technical documentation, user settings and credentials are not uploaded here. The installer includes required third-party runtimes and resources.

GitHub's automatically generated “Source code” archives contain only these public metadata files, not the application's source code. Executable binaries can still be analyzed or decompiled.
