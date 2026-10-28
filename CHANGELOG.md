# 28/10/2026 dev35 > dev36 - 0.6.0-batch-dev36

- Remove the mod's Ctrl+N shortcut, separate commander menus and commander purchases with resources. Keep the normal HD Backpack Sort button. Equip commander items through the normal Commander icon.
- Right-click a part when all six different matching parts are equipped on the Commander to confirm assembly. After the Commander window closes, replace them with one equipped relic in the clicked slot. Right-click an equipped relic to confirm dismantling: preserve original items and their battle growth; place parts in free commander slots and send remaining parts to the backpack. A full backpack refuses atomically when required; declining changes nothing.
- Add a5%chance of one random commander part after every confirmed human victory. Include all18parts and exclude complete relics. Preserve the two-copy map plan,180finds, original external monsters and guaranteed hero parts at18,25,32,39and every7levels thereafter. Existing normal battle loot remains unchanged. AI gets no custom reward.
- Use the existing confirmed battle result/commit flow for normal and Quick Combat; simulations, failed/replayed results and duplicate packets create no extra attempts. Rewards enter the backpack and show the normal artifact picture. A full backpack consumes the attempt without rerolling or altering existing items. No gold, wood, ore, hero-level or commander-level purchase requirement.
- Restart fully and create a NEW map on matching36 clients. Targeted native-code/ERM/resource/release checks pass; actual native UI, battle, save/load and two-computer acceptance remain pending. No game control or installed/settings/save changes.

# 28/10/2026 dev34 > dev35 - 0.6.0-batch-dev35

- Equip the18 new commander parts and three assembled relics through the normal Commander icon. They appear in the actual six Commander-screen slots, alongside original artifacts. Click an equipped icon to return it to the backpack; right-click for green N/6 set progress. Ctrl+N is only an optional forge/assembly menu, no longer an equipment requirement. New commander items cannot be worn on the hero.
- Count actual commander equipment in any physical slot. Preserve partial2/4/6 bonuses; assembling six matching parts from native slots and/or the backpack consumes only those parts. A relic occupies one real slot, leaving five free; preserve original artifact abilities and battle-growth records. Guard custom rendering before the original ten-item lookup. Require matching35, a full restart and a NEW map; old saved scripts are not migrated.
- Add native-format translucent ground shadows to all90 individual map artifacts. Retain their painted subject pixels, adaptive colors, one-cell footprints and separate frame-cache names. Keep exactly two copies per item,180finds, external map monsters and level18+7k rewards unchanged.
- Targeted native-code, authored ERM, resource and release checks only; no full-suite repeat. Actual native UI, battle, save/load and two-computer acceptance remain pending. No game control or installed/settings/save changes.

# 28/10/2026 dev33 > dev34 - 0.6.0-batch-dev34

- Reduce NEW-map generation to exactly2copies of every individual faction component and commander item:90types*2=180finds, with90on each layer when underground exists. Do not generate complete assembled relics. Existing maps keep their original objects; level rewards at18,25,32,39and every7levels thereafter are unchanged.
- Align placement, completion, pickup and network bounds with180sites; require matching34on both peers and a NEW map. Preserve all set bonuses, assembly, artwork, champions, AI grant rules, Sort, feedback forms and optional English/Russian Revolut support.
- Require the original external adventure-map monster proximity check for every new or reused site. Additional items no longer use unguarded open land. Preserve existing monster armies and ordinary guarding/movement behavior; add no embedded armies, custom Yes/No dialog or scripted battle. A plan without enough suitable guarded locations fails explicitly instead of filling unguarded sites.
- 15 targeted generation/replication/pickup and catalog/release checks pass; no full-suite rerun or native game/save/Lobby acceptance. No game control or installed/settings/save changes.

# 28/10/2026 dev32 > dev33 - 0.6.0-batch-dev33

