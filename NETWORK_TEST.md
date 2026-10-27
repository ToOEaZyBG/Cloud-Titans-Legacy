# Legacy of the Cloud Titans â€” Online Lobby test

Version **0.6.0-batch-dev25**. This is an experimental all-faction release for a new two-player test. Automated checks pass; native gameplay, save/load and two-computer synchronization still need player verification.

## Install the same build

Both players close the game, then use the existing **Legacy of the Cloud Titans - TEST** entry in Heroes Launcher â†’ Mod Browser. Keep the folder **Cloud Titans Legacy - Local Test**; enable only one copy of this mod. The installed `mod.json` must say **0.6.0-batch-dev25** on both computers. Catalog metadata can lag behind downloaded files; an older version displayed in the browser does not establish which build was installed. Check the installed version before starting.

Use identical ERA/HD versions, enabled mods, load order and WoG options. The inspected base profile used ERA platform 2.299, HD 5.8 R22, Advanced Classes Mod 1.11, JS new objects 1.40, JS main module 1.21.2, JS commanders 1.02, JS map fixes 1.12 and JS terrains 1.4.1. Match the exact versions available to both players; TEST_PROFILE.json is an observed reference, not certification of every combination. Keep Knightmare Kingdoms and other metadata-listed incompatible packages disabled. Keep both ERAHDHeroes_3_Reborn (Full) and HD Editionfixai (Lite) disabled for this trial, following the selected remaster-free profile. Use their original Mod Browser files; this release does not patch them.

Start a **NEW G random map with underground through Heroes Launcher Online Lobby**, using sequential turns with simultaneous turns disabled. Do not resume an older-version map and do not use F12. For the first comparison, both players can choose Necropolis. WoG option 126 is optional; enable it on both clients if testing level-up rewards. Commanders must be enabled for champion quests. No extra starting army or automatic test gift is granted.

## Dev25 first checks

Click Sort in HD Backpack; it should close and rebuild with name-sorted items. The click fix is covered offline but awaits actual native acceptance. On a NEW G map with underground, component plans retain equal layer totals and include some opposite-layer faction parts. Necropolis/Inferno/Dungeon must no longer be entirely absent from the surface. Old maps are not changed.

Enable option126. Verify missing own-faction parts at18,23,28,33 and every5 levels; check batch levels, other owned heroes and save/reload. Complete collections give ordinary Relics.

## Local acceptance first

Start a NEW local map with the installed build. On the first adventure turn, inspect `Debug/CloudTitansWorld.ini`: `version` must match the installed build, `error` zero and surface/underground equal when both levels exist. Read declared counts, not old trailing item rows. `Debug/CloudTitansAccess.ini`, section `native`, must show `artifact_guard=1`; stop and preserve Debug if protection is unavailable. Then hover and collect one component and check its name, picture and slot.

Dev25 doubles the spacing-limited top-up target for all factions and sizes, within the retained nominal and density caps. Complete-pair caps for widths 36/72/108/144/180/216/252 are 20/40/60/80/100/120/140 total sites. Surface-only caps are 20/40/60/80/99/119/139. Valid-site shortages can reduce counts. A bounded top-up adds sites to spacing-limited plans while retaining at least four tiles of separation; it cannot guarantee a part on every explored route. Option126 now guarantees missing parts at18+5k.

Observe AI encounters and captured loot: no custom part or relic should remain with an AI. Human inventories, including other human players, must remain intact. Report the first violation with the matching save. The automated fixtures do not establish actual native interception or loot behavior.

## Dev20 / Dev21 / Dev22 local checks

Accept each quest family with a known hero. Switch town heroes and leave town: status must retain the recorded hero; fulfilled component objectives remain green. A substitute cannot claim or add victories. Lose the bound hero, then accept with a replacement: unfinished counters reset, the original faction remains locked, and claimed rewards stay claimed. Save/reload at each phase.

