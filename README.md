# atube

Public download repository for atube.

The source code is kept in a private repository. This repository contains only public release metadata and links to installer downloads.

## Download

Use the latest GitHub Release:

https://github.com/sanklip98-sys/atube-download/releases/latest

## Current Version

Version: 1.4.0

Installer SHA256:

`D7608F6CE59313B6DCDBF938BA0711ED501BD5B04A8A0B9961F964139C71BB68`

## Release Notes

- Added an accessible download manager under `Ctrl + P` for queues of YouTube videos in MP4 or MP3 format.
- Downloads started from keyboard shortcuts now open the same system window with screen-reader progress, status, and cancellation controls. Synchronized SRT and TXT audio-description files remain supported.
- Added an MP4 fallback that downloads compatible H.264 video and M4A audio streams and merges them through the bundled VLC without requiring FFmpeg.
- Expanded seek steps from 10 seconds to 5 minutes and combined rapid seek commands to reduce repeated buffering.
- YouTube video listings now request titles in the current atube interface language, including Polish channel titles when provided by YouTube.
