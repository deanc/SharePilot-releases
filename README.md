# SharePilot downloads

SharePilot is a native macOS menu-bar app that keeps your network shares connected
when your Mac wakes or changes networks.

**[Download SharePilot 1.1.0](https://github.com/deanc/SharePilot-releases/releases/tag/v1.1.0-build17)**

[Changelog](CHANGELOG.md) · [All releases](https://github.com/deanc/SharePilot-releases/releases)

Requires macOS 26 or later. Supports Apple Silicon and Intel Macs. SharePilot
connects to your own NAS or file server; it does not provide hosted storage.

## Trial and licences

SharePilot includes a seven-day full-feature trial from first launch. No account
or payment details are required. The original trial start is stored in Keychain
and preserved across updates and reinstalls.
After expiry, controls and background automation lock without a licence. Existing
volumes remain mounted and can still be managed in Finder.

[Buy a SharePilot 1 licence](https://sharepilot-licensing.dclat.workers.dev/buy)
for one Mac at a time, including all 1.x updates. The one-time base price is
US$24.99; your currency and applicable taxes are shown at checkout. A future 2.x
release requires a separate licence, bought outright or through a paid upgrade if
offered. You may keep using version 1 on compatible macOS versions.

Your licence key appears after checkout: save or download it, then paste it into
SharePilot's licence settings to activate this Mac. Paddle emails the payment
receipt separately. Deactivate before activating another Mac. Activation and
periodic checks require internet access, with up to seven days of verified offline
use. The purchased version 1 licence itself does not expire.

## Installation and updates

1. Download **SharePilot-macOS.zip** from the release above.
2. Extract the ZIP and read `READ-ME-FIRST.txt`.
3. Quit an existing copy, move `SharePilot.app` into Applications, then open it.

**The app is not Developer ID signed or notarised.** It has an ad hoc signature
for integrity only. macOS may block first launch. If you trust the source,
follow [Apple's installation guidance](https://support.apple.com/en-us/102445)
and use System Settings > Privacy & Security > Open Anyway where available.
Do not disable Gatekeeper globally to install SharePilot.

Updates are manual. Settings and trial/licence data are preserved. An ad hoc
update can prompt for Keychain access again. Use **Retry Keychain access** in the
app and respond to the macOS prompt yourself. Never enter your Mac password in the
licence-key field.

Download `SHA256SUMS` beside the ZIP and check it with:

```sh
shasum -a 256 SharePilot-macOS.zip
```

Compare the output with the ZIP's entry in `SHA256SUMS`. Checksums help detect
corruption; they do not replace Developer ID signing or notarisation.

## About this repository

This repository contains public download documentation and release assets.
The application source is maintained separately. GitHub's automatic source
archives contain this documentation, **not the app**.

Each release includes installation notes, checksums and `release.json`, recording
the app version, build, source commit, architectures, licensed major version and
signing state. Merchant and private licence-signing secrets are never included.

[Product information](https://deanclatworthy.com/software/sharepilot/) ·
[Refund policy](https://deanclatworthy.com/software/sharepilot/refunds/) ·
[Support](https://deanclatworthy.com/contact.html?subject=SharePilot%20support#my-form)