Open HD Backpack and click Sort at its top-right. Put down any artifact held on the cursor first. The popup closes and reopens after sorting so its cells reflect the current order. The inspected HD5.8R22 WoG provider is supported; Ctrl+N in the hero screen, then Sort backpack by name, remains the fallback if the button is unavailable. The town Inventory tools entry is removed. Check duplicates, distinct scroll spells, equipment and counts before/after, repeated sort and actual save/reload. Review all eight colored component names in an artifact tooltip; green=equipped, gray=not equipped. The set heading shows the current equipped count (N/8); an assembled relic counts as all eight. Backpack items do not count.

If the stack-experience rank table is blank, inspect the Stack Experience Rebalance configuration. Its own Runtime INI overrides its shipped JSON defaults. Enable Rebalance, WoG Stats, WoG Abilities and WoG Neutrals through that provider's configuration. The recommended Medium preset is +100% Health and Damage, +10 Attack/Defense and +10% Speed at rank10. TUM options require that provider and are separate. Restart/load after confirming. Each peer configures this separately; a Cloud Titans update does not overwrite another mod's options.

Dev23 writes a read-only check after game entry to Debug/CloudTitansStackExperience.ini. With the selected provider/settings active, the Vampire Lord sample should have six enabled stat rows and one ability row (seven total). Disabled settings and empty live rows are reported separately. This does not itself prove native table rendering or real combat application.

## First shared test

1. Each player reaches their first adventure turn. Open `Debug/CloudTitansNetwork.ini` in the game folder and compare `version`, `placed`, `hash`, `surface`, `underground` and `world_error` on both computers. Errors must be zero. Counts must agree; surface and underground must be equal, up to 70/70 on G with adequate valid sites. A shortage reduces both equally. These read-only checks require no development gifts or quest-menu debug rows.
2. Hover and collect one map component. Hover, pickup picture/name and inventory must identify the same item and its equipment slot. A foreign faction part found on the map is allowed. After turn transfer, confirm that the object is absent on the other computer; the receiving player checks their inventory. A second visit must give nothing.
3. Finish one ordinary battle and record the winner's faction quest progress before/after. Then save together, exit normally, reload through the same Lobby workflow and check that player's progress/inventory again. Actual save/load and reconnect are acceptance tests, not established support claims.

Stop on the first wrong item, script error, mismatch or crash. Preserve both saves and relevant Debug folders locally. Record the exact action, turn, version, player and screenshots; do not repeatedly visit a failed object. Do not update either client during a running game.

## Sets and quests

All nine towns have eight components and an assembled relic. Worn distinct parts unlock cumulative bonuses; backpack items and duplicate copies do not multiply them. The relic represents all eight components. Its equipment slot is stated in its description. Assemble/disassemble through the mod's existing hero/town actions; disassembled parts go to the backpack. Keep space for the resulting items. Failed grants preserve the reward for retry.

Level-up and faction quest components follow the hero's faction. Custom artifacts are excluded from native random loot, so Dragon Utopia cannot award a complete custom relic. Human map finds can belong to another faction. AI heroes are excluded from our artifacts: native equipped/backpack/automatic grant paths are guarded, and load/day/prebattle cleanup removes existing custom AI inventory. This new native policy still requires player-run acceptance; it is not an established fix for earlier AI-turn crashes. Set quest targets receive another10% reduction from dev24, rounded up: **328 / 2617 / 6542 / 65408 / 1309 / 656 / 99 / 6542**, with objective names and progress in the quest menus. Option126 guarantees a missing own-faction component at18,23,28,33 and every5 levels thereafter, checking all owned heroes. A complete collection gives an ordinary Relic instead.

Link an equipped relic to a matching owned developed town to test its weekly apex recruitment bonus. Compare hero and creature values before/after equipping/removing pieces, daily mana (including Intelligence capacity), duplicate items, full backpacks and town ownership changes. Linked growth, movement and native callbacks require in-game acceptance.

## Dev21 stat balance

All positive artifact primary and equipment/set stat bonuses increase by 50%, rounded up per individual bonus. Examples: +4 becomes +6, +2 becomes +3, +1 Speed becomes +2, and 300 movement becomes 450. All faction troops gain +3 Attack/Defense and +2 Speed at the corresponding thresholds. Apex troops gain another +5 Attack/Defense and +2 Speed from the ring. Health is +15%, or +23% for Necropolis; Tower retains its lightning threshold instead. Full daily regeneration is 16 spell points within the existing mana cap. Spell costs, battle power mechanics, weekly recruits, 30% Life Leech and champion specialties are unchanged.

