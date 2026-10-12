# Email MCP for macOS

This repository hosts installers and authenticated update metadata for Email MCP by InfinitIQ Tech. Implementation source and private signing material are not published here.

## Release status

The first production release is being prepared. No production installer is available yet.

## Platform

- Apple Silicon Mac (arm64)
- macOS 26.0 or later

Production installers will be signed with InfinitIQ Tech's Developer ID and notarized by Apple. In-app updates will verify a signed Sparkle feed and a separately signed archive before installation.

Release assets are limited to the versioned DMG, `appcast.xml`, and `SHA256SUMS.txt`. GitHub's automatically generated repository ZIP and tar archives contain only this release repository's metadata; they are not application installers.

The app keeps account configuration and credentials local to the user's Mac. Updates are intended to preserve those settings and require an explicit check from the application's **Check for Updates** menu.

## Authenticity

- Application bundle: `tech.infinitiq.mail-mcp.accounts`
- Apple signing team: `34P4RF23ET`
- Sparkle Ed25519 public key: `ga3v/VVnjPwmUUGbpUK4buI2hKXJWhcJSy/lLchnjLE=`
- Stable feed: `https://github.com/InfinitIQ-Tech/email-mcp-releases/releases/latest/download/appcast.xml` (available after the first production release)

Never disable Gatekeeper or remove quarantine to install this application. A development installer is not a production release.
