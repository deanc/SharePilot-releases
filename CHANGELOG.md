# Changelog

All 1.x updates are included in a SharePilot 1 licence. From version 1.2.0,
SharePilot checks for updates automatically and offers installation in the app.
Automatic downloading and installation are optional in Update Settings. Older
versions need a manual download and replacement in Applications. Your settings
and trial/licence data are preserved. macOS may ask for Keychain approval again
after an update.

The public version history is maintained in the [SharePilot downloads repository](https://github.com/deanc/SharePilot-releases/blob/main/CHANGELOG.md).

## 1.2.0 (build 18) — 2026-10-26

### Added

- In-app updates through Sparkle, with automatic daily checks, release notes, and installation and relaunch. Use **Check for Updates…** from the app menu or the menu-bar panel's More options menu. **Update Settings…** includes optional automatic downloading and installation.
- Signed update feeds and downloads, restricted to the app's current major version. Future paid major upgrades cannot replace your licensed version automatically.

### Fixed

- Queued disconnects recheck the exact network mount before unmounting and refuse symlink redirection. Busy volumes remain protected by normal, non-forced macOS unmounts.
- Changing a connection keeps its previous saved password until replacement settings have been saved successfully.
- Closing the menu-bar panel and settings window releases their views, avoiding retained background observers.

Personal builds keep licensing disabled without reading or changing saved trial/licence records. In-app production updates are disabled in personal, sandbox and trial-preview builds.

Existing SharePilot 1 licences cover this update. No checkout or entitlement changes.

## 1.1.0 (build 17) — 2026-10-24

### Added

- A saved **Hide Dock icon** option beside **Open at login**. Changes apply immediately and are remembered after restarting. The Dock icon is hidden by default; SharePilot stays accessible from the menu bar.

Existing SharePilot 1 licences cover this update. No licensing or checkout changes.

## 1.0.1 (build 16) — 2026-10-23

### Fixed

- Settings exports now have owner-only file permissions and remove inherited read-access grants, protecting server addresses, usernames and rules from other local users.
- Automatic disconnects now require failed server checks spanning at least 30 seconds. Network changes and replacement mounts reset old outage history.
- Busy-file reports and pending health checks are discarded when they belong to a previous mount or network.
- An in-progress disconnect stays tracked if the app locks and unlocks, preventing duplicate disconnects and premature settings changes.
- Connection rules are checked again after the server responds, before starting a mount.
- Open in Finder now runs consistently when macOS reports a mount through the mount table before its completion callback.
- Endpoint checks now distinguish WebDAV paths containing escaped slashes and trailing slashes, and correctly compare default ports with uppercase URL schemes.
- Release-package validation remains enforced when Python optimisation is enabled.

Existing SharePilot 1 licences cover this update. No licensing or checkout changes.

## 1.0.0 (build 15) — 2026-10-22

Initial commercial release, published as version **1.0** with tag `v1.0-build15`.

- Automatic network-share mounting with connection rules, retries, menu-bar controls and busy-volume diagnostics.
- A seven-day full-feature trial and one-time SharePilot 1 licences through Paddle.
- Universal app for Apple Silicon and Intel Macs running macOS 26 or later.
