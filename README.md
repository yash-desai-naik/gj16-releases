# gj16-releases

Public download repo for **GJ16** installer binaries.

> **Alpha status:** the published builds (currently `v0.1.0`) are **alpha / testing builds**,
> not stable releases. They're here so testers can try the app and report issues. Expect bugs
> and rough edges — the app is still in early development.

## Download (Windows)

Grab the installer from the **latest release**:

- [`GJ16_0.1.0_x64-setup.exe`](https://github.com/yash-desai-naik/gj16-releases/releases/latest/download/GJ16_0.1.0_x64-setup.exe) — NSIS installer (recommended)
- [`GJ16_0.1.0_x64_en-US.msi`](https://github.com/yash-desai-naik/gj16-releases/releases/latest/download/GJ16_0.1.0_x64_en-US.msi) — MSI installer

macOS and Linux builds are not available yet.

## Why a separate repo

The source lives in the private [`gj16`](https://github.com/yash-desai-naik/gj16) repo. This
repo is public and holds only the built installer binaries, so the installers are reachable by
anyone (a private repo's release assets aren't publicly downloadable).

## Status

| Version | Channel        | Notes                                   |
| ------- | -------------- | --------------------------------------- |
| v0.1.0  | Alpha testing  | First published build — feedback wanted |

## Reproduce a release

Built from the `gj16` repo with `cd desktop && bun run tauri build`, then published here with
`gh release create`.
