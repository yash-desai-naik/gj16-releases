# gj16-releases

Public download repo for **GJ16** installer binaries.

> **Alpha status:** the published builds are **alpha / testing builds**, not stable releases.
> They're here so testers can try the app and report issues. Expect bugs and rough edges — the
> app is still in early development.

## Download (Windows)

Grab the installer from the **latest release**:

- [`GJ16_0.2.8_x64-setup.exe`](https://github.com/yash-desai-naik/gj16-releases/releases/latest/download/GJ16_0.2.8_x64-setup.exe) — NSIS installer (recommended)
- [`GJ16_0.2.8_x64_en-US.msi`](https://github.com/yash-desai-naik/gj16-releases/releases/latest/download/GJ16_0.2.8_x64_en-US.msi) — MSI installer

macOS and Linux builds are not available yet.

## Why a separate repo

The source lives in the private [`gj16`](https://github.com/yash-desai-naik/gj16) repo. This
repo is public and holds only the built installer binaries, so the installers are reachable by
anyone (a private repo's release assets aren't publicly downloadable).

## Status

| Version | Channel        | Notes                                                                 |
| ------- | -------------- | --------------------------------------------------------------------- |
| v0.2.8  | Alpha testing  | New GJ16 wordmark branding (app + shortcut icons)                      |
| v0.2.7  | Alpha testing  | Duplicate scan is async with live progress (no more UI freeze)         |
| v0.2.6  | Alpha testing  | Guard against false "completed" while files remain pending             |
| v0.2.5  | Alpha testing  | Fix resume/retry progress resetting to 0                               |
| v0.2.4  | Alpha testing  | adb embedded in app, set up at launch — installer can't fail on adb   |
| v0.2.3  | Alpha testing  | Run adb from a runtime dir so it never locks the installer's files     |
| v0.2.2  | Alpha testing  | Fix installer "file in use" on adb DLLs (GJ16 stops the adb server)    |
| v0.2.1  | Alpha testing  | Fix console window flashes on launch (adb CREATE_NO_WINDOW)           |
| v0.2.0  | Alpha testing  | Self-contained installer (bundles adb, WebView2, SQLite), UI pass      |
| v0.1.0  | Alpha testing  | First published build — feedback wanted                                |

## Reproduce a release

Built from the `gj16` repo with `cd desktop && bun run tauri build`, then published here with
`gh release create`.
