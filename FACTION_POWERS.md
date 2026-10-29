# Owned hero parts and Commander training:0.6.0-batch-dev39

Close the game, update, restart fully and create a NEW map on matching39 clients.
No F12 or old saved-script refresh. Hero-set names are green for owned parts;
N/8and thresholds count only equipped parts. Commander Equipped/Collected counts
remain separate, with the redundant color-explanation sentence removed.

A complete Commander set or its relic trains after every12victories survived:
+1to Attack,Defense,Health,Damage,Magic Power,Speed and Magic Resistance. These
are flat additions to the native basic-stat calculation before existing ACM
multipliers. Minimum Damage is derived by the native calculation; Shots is not
one of the seven basic stats. Progress belongs to the Commander and set, remains
saved when gear is removed or combined, and contributes only while that set is
complete and equipped. Passing gear does not pass training. Partial/backpack
sets, dead/disabled Commanders and AI gain no training. No retroactive wins.

Actual native appearance/battle/save/load and two-computer acceptance still need
player testing. Original item growth and all dev38 map resources remain intact.

# Map artifact shadows and readability:0.6.0-batch-dev38

Close the game before updating, restart fully and create a NEW map on matching38
clients. Both native drawing masks are repaired for all90 individual map parts.
A narrow translucent silhouette and a stronger ground shadow separate thin and
pale subjects from textured terrain. Inventory artwork and gameplay are unchanged.
Actual native appearance needs player confirmation; offline terrain previews and
resource validation do not establish an in-game renderer pass. No F12.

# Commander renderer, collection and Damage/Health:0.6.0-batch-dev37

Close the game, update from the existing Mod Browser entry, restart fully and
start a NEW map on matching37 clients. Do not reload old saved scripts or use F12.
The Commander renderer crash is corrected. Descriptions show separate Equipped
and Collected progress; green names include backpack ownership and (2) indicates
two copies. Collection alone grants no bonus. Damage follows Health for these
three commander sets, including full sets/relics: Ember50%, Iron90%, Astral50%.
Other favored modifiers remain; the nine hero faction sets are unchanged.

Native equipment spot checks passed on the corrected renderer before the latest
collection/balance changes. Those latest changes need a fresh in-game check.
Battle/save/load, sustained AI/fullscreen and two-computer acceptance remain pending.
Older release sections below are historical when they conflict with this update.

# Standard commander combinations and victory rewards:0.6.0-batch-dev36

Close the game, update through the existing Mod Browser entry, restart fully
and create a NEW map. Both peers require36; old saved scripts are not migrated.
No F12. Follow COMMANDER_SETS.md for the current commander workflow; older
sections below are historical when they conflict with this update.

There is no Ctrl+N shortcut, separate commander menu or resource purchase.
Give parts to the normal Commander icon. With all six matching parts equipped,
right-click a part and confirm assembly; the window closes and one relic replaces
the set in the clicked slot. Right-click the equipped relic to dismantle.
Original artifacts and growth are retained; overflow parts need backpack space.
Refusal/cancel changes nothing. Each confirmed human victory also has a5%chance
of one random commander part, with no whole relic or AI rewards. A full backpack
consumes the attempt without rerolling. Normal loot is retained.

The map remains2copies per individual type,180finds,90/90layers, external map
monsters; hero-set rewards at18+7k remain unchanged. Native map shadows and all
artwork from35 are retained. Targeted offline checks do not establish actual
native rendering, combat, save/load or Lobby acceptance. No game/UI/install writes.

# Native Commander equipment and map shadows:0.6.0-batch-dev35

Close the game before updating through the existing Mod Browser entry; restart
fully and create a NEW map. Both peers must run35. Old saved scripts and the
former separate equipment ledger are not migrated. Do not use F12.

