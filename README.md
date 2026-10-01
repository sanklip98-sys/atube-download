# atube

Public download repository for atube. Application source code and technical documentation are maintained in a separate private repository.

## Download

[Download atube 1.4.6 for Windows](https://github.com/sanklip98-sys/atube-download/releases/download/v1.4.6/atube-Setup.exe)

[Latest release](https://github.com/sanklip98-sys/atube-download/releases/latest)

## Current Version

Version: 1.4.6

Installer: `atube-Setup.exe` (146374574 bytes)

Installer SHA-256:

`76E2030CF07AC288460DEB74B007B76841DE24A19BD96F6899D3FC87903AC6FD`

## Release Notes

- Ctrl+U shares a video title and public link. WhatsApp and Telegram open their sharing flows; Messenger explicitly copies the message and opens the website so you can select a conversation and paste with Ctrl+V. Nothing is sent automatically.
- The main Download video command has one accessible dialog: choose MP3/MP4 with arrows, Tab to audio description, then Tab to Download and confirm with Space or Enter.
- Context menus offer separate Download MP3, Download MP4 and Download with audio description commands. Enter selects the mode directly without another format dialog. Existing save-location and AI-cost confirmations remain.
- Download from link — no playback accepts up to 100 YouTube links, one per line. Download all processes the validated list sequentially. Canceling or failing a file stops remaining items.
- Download commands inside the link editor affect only the captured caret row, never the whole list. Blank/invalid rows and multirow text selections disable these actions. Right-clicking within selected text preserves Cut/Copy.
- Ordinary pasting into the main search field still plays the requested single video and announces its title.
- Includes the live streams, comments, chat, account/playlist support and earlier improvements.

Audio descriptions for downloads remain MP4 plus SRT/TXT files, not synthesized narration in MP3. Link cards and playback behavior on recipients' devices depend on their messaging service and YouTube.

Regression tests, keyboard/modal-dialog checks and a real MP4 download with audio/video passed. Actual messages to contacts, new paid AI-description calls and a manual NVDA/JAWS listening test were not performed. Node.js or Deno is required for yt-dlp. The installer is not Authenticode-signed.

## Publication Policy

This public repository contains only `README.md` and `latest.json`. Releases provide only the installer. Application source files, tests, build scripts, technical documentation, user settings and credentials are not published here. Required third-party runtimes, resources and licenses are included in the installer.

GitHub's automatically generated “Source code” archives contain only the public metadata files, not the application's source code. Executable binaries can still be analyzed or decompiled.
