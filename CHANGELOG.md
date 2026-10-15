# 0.5.1-nettest-alpha

Published test candidate; the user will verify changes through Online Lobby. No native/runtime pass is claimed for this update.

- Apply idempotent operations locally before broadcast; add progress readback diagnostics.
- Browse quest progress without a hero; label counted objectives.
- Native-ID map proxies and guarded, idempotent component pickup; consume only after delivery.
- Fixed wire entry 26897 for pickup; existing six IDs unchanged.
- New random map required. Old 0.5.0 maps are not migrated.
- Hard quest targets, level 25/full ordinary Tower claim requirements and balance unchanged.

See NETWORK_TEST.md. VALIDATION.md describes earlier 0.5.0 local checks, not this update.
