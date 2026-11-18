# Production Desk Local releases

Mac-only offline production workspace. This repository hosts clean application release archives and the Ed25519-signed Sparkle update feed. No saved workspaces or private starter snapshots are included.

**Current release: 0.5.0 — sidebar and templates.** The top-left header button hides or restores the sidebar and remembers the choice after reopening. The Your sources stay yours sidebar section has been removed. Templates now offers **01 Video Project** and **03 Social clips**. Existing project workflows and checklists are preserved. Color-coordinated to-do brand tags remain available.

Use **Production Desk Local → Check for Updates…**, then **Install Update**, then **Install and Relaunch**. Version 0.2.1 predates the updater and needs a one-time bootstrap installation.

**Verified November 17, 2026:** actual hosted upgrades 0.3.0 → 0.3.1, 0.3.1 → 0.4.0, and 0.4.0 → 0.5.0 passed, including automatic restart. The latest upgrade preserved all 22 files present immediately before installation byte for byte. Sidebar persistence, the reduced template gallery and project creation were tested in a separate native fixture app, then the installed controls were checked.

Authentic archive/feed signatures passed. Tampered archives, tampered feeds and unsigned feeds were rejected by Sparkle verifier tools. Offline project/task loading was verified during the updater bootstrap validation.

Published/tested build: **Apple silicon, macOS 12 or newer**. Locally ad hoc code signed, **not Apple Developer ID signed or notarized**. Update authentication does not establish Gatekeeper approval on other Macs. Intel, interrupted-install recovery and other macOS versions have not been validated.

Normal workspace use requires no internet, account or cloud sync. Update checks are manual. No iPhone sync.

Local records remain in `~/Library/Application Support/ProductionDeskLocal`. Never delete this folder while replacing the app. Private preserved starters stay in a local `starter-snapshot.json`; saved edits take precedence. Public downloads have empty starter lists.
