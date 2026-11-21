# Trace for Mac

Trace by MindTrace for Apple silicon Macs.

[Download Trace for Mac](https://github.com/HARSHITJAIS14/trace-releases/releases/latest/download/Trace-arm64.dmg) · [Latest release notes](https://github.com/HARSHITJAIS14/trace-releases/releases/latest) · [SHA-256 checksum](https://github.com/HARSHITJAIS14/trace-releases/releases/latest/download/Trace-arm64.dmg.sha256)

**Build 73 launch notice.** This is a development-signed, unnotarized test build. macOS Gatekeeper rejected the copied app in testing. A Mac using default security settings may block the first launch. A fresh-Mac install and upgrade are still unverified for this version. [Build 73 test release notes](https://github.com/HARSHITJAIS14/trace-releases/releases/tag/v0.1.0-build73)

Open the disk image, drag Trace to Applications, eject the image and open Trace from Applications. When both local models are missing, first-run setup downloads about 1.20 GB.

## Website download button

Use the same address for every public version.

```text
https://github.com/HARSHITJAIS14/trace-releases/releases/latest/download/Trace-arm64.dmg
```

## Publishing an update

1. Prepare a versioned draft release. Record the version, build number, signing status and clean-Mac test result. For a normal public release, use a Developer ID signed, notarized disk image that has passed the clean-Mac install and launch test.
2. Name a copy of the final image `Trace-arm64.dmg`. Run `shasum -a 256 Trace-arm64.dmg > Trace-arm64.dmg.sha256` and attach both files to the draft.
3. Publish and mark the intended release as **Latest**. Earlier builds remain available under their own tags.
4. Download both files through the permanent links as a signed-out visitor. In the download directory, run `shasum -a 256 -c Trace-arm64.dmg.sha256` and confirm it reports `OK`.