- Add optional Revolut support at https://revolut.me/antonezwt and English/Russian invitations for feedback, bug reports and support for improvements and future mods.
- Add the repository funding link and preserve all existing feedback forms. Donations are optional; playing, sharing and reporting issues are welcome too.
- Presentation-only release: all398 Data/EraPlugins/Lang files are byte-identical to dev32. Runtime diagnostics remain32; public metadata is33. Existing dev32 maps are unaffected by this documentation update. Earlier native acceptance limits remain unchanged.
- Six targeted catalog/release tests pass; the full gameplay test suite is not repeated. No game control, installation, settings or save changes.

# 28/10/2026 dev31 > dev32 - 0.6.0-batch-dev32

- Combine the six matching commander parts into a single Ember Oath Relic, Iron Covenant Relic or Astral Conclave Relic. Consume one of each from commander equipment or the backpack, with no extra fee. The relic enters the backpack; equip it in the commander Pendant position to retain the full50-point bonus to all eight ACM modifiers and90total to its favored pair. Five native commander positions remain available with their original effects.
- Show green set headings with N/6 progress and a six-part checklist. Active parts and earned2/4/6 thresholds turn green; an active assembled relic represents6/6. Two active matching parts still give15points to all eight modifiers. Hero equipment and backpacks do not count as active gear. Refresh descriptions for the inspected commander and after equipment changes.
- Dismantle a backpack relic into six parts after unequipping it. Validate all component identities, capacity, cursor, owner, full-record backpack hash, saved gear and sequence before committing; failures preserve all items, gear and resources, and replay does not duplicate rewards. Direct forging of complete relics is refused.
- New relics549..551 are excluded from map templates and native random pools, receive no AI grants or activation, and have no effect as hero equipment. Give each assembled relic its own original painted icon. Map generation stays90individual part types*3=270finds; no full relics. Level18+7k rewards, hero sets, champions, portraits, Sort and feedback forms remain included.
- 776 offline tests pass; native rendering, commander battle integration, native save/load and two-computer acceptance remain pending. No game/UI control or installed/settings/save changes. Both players close and update through the existing Mod Browser entry, matchdev32 and start a NEW map.

# 28/10/2026 dev30 > dev31 - 0.6.0-batch-dev31

- NEW random maps now target exactly3 copies of each of72 faction components and18 commander items:270 finds,135 per layer when underground exists. Complete relics are never placed. Existing eligible sites are reused and additional safe open land sites are added without deleting other objects; an incomplete plan is reported as an error.
- Level-up rewards remain unchanged: faction components at18,25,32,39 and every7levels thereafter. This three-copy policy concerns map generation only.


- Add18 original painted commander artifacts in three six-piece universal sets: Ember Oath (Attack/Damage), Iron Covenant (Defense/Health), Astral Conclave (Spell/Passive). Every town and commander class may use each set.
- In the hero screen press Ctrl+N, select Commander equipment and forge. This separate six-slot page owns the new equipment. Carrying an item in hero equipment or backpack gives no bonus. Native commander items reserve matching positions; new IDs are never forced into the native commander artifact table and existing items are unchanged.
- Each active piece adds5 percentage points to all eight ACM commander attribute modifiers. At2/4/6 matching parts, add another5/5/10 points to all. A full set adds40 to its two favored modifiers:50 points to all eight,90 to its favored pair; identical480-point budget. Bonuses augment ACM outputs without replacing commander classes, learned abilities, passive mechanics or existing modifiers. Actual balance awaits player feedback.
- Forge each part for50,000Gold,20Wood and20Ore with a level20 hero and enabled living human commander. Forged items enter the backpack and require explicit commander equipping. Capacity/currency/owner/slot/hash/sequence validation prevents failed changes from losing items or money, and prevents duplicate packet rewards.
- Extend native AI grant rejection and inventory cleanup through artifact548. AI, dead/disabled commanders and native-occupied custom positions receive no custom bonus. Removing retained gear is allowed even while a commander is dead or its native slot is occupied.
- Preserve prior hero-set stats, quests, level-up acquisition, champions, portraits, first-click Backpack Sort and feedback forms. No installed files, settings or saves were changed and no game was controlled. Offline checks do not establish native UI/save/load or two-computer compatibility; those acceptance steps remain pending. Match dev31 and start a NEW map after both players close and update.