To equip a new commander part or relic, pick it up from the hero's backpack
and give it to the normal Commander icon, exactly as with an original item.
Open the Commander screen to see it in the actual six slots. Click its icon
to return it to the backpack; make room first. Right-click shows green N/6
progress. No Ctrl+N shortcut is required for equipping or taking items off.
Ctrl+N > Commander forge and relics remains an optional crafting menu.
New commander items cannot be worn on the hero. Carried items give no bonus.

Assemble six matching parts from the native commander slots and/or backpack.
The single relic uses one real slot; five remain available for original items.
Native shooting/revival/growth and existing battle counts are preserved.
Two matching parts still grant15 points to all eight ACM modifiers; a full
set/relic grants50 to all eight and90 total to its favored pair.

All90 individual map-artifact types now contain native translucent shadows.
Exactly2copies per type remain:180finds,90/90with underground. External map
monsters and level18+7k rewards are unchanged; no complete relics appear.

Targeted source/native-code fixtures and packed-resource checks pass. These
do not execute the game's renderer, battle engine, real save/load or Lobby.
First player acceptance: equip/take off one part through the normal icon,
inspect green1/6 and2/6 and changed attributes, assemble/equip a relic, retain
an original bow in another slot, then save/reload and compare peers.
No game was controlled and no installed file, setting or save was changed.

Earlier release notes below are historical when they conflict with this section.

# Map-density update: 0.6.0-batch-dev34

NEW maps contain two copies of each individual part:72 faction parts +18
commander items,180finds total,90/90with underground. No complete relics.
Level18+7k rewards are unchanged. Existing maps are not edited or reduced.
Both peers need34and a NEW map. All placements use the original external
adventure-map monster proximity check. No embedded armies, custom confirmation
or scripted battles are added; ordinary map guarding/movement rules apply.
Earlier version notes below are historical where they conflict with this update.

# Presentation update: 0.6.0-batch-dev33

English/Russian optional creator support and feedback links only. Gameplay files are identical to dev32, so runtime diagnostics still show32. Existing dev32 maps can continue; the underlying dev32 guide and its pending native acceptance limits follow.

# Legacy of the Cloud Titans â€” Online Lobby test

Version **0.6.0-batch-dev32**. This is an experimental all-faction release for a new two-player test. Automated checks pass; native gameplay, save/load and two-computer synchronization still need player verification.

## Install the same build

Both players close the game, then use the existing **Legacy of the Cloud Titans - TEST** entry in Heroes Launcher â†’ Mod Browser. Keep the folder **Cloud Titans Legacy - Local Test**; enable only one copy of this mod. The installed `mod.json` must say **0.6.0-batch-dev32** on both computers. Catalog metadata can lag behind downloaded files; an older version displayed in the browser does not establish which build was installed. Check the installed version before starting.

Use identical ERA/HD versions, enabled mods, load order and WoG options. The inspected base profile used ERA platform 2.299, HD 5.8 R22, Advanced Classes Mod 1.11, JS new objects 1.40, JS main module 1.21.2, JS commanders 1.02, JS map fixes 1.12 and JS terrains 1.4.1. Match the exact versions available to both players; TEST_PROFILE.json is an observed reference, not certification of every combination. Keep Knightmare Kingdoms and other metadata-listed incompatible packages disabled. Keep both ERAHDHeroes_3_Reborn (Full) and HD Editionfixai (Lite) disabled for this trial, following the selected remaster-free profile. Use their original Mod Browser files; this release does not patch them.

Start a **NEW G random map with underground through Heroes Launcher Online Lobby**, using sequential turns with simultaneous turns disabled. Do not resume an older-version map and do not use F12. For the first comparison, both players can choose Necropolis. WoG option 126 is optional; enable it on both clients if testing level-up rewards. Commanders must be enabled for champion quests. No extra starting army or automatic test gift is granted.

## Dev25 first checks

Click Sort in HD Backpack; it should close and rebuild with name-sorted items. The dev30 first-click regression and full-record permutation fixtures pass; actual current native click response and two-computer acceptance remain pending. On a NEW G map with underground, component plans retain equal layer totals and include some opposite-layer faction parts. Necropolis/Inferno/Dungeon must no longer be entirely absent from the surface. Old maps are not changed.

