# Privacy Policy — Music Handoff

_Last updated: 2026-05-22_

Music Handoff is a Chrome extension that lets you move music playback between
[music.youtube.com](https://music.youtube.com) and the YouTube Music app on your phone.
This document describes what the extension does with your data.

## Summary

Music Handoff **does not collect, transmit, or sell any personal information**.
It does not use analytics, trackers, or any third-party servers operated by the developer.

## What the extension stores

The extension stores the following data **only on your own device**, using the browser's
local `chrome.storage` API:

- The screen ID and Lounge tokens issued by Google when you pair your phone.
  This is what lets your phone recognize the browser as a known device on subsequent sessions.
- A configurable device name (the label shown on your phone's cast picker).
- The most recent tab volume, so your preference persists across page reloads.

This data is **not** sent to the developer or to any third party. It stays on your machine
and is removed when you uninstall the extension or clear the extension's storage.

## What the extension communicates with

Music Handoff talks directly to two Google-operated endpoints:

- `music.youtube.com` — the tab where playback runs.
- `www.youtube.com/api/lounge/*` — Google's Lounge protocol endpoints, the same ones
  the YouTube Music phone app uses to talk to Cast devices and TVs.

Both are first-party Google services. The extension does **not** route any data through
servers operated by the developer or any other third party.

## What is not collected

- No analytics, telemetry, or crash reporting.
- No tracking pixels, cookies, or fingerprinting.
- No personal data, email address, IP address, or browsing history.
- No data is sold or shared with anyone.

## Permissions, in plain language

- `storage` — to remember your paired phone and preferences across sessions.
- `alarms` — to keep the Lounge session alive in the background.
- Access to `music.youtube.com` — to read playback state and send commands to the tab.
- Access to `youtube.com/api/lounge/*` — to talk to Google's casting endpoints.

## Contact

Questions, concerns, or data requests can be filed as an issue at
[github.com/EH127/music-handoff-feedback](https://github.com/EH127/music-handoff-feedback/issues).

## Changes

Material changes to this policy will be reflected in this file's git history and the
"Last updated" date above.