- Background validation: 751 offline tests pass, including4096 commander gear combinations, exact270-site generation, three-copy counts, sender/receiver native mutation-order equality, replay and commander pickups. No new native game acceptance is claimed.

# 28/10/2026 dev29 > dev30 - 0.6.0-batch-dev30

- Fix the reported delayed Sort button: clicking Sort in the supported HD5.8R22 Backpack closes the current modal immediately, sorts after destruction of cached cells and reopens the updated backpack without waiting for another click.
- Use H3API H3Msg::CloseDialog instead of an ignored synthetic Escape key-down. Keep the provider's cancellation result and ordinary item behavior; held artifacts still prevent sorting. Complete artifact records, sequence/hash checks and network sorting transactions are unchanged.
- Background verification includes the production x86 popup lifecycle fixture, a regression that fails against the old handler, and isolated execution of the shipped native close/default-message helpers. Actual in-game rendering/click response and two-computer synchronization remain pending; no game was launched or controlled. The full suite was not repeated; the previous 716-test record belongs to dev28 development.
- The dev29 feedback invitation and bug/suggestion forms remain included. Close the game before updating through the existing Mod Browser entry; match dev30 on both clients. Older embedded save scripts are not migrated.

# 28/10/2026 dev28 > dev29 - 0.6.0-batch-dev29

- Add a visible feedback invitation to the Mod Browser description and project README, with separate guided forms for bugs and suggestions.
- Bug reports request installed mod/ERA/HD versions, enabled mods, reproduction steps and expected/actual results. Screenshots are optional; saves, raw logs, crash dumps and personal information should remain private.
- Documentation and release metadata only. All Data, EraPlugins and Lang files are byte-for-byte identical to dev28. No new gameplay fix or native acceptance is claimed. The existing dev28 record of 716 passing offline tests is retained; the full suite was not repeated for this update.

# 28/10/2026 dev27 > dev28 - 0.6.0-batch-dev28

- Require200 each of Wood, Ore, Mercury, Sulfur, Crystal and Gems and200,000Gold for champion receipt. Resources are retained.
- Fix the unused native champion selector: pass the requested player's mask as the input to the documented hero-availability check, and accept normal unused starting XP below100 and level-one commanders. Recheck those starting-state limits during authorized one-time initialization. Keep owned, placed/prison, tavern, already initialized and existing equipment-ledger heroes protected.
- Retain the bound garrison hero/free lower visitor slot requirements, live qualification checks, native readback and retry safeguards. No scripted trial battles return.
- Change guaranteed missing own-faction component rewards with option126 from every5 to every7levels, starting at18:18,25,32,39,46,53,60,67,74,81,88,95,102. Retain collection checks, ordinary Relics for complete sets and the native grant path.
- Deliver the champion after closing the town screen. Use the documented ERA specialty hints and paired portrait command. Package all18 indexed portraits inside the native resource archive; remove loose H3-format PCX files that the external-file decoder loaded as empty images.
- 716 offline tests passed during dev28 development; the resource-only correction was checked with package/resource gates and targeted tests without repeating the full suite. Native spot acceptance on a protected local save passed actual Andonov receipt through the town menu, both portraits, level1/25/25/25/25, town exit/reentry and actual save/reload. All18 native portrait resources load with correct dimensions and nonempty pixels. Other individual champion lifecycles and real two-computer Lobby synchronization remain pending.
- Close the game before updating through the existing Mod Browser entry. Match dev28 on both clients and start a NEW map; old embedded save scripts are not automatically migrated.

# 27/10/2026 dev26 > dev27 - 0.6.0-batch-dev27

