# 0.6.0-batch-dev14 — experimental local / Online Lobby test

- Map component budgets increase by 10% on all map sizes, rounded up per layer; underground maps retain equal complete pairs. G supports up to 70/70 sites when eligible locations suffice. A bounded spacing top-up helps plans that previously stopped below the nominal cap.
- All nine component quest targets receive a further 5% reduction from dev13, rounded up. Champion requirements and option 126 chance/spacing are unchanged.
- Native equipped, backpack and automatic grant paths reject custom artifacts for AI. Safe load/day/prebattle cleanup removes existing AI custom inventory. Human and ordinary artifact grants are preserved. Actual native enforcement needs local acceptance.
- Explicit local world counts and an artifact-guard readiness diagnostic support the first new-map test.
- 244 offline tests pass. No actual game, native save/load or two-computer Lobby test ran. Earlier AI-turn/fullscreen incidents remain unresolved; this is an experimental build requiring a NEW map.

# 0.6.0-batch-dev13 — experimental Online Lobby test

- Champion delivery now verifies the hero's actual town coordinates. A refused initial move remains retryable; an already prepared champion keeps later progress and must return to the delivery town.
- A completed map plan cannot shrink or gain new sites from late packets. Inconsistent completion counts are rejected, and map errors are written to the network diagnostic file immediately. Equal surface/underground counts remain 1:1.
- Very large battle kill totals saturate quest counters before integer overflow. Quest targets and rewards are unchanged.
- 233 offline tests pass, including the combined battle-result/quest path, replay cancellation, independent receivers, initial placement and inspected ACM attack dispatch. Native gameplay, actual save/load and two-computer Lobby acceptance remain pending. Earlier AI-turn/fullscreen incidents have no established fix.


# 0.6.0-batch-dev12 — experimental all-faction Online Lobby test

- Nine faction sets, champion quests/portraits/specialties and matching commanders.
- Correct map hints/pictures/shield silhouette; own-faction controlled rewards and no complete relics in native loot.
- Equal surface/underground component counts, bounded candidate space reserved for both levels and 15% lower set objectives.
- Painted in-book relic page, eight manual powers and additional Necropolis physical Life Leech.
- Verified champion delivery retry phases; real ACM mana capacity; backpack-preserving forge rollback.
- Immutable map packet identity and complete-plan validation; expanded persistence/replication fixtures.
- 213 offline tests pass. Native gameplay and two-computer Lobby acceptance remain pending; old AI-turn/fullscreen incidents have no established fix.

# 0.5.4-nettest-alpha — combined test update

Includes the 0.5.3 hover and quest display fixes, plus all currently agreed changes for the next test:

- Option 126: 5% component gate from level 18, with at least ten levels between selections per hero. Local saved cooldown; deterministic map-salted schedule online. Multiple-level gains respect the same spacing.
- Quest ownership labels count components held by all owned heroes, including parts represented by the assembled relic. Owning a part never blocks the separate once-per-player quest reward.
- Quest list/detail use one numeric state reader; requirement strings use the correct string assignment command.
- Map sites retain custom graphics and pickup names, with unsafe custom map hints removed.
- Network status exposes quest write errors separately.
- 50 offline tests pass. Runtime verification is pending for these changes; start a NEW map and keep both clients on the same version.
- The reported crash during fullscreen switching remains unresolved; no speculative graphics/native patch is included.

# 0.5.3-nettest-alpha

- Stop assigning trigger-local string references as persistent map-object hints. This targets the generic legacy hover error reported as File: erm, Line: 9614.
- Correct two VR:Z assignments on a local string in quest requirements (use VR:S).
- Read quest list/detail progress through one numeric helper; refresh town owner and hero after the selection dialog. Targets the reported Aegis 1275/10000 versus 0/10000 mismatch.
- Start a NEW map: existing native hint state in saves is not migrated.
- 44 offline checks pass; these fixes still need user-driven runtime verification. Two clients on one computer are not a substitute for a two-computer test.
- Option 126 balance is unchanged; the requested lower rate and ten-level limit remain pending.

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
