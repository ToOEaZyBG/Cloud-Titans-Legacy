# Legacy of the Cloud Titans — Online Lobby test

Version **0.6.0-batch-dev16**. This is an experimental all-faction release for a new two-player test. Automated checks pass; native gameplay, save/load and two-computer synchronization still need player verification.

## Install the same build

Both players close the game, then use the existing **Legacy of the Cloud Titans - TEST** entry in Heroes Launcher → Mod Browser. Keep the folder **Cloud Titans Legacy - Local Test**; enable only one copy of this mod. The installed `mod.json` must say **0.6.0-batch-dev16** on both computers. Catalog metadata can lag behind downloaded files; an older version displayed in the browser does not establish which build was installed. Check the installed version before starting.

Use identical ERA/HD versions, enabled mods, load order and WoG options. The inspected base profile used ERA platform 2.298, HD 5.8 R22, Advanced Classes Mod 1.11, JS new objects 1.40, JS main module 1.21, JS commanders 1.02, JS map fixes 1.12 and JS terrains 1.4. Match the exact versions available to both players; TEST_PROFILE.json is an observed reference, not certification of every combination. Keep Knightmare Kingdoms and other metadata-listed incompatible packages disabled. Keep both ERAHDHeroes_3_Reborn (Full) and HD Editionfixai (Lite) disabled for this trial, following the selected remaster-free profile. Use their original Mod Browser files; this release does not patch them.

Start a **NEW G random map with underground through Heroes Launcher Online Lobby**, using sequential turns with simultaneous turns disabled. Do not resume an older-version map and do not use F12. For the first comparison, both players can choose Necropolis. WoG option 126 is optional; enable it on both clients if testing level-up rewards. Commanders must be enabled for champion quests. No extra starting army or automatic test gift is granted.

## Local acceptance first

Start a NEW local map with the installed build. On the first adventure turn, inspect `Debug/CloudTitansWorld.ini`: `version` must match the installed build, `error` zero and surface/underground equal when both levels exist. Read declared counts, not old trailing item rows. `Debug/CloudTitansAccess.ini`, section `native`, must show `artifact_guard=1`; stop and preserve Debug if protection is unavailable. Then hover and collect one component and check its name, picture and slot.

Map budgets increase by 10%, rounded up per layer, for all factions and sizes. Complete-pair caps for widths 36/72/108/144/180/216/252 are 20/40/60/80/100/120/140 total sites. Surface-only caps are 20/40/60/80/99/119/139. Valid-site shortages can reduce counts. A bounded top-up adds sites to spacing-limited plans while retaining at least four tiles of separation; it cannot guarantee a part on every explored route. Option 126 chance and spacing are unchanged.

Observe AI encounters and captured loot: no custom part or relic should remain with an AI. Human inventories, including other human players, must remain intact. Report the first violation with the matching save. The automated fixtures do not establish actual native interception or loot behavior.

## First shared test

1. Each player reaches their first adventure turn. Open `Debug/CloudTitansNetwork.ini` in the game folder and compare `version`, `placed`, `hash`, `surface`, `underground` and `world_error` on both computers. Errors must be zero. Counts must agree; surface and underground must be equal, up to 70/70 on G with adequate valid sites. A shortage reduces both equally. These read-only checks require no development gifts or quest-menu debug rows.
2. Hover and collect one map component. Hover, pickup picture/name and inventory must identify the same item and its equipment slot. A foreign faction part found on the map is allowed. After turn transfer, confirm that the object is absent on the other computer; the receiving player checks their inventory. A second visit must give nothing.
3. Finish one ordinary battle and record the winner's faction quest progress before/after. Then save together, exit normally, reload through the same Lobby workflow and check that player's progress/inventory again. Actual save/load and reconnect are acceptance tests, not established support claims.

Stop on the first wrong item, script error, mismatch or crash. Preserve both saves and relevant Debug folders locally. Record the exact action, turn, version, player and screenshots; do not repeatedly visit a failed object. Do not update either client during a running game.

## Sets and quests

All nine towns have eight components and an assembled relic. Worn distinct parts unlock cumulative bonuses; backpack items and duplicate copies do not multiply them. The relic represents all eight components. Its equipment slot is stated in its description. Assemble/disassemble through the mod's existing hero/town actions; disassembled parts go to the backpack. Keep space for the resulting items. Failed grants preserve the reward for retry.

Level-up and faction quest components follow the hero's faction. Custom artifacts are excluded from native random loot, so Dragon Utopia cannot award a complete custom relic. Human map finds can belong to another faction. AI heroes are excluded from our artifacts: native equipped/backpack/automatic grant paths are guarded, and load/day/prebattle cleanup removes existing custom AI inventory. This new native policy still requires player-run acceptance; it is not an established fix for earlier AI-turn crashes. Set quest targets receive another 5% reduction from dev13, rounded up: **404 / 3230 / 8075 / 80750 / 1615 / 808 / 122 / 8075**, with objective names and progress in the quest menus. Option 126 uses a 5% eligible component gate from level 18 and at least ten levels between component selections; a short game need not produce one.

Link an equipped relic to a matching owned developed town to test its weekly apex recruitment bonus. Compare hero and creature values before/after equipping/removing pieces, daily mana (including Intelligence capacity), duplicate items, full backpacks and town ownership changes. Linked growth, movement and native callbacks require in-game acceptance.

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

Choose **Champion quest** in a matching owned town to enroll and view the reward/progress checklist. Enrollment can precede qualification. To count the five qualifying wins, bring a level-25 hero with four distinct matching components (kept; the assembled relic also qualifies), all required ordinary town buildings and enabled commanders. Grail and optional coastal buildings are excluded; each town uses its own available Mage Guild maximum. Use only the faction's regular troops in those wins; commanders/machines do not interfere.

Leave town and Alt-left-click your own adventure hero for the final trial. Stronghold requires no hero spells in its trial; Conflux requires four distinct elemental steps. Return to the matching town with a free visitor space and fewer than eight heroes. A full roster, occupied visitor or unavailable matching unused native slot keeps the reward waiting. Delivery is complete only after the actual hero, town position, army and visitor checks pass. If an already prepared pending champion has moved away, bring that champion back to the delivery town before retrying; later progression is preserved.

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

The champion starts at level 1, zero XP and base **10/10/10/10**, with a fresh matching commander. Specialization works without the set; Andonov has stronger faction bonuses. Repeated delivery and loading must preserve later progression and commander state. Check real heroes, portraits, armies and commanders on both clients, not only counters.

## Known limits

The earlier AI-turn and fullscreen crashes have no established fix in this release. Matching hashes and offline fixtures do not prove compatibility with every mod or real Lobby transport. The online experiment uses sequential turns. Quick Combat, replay, trials, native spellbook presentation, complete champion lifecycle, weekly changes and multiplayer save/load remain separate acceptance steps.