- Remove scripted champion trials for all nine towns, including Andonov's 150 Archangels and Conflux's four elemental steps. Replace them with three held reserves: 50,000 Gold; 50 Wood and 50 Ore; 25 each of Mercury, Sulfur, Crystal and Gems. These are checked at receipt and are not spent.
- Retain the bound hero, level25, four distinct matching components (or assembled relic), fully developed owned town, enabled commanders and five ordinary faction-only victories. Recheck qualification when claiming. Parts are kept.
- Choose Champion quest > Receive champion with the bound hero in the upper garrison slot and an empty lower visitor slot. The new champion goes into that lower slot. Missing conditions, an absent hero, occupied slot, full roster or unavailable unused matching hero leave the reward available. Native readback and retry safeguards preserve initialized hero/commander progression.
- Show current reserve amounts in status. Ctrl+J and Alt-click open the checklist. Retired trial requests and delayed trial packets cannot invoke a battle; load clears stale active associations without rewards.
- 706 offline tests pass, covering reserve boundaries and town delivery for all nine factions, resource retention, lost qualification, blocked/retried grants and obsolete requests. Offline fixtures do not execute real ERA dialogs or Lobby transport. The reported scripted-trial route is removed; a general post-battle crash repair is not claimed. Native delivery/save-load and two-computer acceptance remain pending.
- Close the game before updating through the existing Mod Browser entry. Both clients need matching dev27 and a NEW sequential-turn map; do not use F12 or migrate old saves for acceptance.

# 27/10/2026 dev25 > dev26 - 0.6.0-batch-dev26

- All nine sets: the full active bonus line is green when its worn-piece threshold is reached. Carried items and duplicates do not unlock thresholds. Descriptions refresh when the inspected hero changes.
- Replace the exact Mage/Arch Mage/Enchanter quest target family with Lich/Power Lich, including Tower. Replace Unicorn/War Unicorn/Hell Steed with Black Knight/Dread Knight, and Green/Gold/Diamond Dragon with Bone/Ghost/Blood Dragon/Dracolich, wherever those quest families occur. Other families and numerical requirements remain unchanged. These replacements reflect the encountered armies; availability still depends on the generated map.
- Preserve the existing guaranteed missing own-faction rewards at18,23,28,33 and every5 levels thereafter. Read-only diagnostics from the reported save confirm five native rewards at18,23,28,33,38.
- Repair the trial position guard using the native visibility and object-below fields. The engine retains the last town type after leaving onto an empty tile, which previously caused an incorrect leave-town refusal. Hidden garrison heroes and actual town visitors remain excluded.
- 686 offline tests pass. Native champion post-battle crash investigation remains open; no crash fix or two-computer synchronization pass is claimed.
- Close the game before updating via the existing Mod Browser entry. Start a NEW map; existing saves keep embedded scripts and quest targets.

# 27/10/2026 dev24 > dev25 - 0.6.0-batch-dev25

- Apply acquisition changes to all nine castles. Reduce each component quest target another10%, rounded up:328/2617/6542/65408/1309/656/99/6542. Champion requirements remain unchanged.
- Replace the5% gate and ten-level cooldown with a guaranteed own-faction component at18,23,28,33,38,43 and every5 levels thereafter, with WoG option126 enabled. Each reward in a multiple-level gain uses its individual level. The hero class determines its faction.
- Choose a component currently missing from the player's collection across all owned heroes' equipment and backpacks. An assembled relic represents all eight parts. If the collection is complete, award an ordinary native Relic instead. Found and level-up parts do not consume quest claims. Native reward code still grants one item per level; the selector never adds a second grant.
- Double the spacing-limited map top-up target, within the existing map-size cap,55% loose-artifact density limit and maximum140 sites. Retain guarded eligible locations, minimum four-tile separation and complete equal surface/underground pairs. Counts depend on generated eligible locations; old maps are not repopulated.
- 639 offline tests pass. A NEW local G map reached the first turn and placed140 components,70 per layer,error0. Native artifact guard reports1. The all-faction selector and real level18/23 delivery are covered by offline fixtures; their native acceptance and save/load remain pending. No two-computer synchronization pass is claimed.
- Close the game before updating through the existing Mod Browser entry. Start a NEW map; old save scripts and missed past rewards are not migrated.

# 26/10/2026 dev23 > dev24 - 0.6.0-batch-dev24

