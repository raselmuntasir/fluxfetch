# Portable Builds

Build FluxFetch with `cargo build --release`, then package `target/release/fluxfetch.exe` with the required assets and licenses.

Portable packages should not ship user settings, downloaded helper binaries, browser profiles, or signing secrets. Keep the original `LICENSE`, `NOTICE.md`, and third-party license files in every distribution.
