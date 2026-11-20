# DJ Lab — beta release files

This repository holds **only distribution files** for the DJ Lab private beta on macOS:

- `macos/<arch>/appcast.xml` and `appcast.xml.sig` — the update feed DJ Lab checks (served by GitHub Pages at
  `https://gitnoureldin.github.io/djlab-releases/`). The feed and every update package are signed with an Ed25519 key that is
  kept offline; the app only trusts packages that match the public key built into it.
- Update packages (`DJLab-<version>-build<N>-<arch>.zip`) attached to the GitHub Releases of this repository.
- `notes/` — short release notes.

No source code, no personal data, no music and no rekordbox libraries are stored here. First-time installers are shared
privately with invited testers; this repository is the update channel.

DJ Lab is an unsigned engineering beta (no Apple Developer ID yet): macOS asks for a one-time *Open Anyway* approval.

## Licenses
DJ Lab includes code from [rekordbox-mcp](https://github.com/davehenke/rekordbox-mcp) (MIT License, see
`LICENSE-rekordbox-mcp.txt`). The third-party components bundled in the app and their licenses are listed in
`THIRD_PARTY_NOTICES.txt` (also inside every app at `DJ Lab.app/Contents/Resources/`). Sparkle (MIT) provides the updates.
