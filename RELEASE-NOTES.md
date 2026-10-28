# FluxFetch 1.0.0

- Introduces the FluxFetch product identity, executable, storage path, and browser integration.
- Migrates existing `download_craft` and `idm_rust` configuration data automatically.
- Prevents startup from opening a popup for every queued download.
- Improves segmented-download buffering and throughput behavior.
- Verifies downloaded helper binaries with pinned SHA-256 hashes before execution.
- Disables unconfigured upstream update and mutable site-rule channels.
