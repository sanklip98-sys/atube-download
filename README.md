# atube

Public download repository for atube.

The source code is kept in a private repository. This repository contains only public release metadata and links to installer downloads.

## Download

Use the latest GitHub Release:

https://github.com/sanklip98-sys/atube-download/releases/latest

## Current Version

Version: 1.3.93

Installer SHA256:

`048902F7AC34B480676C2D62EA22C59247A7F10C9BA861D63DAF89DEC7E43553`

## Release Notes

- Added an optional screen-reader-friendly window title that places the current video title before the atube name.
- Kept the window title stable between playback changes to avoid repeated, unsolicited NVDA announcements.
- Improved autoplay responsiveness by preparing the embedded VLC player asynchronously and resolving the first stream in parallel.
- Improved playback reliability by forwarding the HTTP headers required by YouTube streams and retrying failed videos with an alternate YouTube player client.
