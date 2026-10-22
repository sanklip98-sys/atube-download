# atube

Public download repository for atube. Application source code and technical documentation are maintained in a separate private repository.

## Download

[Download atube 1.4.16 for Windows](https://github.com/sanklip98-sys/atube-download/releases/download/v1.4.16/atube-Setup.exe)

[Latest release](https://github.com/sanklip98-sys/atube-download/releases/latest)

## Current Version

Version: 1.4.16

Installer: `atube-Setup.exe` (155322863 bytes)

Installer SHA-256:

`EB0BC47829401CE23E56D9364D8CFC928B057CB7D6C7FEA55068A06DAA3559D5`

## Release Notes

- The number of loaded videos after opening a YouTube Mix or playlist is now actually spoken by the screen reader. Earlier releases sent correct accessibility events, but the announcement label was placed outside the visible screen area, so NVDA stayed silent.
- The announcement label appears for a fraction of a second in the top-left corner of the window and disappears immediately, so it never covers the interface and never enters Tab navigation.
- The release also fixes the build and installation tools: the release script now has an equivalent Python version, the desktop shortcut is created natively without PowerShell, and the YouTube session module start-up test no longer hangs.
- The full documentation is now also available in Word format. After installation it is in the `Dokumentacja` folder next to the program: `ATube-dokumentacja.docx` (program description, publication rules and release notes), `ATube-README.docx` (user guide) and `ATube-AGENTS.docx` (instructions for AI models working on the code). The Word files are generated from the Markdown sources during the build, so they always match the installed version.
- The installer also creates a shortcut in the Start menu and can be run in a portable test mode that leaves the registry and the existing shortcuts untouched.
- Restores focus to the results list after closing Program settings opened from the application menu, including Cancel, Save, Escape and the window close button.
- Ctrl+U shares a video title and public link. WhatsApp and Telegram open their sharing flows; Messenger explicitly copies the message and opens the website so you can select a conversation and paste with Ctrl+V. Nothing is sent automatically.
- The main Download video command has one accessible dialog: choose MP3/MP4 with arrows, Tab to audio description, then Tab to Download and confirm with Space or Enter.
- Context menus offer separate Download MP3, Download MP4 and Download with audio description commands. Enter selects the mode directly without another format dialog. Existing save-location and AI-cost confirmations remain.
- Download from link — no playback accepts up to 100 YouTube links, one per line. Download all processes the validated list sequentially. Canceling or failing a file stops remaining items.
- Includes the live streams, comments, chat, account/playlist support and earlier improvements.

Audio descriptions for downloads remain MP4 plus SRT/TXT files, not synthesized narration in MP3. Link cards and playback behavior on recipients' devices depend on their messaging service and YouTube.

Regression tests, keyboard/modal-dialog checks, a clean installer run and a real MP4 download with audio/video passed. Actual messages to contacts, new paid AI-description calls and a manual NVDA/JAWS listening test were not performed. Node.js or Deno is required for yt-dlp. The installer is not Authenticode-signed.

## Publication Policy

This public repository contains only `README.md` and `latest.json`. Releases provide only the installer. Application source files, tests, build scripts, technical documentation, user settings and credentials are not published here. Required third-party runtimes, resources and licenses are included in the installer.

GitHub's automatically generated “Source code” archives contain only the public metadata files, not the application's source code. Executable binaries can still be analyzed or decompiled.