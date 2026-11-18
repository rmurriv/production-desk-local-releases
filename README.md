# Production Desk Local releases

Mac-only offline production workspace. This repository hosts clean application release archives and the Ed25519-signed Sparkle update feed. It contains no saved workspaces or private starter snapshots.

Updates use **Production Desk Local → Check for Updates…**, followed by the download and install/restart prompts. Version 0.2.1 predates the updater and needs a one-time bootstrap installation.

The current build targets Apple silicon and macOS 12 or newer. It is locally ad hoc code signed, **not Apple Developer ID signed or notarized**. Ed25519 signing authenticates updates separately from Apple Gatekeeper. Normal workspace use requires no internet, account, or cloud sync.

Local data stays in `~/Library/Application Support/ProductionDeskLocal`. Never delete this folder when replacing the app.

Update integration validation is in progress; this repository does not yet claim a passing older-to-newer test.
