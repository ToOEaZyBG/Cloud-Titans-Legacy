LATEST PUBLIC BUILD: 0.6.0-batch-dev25

--------------------------------------------------------------
## CHANGELOG

27/10/2026 dev24 > dev25
- All nine castles: component quests are another10% easier.
- Guaranteed missing own-faction component at levels18,23,28,33 and every5 levels thereafter with option126. Check all owned heroes; a complete collection gives an ordinary Relic instead.
- Double the spacing-limited map top-up target, within existing guarded-site,55% density,140-site and equal-layer limits. Start a NEW map.

26/10/2026 dev23 > dev24
- Fix Sort and the Relics page button to handle the native completed-click event rather than mouse-down.
- Correct opposite-layer artifact selection: all nine towns can have parts on both layers; new map required.
- Keep the5% level gate and ten-level cooldown; guarantee a component on the tenth eligible attempt. Log failed attempts as well as successes.

25/10/2026 dev22 > dev23
- All nine newly awarded champions start at level1 with 25 Attack, Defense, Spell Power and Knowledge; later progression is preserved.
- Add read-only live stack-experience row diagnostics and clarify the provider-owned switches needed for rank bonuses. Restore the selected WoG profile locally without changing third-party payloads.
- Include the HD Backpack Sort button from dev22. Native table/button rendering and two-computer acceptance remain pending.

25/10/2026 dev21 > dev22
- Add Sort directly to the HD Backpack window; sorting closes and rebuilds the popup to refresh every cell.
- Reuse the existing full-record name sort and online transaction, preserving scroll spells and equipment.
- Guard the integration for the inspected HD5.8R22 WoG provider; retain Ctrl+N as a fallback. Native UI and two-computer acceptance remain pending.

25/10/2026 dev20 > dev21
- Increase every custom artifact primary and equipment/set stat bonus by50%, rounded up per positive bonus.
- Show equipped parts in green, other parts in gray and the current equipped count as (N/8), following the native artifact presentation.
- Keep spell costs, quest targets, growth, special battle powers and30% Life Leech unchanged. New map required; native and two-computer acceptance pending.

25/10/2026 dev19 > dev20
- Includes the previously private dev19 quest/inventory work; the previous public build was dev18.
- Bind component/champion quests to the accepting hero and one permanent faction per player; reset unfinished progress after hero loss.
- Reduce all component quest targets by another10%; show completed objectives outside town and compact quest rows.
- Add colored component checklists and backpack name sorting; repair champion trial input with Ctrl+J alternative.
- Remove the town Inventory tools entry; sorting remains available with Ctrl+N in the hero screen. The Backpack-window button is not included yet.
- No PRIVATE QA script or menu in the delivered package. 539 offline regression checks passed before this menu cleanup; current release checks are recorded in VALIDATION.md. Native battle/save/Lobby acceptance remains pending.

--------------------------------------------------------------

## LEGACY OF THE CLOUD TITANS - TEST

Collect your town's artifacts, assemble its legendary relic and earn a unique faction champion.

Legacy of the Cloud Titans adds an artifact-collection and hero-progression system to all nine standard towns in Heroes III ERA: Castle, Rampart, Tower, Inferno, Necropolis, Dungeon, Stronghold, Fortress and Conflux. Explore the map for components, complete faction objectives and build a matching collection that strengthens your hero and army.

## WHAT YOU GET

- Nine faction sets: eight components and one assembled relic for each town.
- 72 components and nine complete relics in total, with themed artifact artwork.
- Individual item effects and cumulative bonuses for wearing different matching pieces.
- Faction artifact quests with objective descriptions and progress tracking.
- Eight manual relic powers, plus Tower's automatic lightning mechanic.
- Nine champion quests with named heroes, custom portraits and faction specializations.
- A relic-to-town link that increases weekly recruitment of the faction's top-tier creature.

## FIND AND EARN COMPONENTS

Map exploration: some eligible loose artifact sites become faction components when a new map is prepared. Finds can belong to any town. On maps with an underground level, the generated plan keeps equal component counts above and below ground. Availability depends on valid locations; exploring a particular area does not guarantee a component.

Faction quests: open Faction set quests in your town menu. Each component has an objective and a progress counter. Defeat the listed enemies or complete the required battles, then return with the recorded qualified hero to claim it. Completed objectives stay green while that hero is away. Read the selected objective for its level and town requirements. Choose Accept with the hero in town. Only that recorded hero earns progress. Your first component or champion quest permanently locks one faction for this game. Death or dismissal resets unfinished progress; a replacement may accept for the same faction. Previously claimed component rewards remain claimed, once per player. Finding a piece elsewhere does not consume that quest reward.

Level-up rewards: with WoG option 126 enabled, eligible human Relic-category level-up rewards can offer a matching-faction component. A missing own-faction component is guaranteed at levels18,23,28,33 and every5 levels thereafter. Equipment and backpacks of all owned heroes count; assembled relics represent all eight parts. A complete collection gives an ordinary Relic instead.

