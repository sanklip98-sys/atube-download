# atube

Public download repository for atube.

The source code is kept in a private repository. This repository contains only public release metadata and links to installer downloads.

## Download

Use the latest GitHub Release:

https://github.com/sanklip98-sys/atube-download/releases/latest

## Current Version

Version: 1.4.0

Installer SHA256:

`D44741BA90033AD96ADB7F8505117335A9966EF72E9C0622F1E2B15659C084F4`

## Release Notes

- Added an accessible download manager under `Ctrl + P` for queues of YouTube videos in MP4 or MP3 format.
- Downloads started from keyboard shortcuts now open the same system window with screen-reader progress, status, and cancellation controls. Synchronized SRT and TXT audio-description files remain supported.
- Added an MP4 fallback that downloads compatible H.264 video and M4A audio streams and merges them through the bundled VLC without requiring FFmpeg.
- Expanded seek steps from 10 seconds to 5 minutes. The first seek now reacts immediately, while rapid follow-up commands are combined into one final VLC jump to reduce repeated buffering.
- YouTube video listings now request titles in the current atube interface language, including Polish channel titles when provided by YouTube.
- Added a `Shorts` result filter that shows only YouTube Shorts while preserving playback, downloads, subtitles, and audio description.
- Simplified screen-reader output for the result filter: it now announces the current option without the redundant list of all available filters. Full filter descriptions are available under `F1`.
- The same Short found through `/watch` and `/shorts` URLs is merged by its YouTube video ID instead of being shown twice.
