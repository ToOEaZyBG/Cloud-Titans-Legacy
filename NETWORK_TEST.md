# Cloud Titans 0.5.4-nettest-alpha — Online Lobby Test

Experimental multiplayer test release. **50 automated checks pass; the gameplay changes have not yet been verified in ERA or between two computers.** User-driven 0.5.2 tests with two clients on one computer confirmed battle-counter transfer and persistence after save/load, quest browsing without a hero, and receiving components from option 126. The new 0.5.3 fixes still require in-game verification.

## Installation and setup

1. Both players must close the game before installing or updating **Legacy of the Cloud Titans - TEST** in Heroes Launcher → Mod Browser. The required installed version is **0.5.4-nettest-alpha**. See [UPDATING.md](UPDATING.md) if the catalog shows an older version or repeatedly offers Update. Do not use F12 during multiplayer.
2. Use matching ERA/HD versions, enabled mods and load order on both computers. TEST_PROFILE.json describes the test profile; it is not a replacement for your settings.
3. Start a **NEW random map through Online Lobby**, with both players choosing Tower. Maps created with 0.5.0–0.5.2 are not migrated. In particular, old custom hint state may remain in saves; use a new map to test the hover fix. Disable simultaneous turns. Enable WoG option **126 (artifacts awarded on level-up)** to test level rewards; human heroes can receive a set component from level 18 onward. See LEVEL_REWARDS.md.
4. Test with sequential turns. Successful local testing does not establish that online synchronization works.

## Changes in this release

- Show already-owned components in quest rows/details without blocking the separate once-per-player quest reward.
- Network status also displays quest write errors.


- Remove custom map-object hint assignments that can enter the legacy hover path with an invalid text index. Custom graphics and pickup reward names are retained; the native map hint may show the underlying standard artifact name.
- Correct two quest requirement string assignments rejected by ERA.
- Use a shared numeric state reader for quest list/detail views and refresh town ownership/hero context after the modal selection dialog. This targets the reported list/detail progress mismatch.
- Option 126 now uses a 5% component gate and a minimum ten-level gap per hero, from level 18. Network selection recomputes a shared per-map/per-hero schedule; local selection saves its cooldown. See LEVEL_REWARDS.md.


- Option 126 now includes human Relic component rewards in network games. Online selection is deterministic per hero and rewarded level, without an extra RNG call or an extra item grant. Multiple levels gained together use distinct level inputs. Actual network behavior still requires testing.


- Network operations apply locally before being broadcast. Receivers include duplicate protection.
- Quest progress can be viewed in a Tower without a visiting hero. Each objective states what it counts. Hero level 25 and all ordinary Tower buildings, including Mage Guild level 5, are required only when claiming a reward. The Grail building is excluded.
- New blue-and-gold artifact sites use a standard artifact ID with separate custom graphics. A coordinate registry identifies the set component. The pickup handler checks delivery before removing the object. This is a candidate fix for incorrect rewards, objects remaining on the map and crashes on a second visit; in-game verification is pending.
- Fixed network entry points 26891–26897 are used. Debug/CloudTitansQuests.ini records the latest committed quest progress.
- Quest targets and rewards are unchanged. No army is granted automatically.

## Online test checklist

1. Let each player take their first turn. In Tower, open the additional town actions → **Cloud Titans network test → Show network status**. Compare Build, Placed and Map hash on both computers. They should match; Errors should be 0.
2. Win and finish one normal battle. The crown objective should increase by one, and total enemy kills should reflect enemy losses. End the turn and compare recorded wins in Network status on both computers.
3. Test Quick Combat separately. Zero progress was previously reported with both Quick Combat and normal battles; Quick Combat has not been established as the sole cause, and its support is not yet confirmed.
4. Collect a blue-and-gold artifact on the map. Check that the correct component is received and the object disappears. Visiting the same tile again must not grant another item or crash. Check the other computer after ending the turn. Stop this test if an incorrect item is awarded.
5. For a short assembly test, use **Receive 8 components - test only, once per player** with an owned hero in Tower and eight free backpack slots. This optional test action is never automatic. Check assembly, disassembly and duplicate prevention.
6. Then test a full backpack during pickup/disassembly, PvP and lightning, Giant/Titan/Lord of Thunder bonuses, removing the set, losing the linked Tower, daily and weekly transitions, and multiplayer save/load.

If a crash, incorrect item or synchronization mismatch occurs, preserve both saves and Debug folders and stop that test. Two-computer delivery, reconnection, a complete weekly cycle and multiplayer save/load remain unverified. Matching map hashes alone do not prove correct pickup or combat bonuses.

## Option 126 test

With option 126 enabled, level a human hero through 17, 18 and several higher levels. Check both single-level and multiple-level gains. Rewards below 18 keep the native class; from 18 onward, each eligible reward has a 5% component gate, with at least ten levels between component selections; other rewards are standard allowed Relics. The assembled necklace cannot drop. Check inventory and reward dialogs, then save/load and continue leveling. A component is not guaranteed on any particular level. For two humans, compare the awarded item on both computers after turn transfer.
