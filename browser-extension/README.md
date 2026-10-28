# FluxFetch Browser Extension

This Manifest V3 extension captures browser downloads and sends links, media, cookies, and required request headers to the local FluxFetch native-messaging host. If the desktop app is unavailable, supported downloads can fall back to the browser.

## Local Installation

1. Open FluxFetch and install the native host from **Settings → Browser integration**.
2. Open the browser extension-management page and enable developer mode.
3. Load this directory as an unpacked extension.
4. Restart the browser after changing the native-host registration.

## Identity

The Chromium manifest keeps a compatibility signing key so the desktop host and unpacked extension continue to share a stable ID. Generate your own key before public release and update `EXTENSION_ID` in `src/app.rs`.

Firefox currently uses the placeholder `fluxfetch@example.invalid`; replace it in both `manifest-firefox.json` and the desktop host allowlist before AMO publication.

## Tests

Run the JavaScript `*.test.js` files with Node.js. No browser account is required for local unpacked testing.