Enable option126. Verify missing own-faction parts at18,25,32,39 and every7 levels; check batch levels, other owned heroes and save/reload. Complete collections give ordinary Relics.

## Local acceptance first

Start a NEW local map with the installed build. On the first adventure turn, inspect `Debug/CloudTitansWorld.ini`: `version` must match the installed build, `error` zero and surface/underground equal when both levels exist. Read declared counts, not old trailing item rows. `Debug/CloudTitansAccess.ini`, section `native`, must show `artifact_guard=1`; stop and preserve Debug if protection is unavailable. Then hover and collect one component and check its name, picture and slot.

Dev34 uses exactly180 finds:2 copies of each of72 faction components and18 commander items. Complete relics are excluded. A successful two-layer plan has90 sites per layer and each item on both layers. Additional candidates are virtual until selected; no temporary ordinary artifacts are created. Insufficient suitable guarded space is an explicit error, not a successful reduced count.

Observe AI encounters and captured loot: no custom part or relic should remain with an AI. Human inventories, including other human players, must remain intact. Report the first violation with the matching save. The automated fixtures do not establish actual native interception or loot behavior.

## Dev20 / Dev21 / Dev22 local checks

Accept each quest family with a known hero. Switch town heroes and leave town: status must retain the recorded hero; fulfilled component objectives remain green. A substitute cannot claim or add victories. Lose the bound hero, then accept with a replacement: unfinished counters reset, the original faction remains locked, and claimed rewards stay claimed. Save/reload at each phase.

Open HD Backpack and click Sort at its top-right. Put down any artifact held on the cursor first. The popup closes and reopens after sorting so its cells reflect the current order. The inspected HD5.8R22 WoG provider is supported; Ctrl+N in the hero screen, then Sort backpack by name, remains the fallback if the button is unavailable. The town Inventory tools entry is removed. Check duplicates, distinct scroll spells, equipment and counts before/after, repeated sort and actual save/reload. Review all eight colored component names in an artifact tooltip; green=equipped, gray=not equipped. The set heading shows the current equipped count (N/8); an assembled relic counts as all eight. Backpack items do not count.

If the stack-experience rank table is blank, inspect the Stack Experience Rebalance configuration. Its own Runtime INI overrides its shipped JSON defaults. Enable Rebalance, WoG Stats, WoG Abilities and WoG Neutrals through that provider's configuration. The recommended Medium preset is +100% Health and Damage, +10 Attack/Defense and +10% Speed at rank10. TUM options require that provider and are separate. Restart/load after confirming. Each peer configures this separately; a Cloud Titans update does not overwrite another mod's options.

Dev23 writes a read-only check after game entry to Debug/CloudTitansStackExperience.ini. With the selected provider/settings active, the Vampire Lord sample should have six enabled stat rows and one ability row (seven total). Disabled settings and empty live rows are reported separately. This does not itself prove native table rendering or real combat application.

## First shared test

1. Each player reaches their first adventure turn. Open `Debug/CloudTitansNetwork.ini` in the game folder and compare `version`, `placed`, `hash`, `surface`, `underground` and `world_error` on both computers. Errors must be zero. Counts must agree; surface and underground must be equal, exactly90/90 on a successful two-layer map. An incomplete180-site plan is an error; start a larger/new map. These read-only checks require no development gifts or quest-menu debug rows.
2. Hover and collect one map component. Hover, pickup picture/name and inventory must identify the same item and its equipment slot. A foreign faction part found on the map is allowed. After turn transfer, confirm that the object is absent on the other computer; the receiving player checks their inventory. A second visit must give nothing.
3. Finish one ordinary battle and record the winner's faction quest progress before/after. Then save together, exit normally, reload through the same Lobby workflow and check that player's progress/inventory again. Actual save/load and reconnect are acceptance tests, not established support claims.

