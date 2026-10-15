# Option 126: artifacts awarded on level-up — 0.5.2-nettest-alpha

Enable WoG option 126 before starting the new test game. The eight Cloud Titans components participate in human Relic level rewards in local and network games. The assembled necklace never drops.

## Reward rules

The original WoG reward classes remain: Treasure at levels 1–5, Minor at 6–11, Major at 12–17 and Relic from level 18 onward. Each eligible human Relic reward selects from one ticket per allowed standard SoD Relic (IDs 7–128), plus one ticket for each of the eight components (450–457). The combined component chance in local random selection is `8 / (allowed standard Relics + 8)`.

Local games use the existing random ticket selection. Network games use a deterministic ticket derived from the hero ID and the individual rewarded level, so the custom selector does not advance the RNG. This is a fixed selection sequence, not an independent random roll. All peers need matching mods and artifact availability. Multiple levels gained at once use the original start level and each reward's array index; they do not all use the final hero level.

The original WoG script remains responsible for granting exactly one artifact and displaying it. The selector does not grant another item or send a separate grant message. Duplicates remain possible; there is no guaranteed component or full set. AI and lower reward classes retain native selection. Exhausted native reward pools outside the human Relic selector have not been changed by this release.

## Integration and limits

The package overrides two selection calls in the pinned `77 wog - map rules.erm`. Original SHA-256: `94db153050a700920454bc4e3a16eeae4e74d8c7b2aa85299abaa51633256c63`. The human call passes the reward index; the AI call passes zero. Other native grant/dialog logic is unchanged. Recheck this override after updating WoG Scripts or installing another override of that file.

No new game process was launched to validate 0.5.2. Automated checks inspect integration and execute the arithmetic expressions in a small offline evaluator; they do not execute ERA or prove two-peer synchronization. Earlier local selector tests do not establish that this update works online.

## Test

Start a new Online Lobby map with option 126 enabled, simultaneous turns disabled and matching versions on both computers. Test level 18+, gaining several levels at once, a full backpack, save/load, and another level after loading. Verify the actual awarded item and dialog. With two human players, compare the hero's inventory on both machines after turn transfer. Custom selections are logged in `Debug/CloudTitansRewards.ini`; these entries describe selector output, not proof of successful delivery.