- Fix the HD Backpack Sort caption button: native LBUTTON_CLICK is13, whereas12 is LBUTTON_DOWN. Preserve normal clicks, held-item rejection and deferred sorting after popup destruction. Apply the same completed-click handling to the Relics page caption button; relic icon selection retains its native icon event.
- Correct the opposite-layer component rotation. A chained self-referential assignment overwrote its own input, excluding Inferno, Necropolis and Dungeon components from the surface. The repaired rotation retains the existing75/25 faction preference and equal total layer counts, while allowing all nine factions on both layers. Existing maps are not rearranged; start a NEW map.
- Keep the5% component gate from level18 and at least ten levels between component selections. Guarantee a component on the tenth eligible attempt after nine failed gates. Cooldown levels do not advance the counter. Local counters persist per hero; duplicate-level calls cannot charge twice. Network mode deterministically reconstructs the same bounded schedule without extra RNG or grant packets.
- Extend the reward diagnostic to record failed eligible checks as well as selected components. Guarantee concerns component selections; inventory delivery and option126 remain separate requirements. Prior save history is not reconstructed or retroactively rewarded.
- Retain dev23 level-one champions with25/25/25/25, the observed provider configuration and all prior set changes.
- 639 offline tests pass, including a completed-click regression that failed against dev23, per-subcommand arithmetic semantics, all-faction layer coverage and local/network guarantee fixtures. Native UI/gameplay/save/Lobby acceptance remains pending.
- Close the game before updating through the existing Mod Browser entry. Both peers must match the complete build and start a NEW sequential-turn map.

# 25/10/2026 dev22 > dev23 - 0.6.0-batch-dev23

- All nine newly delivered champions start at level1, zero XP and base25/25/25/25. The existing one-time initialization and retry/readback guards preserve later hero progression and matching commander state; existing delivered heroes are not reset. Champion quest conditions and faction specialties are unchanged.
- Add a read-only stack-experience diagnostic after provider game entry. Debug/CloudTitansStackExperience.ini records provider/options plus actual enabled Vampire Lord stat and ability rows, allowing disabled settings to be distinguished from absent live data. No rank tables or other mod settings are changed by this diagnostic.
- Document the provider-owned WoG configuration and recommended Medium preset. The author's local saved options had Rebalance and all WoG packages disabled; those four switches were restored locally, retaining selectors and inactive TUM options. This local configuration change is separate from the public package and must be matched by peers through their own provider settings.
- Include the Sort button inside the supported HD5.8R22 WoG Backpack from dev22. Put down held artifacts before sorting; full artifact records are preserved and the popup rebuilds after sorting.
- 627 offline tests pass. Native rank-table/button rendering, combat callbacks, actual save/load and two-computer acceptance remain pending.
- Close the game before updating through the existing Mod Browser entry; check installed version0.6.0-batch-dev23. Start a NEW map for the combined test.

# 25/10/2026 dev21 > dev22 - 0.6.0-batch-dev22

- Add a Sort button directly to the top-right of the HD Backpack popup. Click it to sort carried artifacts by name; the popup closes and reopens with refreshed cells.
- Dispatch only after the provider destroys the old popup. Preserve every complete artifact record, including scroll spell identities; equipment and artifact counts remain unchanged. Continue using the existing verified permutation transaction for online play.
- Do not sort while an artifact is held on the cursor. Preserve ordinary backpack clicks and cancellation. Control allocation failure, an ID collision or an unavailable integration leaves the provider behavior intact.
- Pin this integration to the inspected HD5.8R22 WoG provider; other providers retain the Ctrl+N hero-screen fallback. No third-party file is modified. All dev21 stat and tooltip changes remain included.
- 606 offline tests pass, including executed x86 button/modal fixtures and read-only provider contract checks. Actual HD rendering, hook dispatch and two-computer acceptance remain pending.
- Close the game before updating through the existing Mod Browser entry. The installed mod.json must show0.6.0-batch-dev22.

# 25/10/2026 dev20 > dev21 - 0.6.0-batch-dev21

