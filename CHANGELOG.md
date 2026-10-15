# 0.5.2-nettest-alpha

- Enable the eight human Relic component rewards for WoG option 126 in network games, from level 18 onward.
- Use deterministic hero/reward-level selection online, without an extra RNG call, separate grant packet or extra item.
- Preserve native grants/dialogs and distinct reward-level inputs when several levels are gained together.
- Keep AI, lower reward classes and gameplay balance unchanged.
- 34 automated checks pass; ERA and Online Lobby verification remain pending. Both players must close the game and update together. Start a new map for the test.

# 0.5.1-nettest-alpha

Published test candidate; the user will verify changes through Online Lobby. No native/runtime pass is claimed for this update.

- Apply idempotent operations locally before broadcast; add progress readback diagnostics.
- Browse quest progress without a hero; label counted objectives.
- Native-ID map proxies and guarded, idempotent component pickup; consume only after delivery.
- Fixed wire entry 26897 for pickup; existing six IDs unchanged.
- New random map required. Old 0.5.0 maps are not migrated.
- Hard quest targets, level 25/full ordinary Tower claim requirements and balance unchanged.

See NETWORK_TEST.md. VALIDATION.md describes earlier 0.5.0 local checks, not this update.
