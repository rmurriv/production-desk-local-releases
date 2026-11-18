# Production Desk Local releases

Mac-only offline production workspace. This repository hosts clean application release archives and the Ed25519-signed Sparkle update feed. It contains no saved workspaces or private starter snapshots.

**Current release: 0.4.0 — to-do brand colors.** Assign a brand when creating a task, through quick-add, or in the task table's BRAND column. Labeled tags and task icons match the five sidebar brand colors. Existing tasks stay unassigned until a brand is chosen. Dashboard layout and brand navigation are unchanged.

Use **Production Desk Local → Check for Updates…**, then **Install Update**, then **Install and Relaunch**. Version 0.2.1 predates the updater and needs a one-time bootstrap installation.

**Verified November 17, 2026:** actual hosted upgrades from 0.3.0 → 0.3.1 and 0.3.1 → 0.4.0 both passed, including automatic restart. The 0.4.0 update preserved all 22 data files present immediately before installation byte for byte. Native brand creation, inline editing, and persistence after reopen were verified with disposable test tasks.

Authentic archive/feed signatures passed. Tampered archives, tampered feeds and unsigned feeds were rejected by Sparkle's verifier tools. Projects/tasks also rendered with outbound network traffic blocked during the updater bootstrap validation.

The published/tested app targets **Apple silicon, macOS 12 or newer**. It is locally ad hoc code signed, **not Apple Developer ID signed or notarized**. Ed25519 update authentication does not establish Gatekeeper approval on other Macs. Intel, interrupted-install recovery and other macOS versions have not been validated.

Normal workspace use requires no internet, account or cloud sync. Update checks are manual. No iPhone sync is included.

Local data stays in `~/Library/Application Support/ProductionDeskLocal`. Never delete this folder when replacing the app. Private original starters, when present, remain in a local `starter-snapshot.json` file and saved edits take precedence. Public downloads start with empty starter lists.
