# Additional pre-Lobby checks — 0.5.0-nettest-alpha

2026-10-15. No gameplay changes and no version change were required.

- All 25 automated tests passed again.
- Clean local L random map, Default template, Tower selected, seed 1792082782: generated, WoG converted and entered the adventure screen without a crash. Ten components were placed, covering all eight IDs.
- In the real ERA process, called CLT_UnitTraits using an isolated 128-byte scratch structure initialized to Attack 100 / Defense 200 / Speed 10, with the complete necklace equipped. Giant 40, Titan 41 and Lord of Thunder 152 each returned 105 / 205 / 12. Golem 32 returned 102 / 202 / 11; Skeleton 56 stayed 100 / 200 / 10. This verifies the handler calculation, not a remote battle.
- Fixed progress receiver: 500 followed by stale 499 retained 500.
- Local native save/load preserved one equipped relic, 500 wins, ten placed components and map hash 11166. This is not a multiplayer save/load test.
- Daily mana handler awarded 10 from zero; invoking the same hero/day again kept 10.

The runtime probes, scratch structures, gifted relic and modified counters were confined to the isolated QA copy. They are not in the distributed package or the player's installation. The QA script on disk was restored afterward.

Still unverified: actual two-PC delivery through Heroes Launcher Online Lobby, PvP lightning, reconnect, shared save/load and a full multiplayer weekly growth cycle. Follow NETWORK_TEST.md for the two-player trial. Keep simultaneous turns and WoG option 126 off for this trial.