- Increase positive primary and equipment/set stat bonuses by 50%, rounding up each individual bonus, across all 72 components and nine assembled relics. A +4 primary becomes +6, +2 becomes +3, +1 Speed becomes +2, and 300 daily movement becomes 450.
- Faction troop bonuses become +3 Attack/Defense, +2 Speed and +15% Health; Necropolis Health becomes +23%. Apex troops receive another +5 Attack/Defense and +2 Speed from the ring. Full daily set regeneration is 16 spell points, capped by the existing mana rules.
- Present equipped component names in green and other components in gray. Show the equipped count in the set heading as (N/8), with the assembled relic representing all eight parts. Include the individual artifact name and refresh descriptions for the inspected hero.
- Keep spell costs, special battle powers, weekly recruitment, 30% Life Leech, champion specialties and acquisition requirements unchanged. Tower retains its automatic lightning mechanics.
- 597 offline tests pass. These include all equipment masks, native configuration fields and per-hero tooltip state fixtures; actual native rendering, callback order, save/load and two-computer acceptance remain pending.
- Fully close the game before updating through the existing Mod Browser entry. Start a NEW map with matching versions on both computers.

# 25/10/2026 dev18 > dev20 - 0.6.0-batch-dev20

- Explicit hero enrollment for both component and champion quests; only the bound hero earns progress. First acceptance permanently locks one faction per player. Hero loss resets unfinished progress and permits a same-faction replacement; previously claimed components and delivered champions remain once-only.
- Include hero/generation identity in progress/trial packets and exact identity in reset packets, rejecting late old-hero traffic. Keep completion green outside town; require the recorded hero present for claims and champion delivery.
- Reduce every component target by another10%, rounded up:364/2907/7268/72675/1454/728/110/7268. Compact objective rows while retaining all upgrade eligibility in full details.
- Add colored lists of all eight set parts to artifact descriptions. Provide Sort backpack by name through Ctrl+N in the hero screen; omit the extra town Inventory tools entry, preserving complete artifact records and sending the chosen permutation online.
- Use the official adventure mouse event/modifier data for Alt-click trials; add Ctrl+J for the recorded quest hero.
- The installed private QA helper is removed during the closed-game update; no QA helper is shipped. A sort button inside HD Backpack is still pending and is not claimed in this release.
- 539 offline tests pass. Native acceptance is pending while this candidate is reviewed; no actual save/load or two-computer pass is claimed here.
- Fully close the game before updating. Start a NEW map and match the complete build/profile with the other player.

# 20/10/2026 dev17 > dev18 - 0.6.0-batch-dev18

- Separate the internal map-frame names from inventory frames for all64 added faction components. Read-only inspection of the failed dev17 game found46 map templates using the exact44x44 inventory payload instead of their32x32 adventure frame. All5 observed Tower templates used their correct map frame and already had distinct names.
- Change only those internal frame names in map resources; retain artwork, palettes, geometry, masks, Tower resources, inventory, native plugin, slots, budgets, equal surface/underground counts and quests.
- Reject case-insensitive global DEF frame-name conflicts across every bundled archive and loose resource before release. Identical packed/loose copies remain permitted.
- 257 offline tests pass. Native spot checks on a new G map covered16 identified map items across all nine sets and all eight Inferno component types. All48 different loaded custom map frames matched their correct32x32 map payloads, before and after one actual save/reload. The map had62 sites,31 per layer.
- Close the game fully before updating, then use a NEW map. Individual pickup/equipment checks for all72 parts, full quest/power lifecycles and two-computer Lobby acceptance remain pending.

# 20/10/2026 dev16 > dev17 — 0.6.0-batch-dev17

- Compile all72 map components into a32x32 sprite with matching one-cell MSK/MSG bounds, eliminating the unused blank left tile. The artwork fits within a one-pixel gutter and retains its independent palette.
- Applies to every town and component. Inventory artwork, identities, slots, map budgets,1:1 layers and quests are unchanged.
- Show the current public build and six dated changelog entries before the mod description; preserve the complete additive GitHub history.
- 253 offline tests pass. This is a candidate correction for reported half-visible map artifacts; actual terrain rendering still requires player acceptance. No native gameplay or Lobby pass is claimed.

# 0.6.0-batch-dev16 - clearer adventure-map components