Stop on the first wrong item, script error, mismatch or crash. Preserve both saves and relevant Debug folders locally. Record the exact action, turn, version, player and screenshots; do not repeatedly visit a failed object. Do not update either client during a running game.

## Sets and quests

All nine towns have eight components and an assembled relic. Worn distinct parts unlock cumulative bonuses; backpack items and duplicate copies do not multiply them. The relic represents all eight components. Its equipment slot is stated in its description. Assemble/disassemble through the mod's existing hero/town actions; disassembled parts go to the backpack. Keep space for the resulting items. Failed grants preserve the reward for retry.

Level-up and faction quest components follow the hero's faction. Custom artifacts are excluded from native random loot, so Dragon Utopia cannot award a complete custom relic. Human map finds can belong to another faction. AI heroes are excluded from our artifacts: native equipped/backpack/automatic grant paths are guarded, and load/day/prebattle cleanup removes existing custom AI inventory. This new native policy still requires player-run acceptance; it is not an established fix for earlier AI-turn crashes. Set quest targets receive another10% reduction from dev24, rounded up: **328 / 2617 / 6542 / 65408 / 1309 / 656 / 99 / 6542**, with objective names and progress in the quest menus. Option126 guarantees a missing own-faction component at18,25,32,39 and every7 levels thereafter, checking all owned heroes. A complete collection gives an ordinary Relic instead.

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

Hold three resource reserves: **200,000 Gold**; **200 Wood and 200 Ore**; **200 each of Mercury, Sulfur, Crystal and Gems**. Resources and matching components are kept. The same conditions apply to all nine factions. The five ordinary qualifying faction victories remain required. There are no scripted champion trial battles.

After completing every requirement, place the bound quest hero in the matching town garrison (upper slot), leave the visitor space (lower slot) empty and select **Champion quest > Receive champion**. Close the town screen to complete delivery; the champion appears in that lower slot. Another hero cannot substitute. A blocked delivery keeps the reward available: move the bound hero into the garrison, free the visitor slot and keep fewer than eight heroes. Current qualification and resource reserves are rechecked at receipt. Native position, army and visitor readbacks must pass before completion. A prepared pending champion that moved elsewhere must return to the delivery town before retrying; later progression is preserved.

Ctrl+J or Alt-left-click now opens the bound hero checklist without combat. Old trial requests are inert. Start a NEW map on matching dev32 clients; old saves are not a supported migration path.

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

The earlier AI-turn and fullscreen crashes have no established fix in this release. Matching hashes and offline fixtures do not prove compatibility with every mod or real Lobby transport. The online experiment uses sequential turns. Quick Combat, replay, native spellbook presentation, complete champion lifecycle, weekly changes and multiplayer save/load remain separate acceptance steps.

## Dev27 local acceptance

Test the town-only champion quest on a NEW map. Check the resource amounts, incomplete-requirement and occupied-slot messages, retry after a blocked claim and exactly one level-one champion appearing in the lower slot without combat or resource spending. Save/reload and verify hero and commander progression. Actual native delivery/save-load and two-computer acceptance remain pending. This release removes the reported scripted-trial route; a general post-battle crash repair is not claimed.

Dev26 active set colors and Lich/Black Knight/undead Dragon component objectives remain included. Normal scenario difficulty does not override WoG map rules or Difficulty Mod growth. Third-party payloads and existing armies are unchanged.

Dev28 native spot check: Andonov was received through the real town menu on a protected local save; town exit/reentry, hero inspection and an actual save/reload passed. He remained level1 with25/25/25/25 and correct portraits. All18 portrait resources loaded correctly. This is limited local evidence; other individual champion lifecycles and two-computer synchronization remain pending.

## Commander sets — dev31

Press Ctrl+N in the hero screen and choose Commander equipment and forge.
Use its Helm, Weapon, Shield, Armor, Boots and Pendant slots; new items on the
hero or in the backpack provide no commander bonus. Native commander artifacts
reserve matching positions and suppress custom gear in those positions. You can
remove retained custom gear to a free backpack slot even if the commander is dead.

