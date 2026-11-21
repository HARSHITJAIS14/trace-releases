# Trace for Mac

Official downloads of Trace by MindTrace for Apple silicon Macs.

[View available releases](https://github.com/HARSHITJAIS14/trace-releases/releases)

If the releases page is empty, the first public build is still in preparation. When a release is available, download `Trace-arm64.dmg`, open it, drag Trace to Applications, eject the disk image and open Trace from Applications.

## Website download button

Use the same address for every public version.

```text
https://github.com/HARSHITJAIS14/trace-releases/releases/latest/download/Trace-arm64.dmg
```

The matching SHA-256 checksum is available at the same address with `.sha256` added to the filename. These direct links become active with the first public release.

## Publishing an update

1. Prepare a versioned draft release and record the version and build number in its title or notes. Use a Developer ID signed, notarized disk image that has passed a clean-Mac install and launch test.
2. Name a copy of that final image `Trace-arm64.dmg`. In the same directory, run `shasum -a 256 Trace-arm64.dmg > Trace-arm64.dmg.sha256`. Attach both files to the draft.
3. Publish the stable release and mark it as **Latest**. Earlier versions remain available under their own tags.
4. Download both files using the permanent addresses as a signed-out visitor. In the download directory, run `shasum -a 256 -c Trace-arm64.dmg.sha256` and confirm it reports `OK`.