Compare unequipped, partial-set and assembled values on the same hero and troops. Check the green names and (N/8) counter after moving components, changing heroes and saving/reloading.

## Relic powers

On your own stack's turn after Tactics, open the battle spellbook and select **Relics** at the bottom. The separate page shows the painted set icon, power name and mana cost. Wear the assembled relic; eight separate components do not enable its manual power. Each relic has one manual activation per battle. Cancel spends nothing; invalid targets or insufficient mana must reject the action. Compare both computers immediately after a successful activation, then after the next round/turn. Ordinary spell navigation must still work.

| Town | Power | Mana |
| --- | --- | --- |
| Castle | Seraphic Restoration, shared resurrection Health budget | 40 |
| Rampart | Forest's Embrace, Air Shield and top-creature healing | 30 |
| Inferno | Infernal Gate, temporary Horned Demons | 40 |
| Necropolis | Life Harvest, living-enemy damage and shared undead restoration | 30 |
| Dungeon | Abyssal Rift, targeted Implosion | 25 |
| Stronghold | Warlord's Fury, Haste and Attack-based physical damage | 20 |
| Fortress | Primordial Venom, two-round Poison window without refresh | 25 |
| Conflux | Elemental Invocation, one of four elemental choices | 30 |

Tower lightning is automatic, with its existing Giant/Titan/Lord of Thunder rules. The assembled Necropolis relic additionally gives controlled units 30% Life Leech from physical attacks against living enemies, including shots and retaliation, bounded by starting stack size. This passive has no mana cost and is separate from Life Harvest. Native combat ordering, immunities and synchronization must be tested.

## Champions

Choose **Champion quest**, then explicitly Accept with the hero here. Status always reads that bound hero, wherever they are. Only their faction wins count. Component quests have their own hero binding. The first acceptance locks one faction for the rest of the game across both quest families. Hero loss resets unfinished progress and permits a replacement of that same faction; previously claimed components and a delivered champion are never issued again. Enrollment can precede qualification. To count the five qualifying wins, bring a level-25 hero with four distinct matching components (kept; the assembled relic also qualifies), all required ordinary town buildings and enabled commanders. Grail and optional coastal buildings are excluded; each town uses its own available Mage Guild maximum. Use only the faction's regular troops in those wins; commanders/machines do not interfere.

Leave town and Alt-left-click the bound hero for the final trial, or press Ctrl+J on the adventure map. Stronghold requires no hero spells in its trial; Conflux requires four distinct elemental steps. Return the bound hero to the matching town garrison, leaving a free visitor space, and keep fewer than eight heroes. A full roster, occupied visitor or unavailable matching unused native slot keeps the reward waiting. Delivery is complete only after the actual hero, town position, army and visitor checks pass. If an already prepared pending champion has moved away, bring that champion back to the delivery town before retrying; later progression is preserved.

| Town | Champion |
| --- | --- |
| Castle | Aldric |
| Rampart | Sylvara |
| Tower | Vaelion |
| Inferno | Zareth |
| Necropolis | Andonov |
| Dungeon | Nyssara |
| Stronghold | Kargan |
| Fortress | Ssareth |
| Conflux | Aurelis |

The champion starts at level 1, zero XP and base **25/25/25/25**, with a fresh matching commander. Specialization works without the set; Andonov has stronger faction bonuses. Repeated delivery and loading must preserve later progression and commander state. Check real heroes, portraits, armies and commanders on both clients, not only counters.

## Known limits

The earlier AI-turn and fullscreen crashes have no established fix in this release. Matching hashes and offline fixtures do not prove compatibility with every mod or real Lobby transport. The online experiment uses sequential turns. Quick Combat, replay, trials, native spellbook presentation, complete champion lifecycle, weekly changes and multiplayer save/load remain separate acceptance steps.