Every town can use all three sets. Each active piece grants5 percentage points
to the eight ACM commander modifiers. Matching2/4/6 parts add5/5/10 further points
to all; a full set adds40 to its favored pair. Complete Ember Oath favors Attack
and Damage; Iron Covenant favors Defense and Health; Astral Conclave favors Spell
and Passive. Full totals:50 points to all eight,90 to the favored pair. Bonuses
are added to ACM class modifiers, not hero stats, and do not accumulate on reopen.

Forge each item for50,000Gold,20Wood and20Ore using a level20 hero with an enabled
living commander. Forging creates a backpack item; equip it explicitly on the
commander page. All18 new icons have an item preview in the selection dialog.
AI cannot receive or activate these artifacts. Existing native commander items are preserved.

Development checked the source contracts of ACM1.11, JS commanders1.02 and WoG
Scripts, plus the neutral-commander mechanisms of Difficulty Mod, Arena rewards
and Enhanced Henchmen's separate equipment. This is not a runtime certificate for
every mod. Knightmare Kingdoms, ERA+, Land Of New Towns, ResOunD and TUM Enchanted
remain incompatible with this distribution. See COMMANDER_SETS.md for items,
the comparison with existing commander artifacts and pending acceptance.

## Two copies of every part on the map

Exactly2 copies of each of72 faction parts and18 commander items:180 finds,
without any complete assembled relic. Successful two-layer maps have90 sites
per layer, with each item represented on both. Ordinary eligible artifact sites
are reused first; additional placements use empty passable non-water/non-rock
land next to existing adventure-map monsters, with at least one clear cardinal
approach and without removing other objects. The planner
spreads finds, relaxing distance only when needed while keeping all coordinates
unique. Unused virtual candidates never create native objects. Successful sender/receiver fixtures verify identical native object-mutation order.

If insufficient safe space exists, the world diagnostic reports an incomplete
plan and no partial plan is certified/broadcast as complete. Do not use that map
for acceptance; create a larger/new random map. Actual ERA map-generation
acceptance remains pending. The seven-field map-site packet includes whether a
safe new site must be created on the receiving peer; both peers require dev32.

This map-only change does not alter level-up rewards at18,25,32,39 and every7
levels thereafter, quest rewards or relic assembly. No full relic drops.

## One-slot commander relics — dev32

Use Ctrl+N > Commander equipment and forge > Assemble six parts into one relic.
One of each matching part must be in this commander's custom equipment or the
hero's backpack. Hero-worn items must first be moved to the backpack. Assembly
has no extra charge and replaces exactly six parts with one backpack relic.
Equip that relic in the custom Pendant position; it reserves only native
commander position5, leaving positions0..4 for five native items and their
original abilities/growth. No extended ID is written into the native NPC table.

Ember Oath Relic, Iron Covenant Relic and Astral Conclave Relic preserve their
set's full50-point bonus to all eight ACM modifiers and90total to the favored
pair. These totals include thresholds; they are not added again. An assembled
relic counts6/6. Partial sets retain individual and2/4/6 thresholds: two active
matching parts give15points to all eight modifiers. Set headings show green
N/6; active names and earned thresholds are green, inactive names gray. Progress
updates for the inspected hero. Backpack and hero-worn gear never count active.

Only parts can be found or forged. All three complete relics are excluded from
map generation and native random pools; the180-item map plan is unchanged.
To dismantle, first unequip the relic to the backpack, leave five more empty
cells and choose Dismantle a backpack relic into six parts. Both operations
preserve unrelated complete artifact records and refuse safely on missing parts,
insufficient space, held artifact, wrong owner or stale/replayed conflicts.

Each assembled relic has its own original painted icon. Native visual, battle, save/load
and two-computer acceptance remain pending; no game was controlled. Matchdev32
on both peers and use a NEW map. The other public guide sections describe the
retained dev31 parts and base bonuses.