- Increase component map artwork to a maximum30 pixels with a clear tile gutter.
- Compile every component with its own map palette, preserving faction colors independently from the inventory palette. Tower and the eight additional towns use the same map compiler.
- Inventory icons, artifact identities/slots, object masks, placement budgets, equal layers and gameplay rules are unchanged.
- 249 offline tests pass, including decoded native sprite geometry, color fidelity and Tower archive/mask preservation. Native map appearance still needs player acceptance.

# 0.6.0-batch-dev15 - startup call hotfix

- Fix the AI artifact-guard readiness call: an explicit STDCALL convention is required even for a function with no arguments.
- The access fixture now rejects the original malformed call and uses the real framework convention constants.
- All dev14 balance and AI-policy changes remain included. 245 offline tests pass; native startup, AI behavior, save/load and Lobby acceptance still require player verification.

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


## Preserved project beginnings and local development milestones

This appendix fills gaps in the original public changelog without deleting its
existing release entries. Dates below are recorded milestone dates in
Europe/Berlin. Local/private milestones are explicitly distinguished from
public releases. The earliest preserved source baseline is0.2.13 on15/10/2026;
work before that baseline is not completely documented, so no missing dates,
versions or successful tests are invented here.

### 15/10/2026 — earliest preserved Tower baseline0.2.13

- One Tower faction collection, equipment/set effects and local test roadmap.
- Guarded random-map acquisition without starting gifts; startup checkpoints
  and original Tower map drawings followed on the same date.
- Local human component rewards were classified as Relic from level18.
- Tower component quests, hero/town development requirements and assembly.

### 15/10/2026 — first public distribution0.4.2

- Published the original Tower local test through the existing Mod Browser
  repository. Installation checks remained distinct from multiplayer acceptance.

### 15/10/2026 — public network test0.5.0

- Added explicit network receiver transactions and a controlled Lobby guide.
- Later0.5.1–0.5.4 changes retain their original detailed entries above.

### 16/10/2026 — all-faction development begins

- Eight additional standard-town sets and painted artifact masters were
  prepared and reviewed. Existing Tower content remained the reference.
- Signature abilities and nine champions were designed. A reported network
  AI-evaluation crash was recorded; no universal fix was established.

### 17/10/2026 — local combined prototype and dev2–dev5

- Integrated nine faction champions, native portraits and commanders.
- Initial combined startup failed and the prior local version was restored.
- Subsequent local repairs addressed artifact configuration bounds, ERA input,
  artifact prose/tooltips and quest display. Dev5 was installed for local tests.
- These local candidates were not separate public Mod Browser releases.

### 17/10/2026 dev5 > dev6 — local candidate

- Added the relic battle-book entry and additional Necropolis life drain.

### 17/10/2026 dev6 > dev7 — local candidate

- Corrected native ERA command framing and expanded book/champion checks.

### 18/10/2026 dev7 > dev8 — local candidate

- Added an isolated relic icon page and readable low-mana entries.

### 18/10/2026 dev8 > dev9 — local candidate

- Revised faction loot exclusions, champion quest flow, relic page and
  component acquisition balance following player screenshots.

### 18/10/2026 dev9 > dev10 — local candidate

- Repaired component map identity, Inferno shield silhouette, pickup pictures
  and collection capacity.

### 18/10/2026 dev10 > dev11 — private audit candidate

- Audited equipment transactions and book lifecycle; equalized map layers1:1.
- Used actual maximum mana and preserved backpack inventory on rollback.

### 18/10/2026 dev11 > dev12 — public test resumes

- Added verified delivery recovery and reviewed release gates. Detailed public
  dev12 and later changes remain in the main changelog above.

All dates and local/public labels derive from preserved Git milestones and
release records. They are not additional gameplay or multiplayer acceptance.

### Publication date index for subsequent public dev builds

- 18/10/2026 dev11 > dev12
- 19/10/2026 dev12 > dev13
- 20/10/2026 dev13 > dev14
- 20/10/2026 dev14 > dev15
- 20/10/2026 dev15 > dev16

Dates are preserved release commit timestamps in Europe/Berlin. Later releases
add their dated transition at the top without deleting this history.