Custom relics are assembled from components; Dragon Utopia does not award a complete custom set. Level-up and faction-quest component rewards follow the hero's faction. A foreign-faction component found on the map is allowed.

## WEAR A SET AND ASSEMBLE ITS RELIC

Different worn pieces unlock cumulative set bonuses. Components in the backpack do not count, and extra copies of the same piece do not multiply those bonuses. Item descriptions explain the effects and equipment slots.

Collect all eight different components and use the assemble/disassemble action in the faction quest menu. The assembled relic represents the full collection. Its slot depends on the relic. Disassembly returns the components to the backpack, so leave enough space.

Visit a matching owned developed town while wearing the relic to link its weekly top-tier recruitment bonus. The highest-level dwelling is required.

## BACKPACK AND SET CHECKLISTS

Click Sort in the HD Backpack window, or press Ctrl+N in the hero screen and select Sort backpack by name. Names are grouped alphabetically; scroll modifiers, duplicates, equipment and backpack capacity are preserved. Put down any held item first. The current reviewed profile supports artifact IDs0-530; unknown extensions are left unchanged.

Our artifact descriptions list all eight matching parts: gold means worn, green means owned but not worn, gray means missing. An assembled relic represents all eight. Only equipped pieces contribute set bonuses.

## USE YOUR RELIC'S BATTLE POWER

For the eight manual powers, wear the assembled relic and open the battle spellbook on your own stack's turn after Tactics. Select Relics at the bottom, then the set's icon. Eight separate components do not unlock the manual power. Each relic has one manual activation per battle and a mana cost; canceling spends nothing.

- Castle: Seraphic Restoration restores fallen troops using a shared resurrection allowance.
- Rampart: Forest's Embrace combines protection with healing for its top creatures.
- Inferno: Infernal Gate summons temporary Horned Demons.
- Necropolis: Life Harvest damages living enemies and restores undead troops. Its relic also adds 30% Life Leech to controlled units' physical attacks against living enemies.
- Dungeon: Abyssal Rift strikes a selected target with Implosion.
- Stronghold: Warlord's Fury combines Haste with Attack-based physical damage.
- Fortress: Primordial Venom opens a limited Poison window.
- Conflux: Elemental Invocation offers four elemental choices.

Tower uses automatic lightning for Giants, Titans and Lords of Thunder instead of a manual spellbook power. Supported creature upgrades are included in the relevant faction effects; commanders and war machines are excluded from regular-troop bonuses.

## EARN YOUR FACTION CHAMPION

Choose Champion quest in a matching owned town to enroll and view the reward and progress checklist. Enrollment is available before you meet the battle requirements.

To count the five qualifying victories, use a level-25 hero carrying four distinct matching components, or the assembled relic, and meet the town-building requirements. Commanders must be enabled. Fight with that faction's regular troops; commanders and war machines do not invalidate the army. The Grail is not required.

After the victories, leave town and Alt-left-click the bound quest hero to begin the final trial, or press Ctrl+J on the adventure map. Component and champion quests each record their accepting hero; another hero cannot substitute. Return the bound hero to the matching town and put them in the garrison, leaving the visitor space free; keep fewer than eight heroes to receive the champion. A blocked delivery keeps the reward pending.

Castle: Aldric. Rampart: Sylvara. Tower: Vaelion. Inferno: Zareth. Necropolis: Andonov. Dungeon: Nyssara. Stronghold: Kargan. Fortress: Ssareth. Conflux: Aurelis.

Champions start at level 1 with 25 Attack, 25 Defense, 25 Spell Power, 25 Knowledge and a matching commander. Their faction specialization works without wearing the set. Andonov has stronger faction bonuses.

## STARTING A GAME

Requires Heroes III ERA, WoG, Era Erm Framework, WoG Scripts, Game Enhancement Mod and Advanced Classes Mod. Enable one copy of Legacy of the Cloud Titans - TEST and start a NEW map. Keep old saves with their matching mod version. Close the game before updating; do not use F12 to update a running game.

The current trial profile keeps Knightmare Kingdoms, the Full/Lite HD remaster packages and the other packages listed as incompatible in mod.json disabled. Support for one creature's upgrades does not establish compatibility with every creature pack.

For an online test, both players need the same build, dependencies, mod order and WoG options. Use sequential turns. Local gameplay, native AI artifact exclusion, save/load and two-computer Online Lobby acceptance are still under testing. This is an experimental release; the earlier AI-turn and fullscreen crashes have no established fix.

## REPORTING A PROBLEM

Keep the save and Debug folder locally. Record the installed version, faction, exact action and a screenshot of the first error. Include whether it happened locally or through Online Lobby. Detailed test instructions are in NETWORK_TEST.md.

## Artwork gallery

![Andonov — Necropolis champion](Screens/quests.png)

[View all nine champion portraits, faction sets and relic close-ups](GALLERY.md). Artwork previews; not gameplay screenshots.
