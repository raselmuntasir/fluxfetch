# FluxFetch

FluxFetch is a fast, privacy-focused desktop download manager written in Rust. It supports segmented downloads, pause/resume, queues, browser capture, video downloads, checksums, and a CLI.

## Highlights

- Multi-connection downloads with automatic fallback when a server does not support ranges
- Resume support, speed limits, scheduling, queues, and download categories
- Chrome, Edge, Brave, Vivaldi, Opera, and Firefox integration
- Video and audio downloads through verified, version-pinned helper binaries
- Windows startup support without opening one popup per queued download
- Local-first operation with no account, ads, analytics, or tracking

## Build

Install the stable Rust toolchain, then run:

```powershell
cargo build --release
```

The Windows executable is written to `target\release\fluxfetch.exe`.

## Test

```powershell
cargo test
```

Browser-extension tests require Node.js and can be run from `browser-extension` using the individual `*.test.js` files.

## Updates

Automatic update checks are disabled by default. Set `FLUXFETCH_UPDATE_API` to a trusted GitHub-compatible release JSON endpoint after creating your own release repository.

## Security

Helper downloads are pinned to explicit versions and verified with SHA-256 before use. Report security problems privately to the project owner rather than opening a public issue.

## Attribution

FluxFetch is a rebranded and modified fork of Download Craft. The original MIT license and copyright notice are preserved in `LICENSE` and `NOTICE.md`.

## License

MIT. See `LICENSE`.
