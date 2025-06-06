# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- Introduced a new `play()` method using `ffplay` for direct media playback.

## [1.0.2] - 2025-06-06

### Added

- Enabled fine-tuning of encoding behavior through `self.crf`, `self.movflags`, and `self.max_muxing_queue_size`.

### Fixed

- Missing `-y` flag when `replace=True` to allow overwriting output files while normal splitting.

### Changed

- Allowed custom thumbnail extraction by letting thumb accept a timestamp string ("HH:MM:SS") instead of only True or False.

## [1.0.1] - 2025-06-04

### Added

- Fetch media info (duration, size, streams) via FFprobe.
- Encode with custom codecs, presets, and metadata via FFmpeg.
- Split files or split into parts (with/without re-encoding).
- Generate thumbnails from videos.
- Custom command execution for ffmpeg, ffprobe, ffplay.
- Track naming and title setting.
- Progress callback support for long operations (encoding, splitting, etc).
- Pure `subprocess` (no dependencies except Python & FFmpeg).

[unreleased]: https://github.com/BhagyaJyoti22006/ffwrapy/compare/v1.0.2...HEAD
[1.0.2]: https://github.com/BhagyaJyoti22006/ffwrapy/compare/v1.0.1...v1.0.2
[1.0.1]: https://github.com/BhagyaJyoti22006/ffwrapy/releases/tag/v1.0.1