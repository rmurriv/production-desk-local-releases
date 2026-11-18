# Production Desk Local releases

Mac-only offline production workspace. This repository hosts clean application release archives and the Ed25519-signed Sparkle update feed. It contains no saved workspaces or private starter snapshots.

Use **Production Desk Local → Check for Updates…**, then **Install Update**, then **Install and Relaunch**. Version 0.2.1 predates the updater and needs a one-time bootstrap installation.

**Verified November 17, 2026:** installed 0.3.0 (build 4) discovered the public 0.3.1 (build 5) release, downloaded it, prompted to install/relaunch, replaced the app and automatically restarted as 0.3.1. A subsequent check reported up to date. All pre-existing workspace/backup files and the preserved local starter snapshot retained identical SHA-256 hashes. This is an actual installed older-to-newer test on the development Mac.

Authentic archive/feed signatures passed. Tampered archives, tampered feeds and unsigned feeds were rejected by Sparkle's verifier tools. Projects/tasks also rendered with outbound network traffic blocked.

The published/tested app targets **Apple silicon, macOS 12 or newer**. It is locally ad hoc code signed, **not Apple Developer ID signed or notarized**. Ed25519 update authentication does not establish Gatekeeper approval on other Macs. Intel, interrupted-install recovery and other macOS versions have not been validated.

Normal workspace use requires no internet, account or cloud sync. Update checks are manual. No iPhone sync is included.

Local data stays in `~/Library/Application Support/ProductionDeskLocal`. Never delete this folder when replacing the app. Private original starters, when present, remain in a local `starter-snapshot.json` file and saved edits take precedence. Public downloads start with empty starter lists.
