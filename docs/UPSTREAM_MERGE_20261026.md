# Upstream migration, 2026-10-26

Merged iLoader v2.4.0 and isideload upstream main into separate migration branches.
The existing fix/watch-login-20261014 branches remain the rollback baseline.

Preserved: embedded Watch bundle ID rewriting, watchOS device registration,
separate watchOS profiles and signing, direct companion installation, HealthKit,
selective anisette reset, approved Windows anisette server and saved selection.
Added upstream automatic anisette reprovisioning and extension-profile reuse.
Watch apps always override profile reuse to keep platform-specific profiles.

Validation: Windows selective-reset and Watch-profile-policy unit tests, frontend
production build and full Windows release build. Physical login, iPhone update,
and Watch companion installation still require device verification.
