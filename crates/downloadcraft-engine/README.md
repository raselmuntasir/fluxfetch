# downloadcraft-engine

The internal multi-connection HTTP engine used by FluxFetch. The crate name remains unchanged for source compatibility.

It provides range probing, dynamic segmentation, work stealing, crash-safe resume metadata, link refresh, throttling, checksum verification, and remote ZIP extraction.

```powershell
cargo test -p downloadcraft-engine
```
