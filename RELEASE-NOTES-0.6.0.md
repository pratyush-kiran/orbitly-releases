# Orbitly 0.6.0 for Windows

First public release of Orbitly, the file converter that lives at your cursor.

## Important: unsigned installer

This installer is **unsigned**. Windows may identify its publisher as unknown.
Download only from this release or the official product page, and verify the
SHA-256 listed alongside the installer. In-app installer execution is disabled
for this release; update checks lead to the download page for manual installation.

## Requirements

- Windows 10 22H2 (build 19045) or Windows 11, x64.
- Installs for the current user; the .NET runtime and compact LGPL FFmpeg are bundled.
- WebView2 is used for web-document-to-PDF conversion.
- Microsoft Office is used for Office-document conversion when installed.

## Included

- Cursor conversion wheel, Explorer integration, and keyboard shortcuts.
- Conversion Studio with batch review, per-file names/destinations, progress,
  cancellation/retry, searchable local history, and image comparison.
- Preset library, ordered workflow chains, customizable shortcuts, watch folders.
- Appearance presets, light/dark/system themes, and custom background images.
- Video/audio format, bitrate, frame-rate and metadata controls.
- Animated GIF resize/crop with frame preservation.
- One-time import of legacy preferences and installer cleanup of obsolete integration entries.

## Known limits

- The compact bundled FFmpeg does not include HDR tone mapping. That option is
  disabled unless a compatible external FFmpeg is configured.
- HEIC output needs the Windows HEVC extension; PNG/JPG alternatives are available.
- Static image outputs and the comparison window use one frame of animated images.
- Windows can block drag-and-drop from elevated programs; use Add files in Studio.
- Watch folders monitor their top level and skip files already present when enabled.

## Verification

The exact bundled FFmpeg passed all 111 existing engine checks. UI, startup,
workflow and interaction regression suites have also been exercised. The installer
has been compiled from the release source; clean-machine testing across every
supported Windows version is not a guarantee supplied by this release.

## Attribution and support

Original software copyright 2026 Atharv Gogia, licensed under MIT. Third-party
licence texts and FFmpeg build/source provenance are included in the installed
licenses folder. Application source remains in a private repository.

Report reproducible problems at https://github.com/pratyush-kiran/orbitly-releases/issues .
