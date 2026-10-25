# Option 126 level-up rewards — 0.6.0-batch-dev24

Enable WoG option 126 to test. Standard reward classes remain Treasure at levels 1–5, Minor at 6–11, Major at 12–17 and Relic from level 18 onward. AI retains native rewards. Human Relic rewards can select components of the hero faction. Complete custom relics never drop.

## Balance

Each eligible human Relic level reward has a **5% component gate**. On the tenth eligible attempt after nine failed gates, a component is guaranteed. After a component selection, another cannot be selected until **at least ten levels later for that hero**: a selection at level 20 permits the next attempt at level 30. Levels 21–29 give ordinary rewards. This limit applies to option 126 only; map artifacts and quest rewards are separate. A level-up component does not consume the corresponding once-per-player quest reward, so another hero can receive a second copy through that quest.

For local games, the first nine eligible attempts use a 0–99 random roll below5. The tenth attempt selects a component without another gate roll. Miss counts, last attempt and last selected component level are saved per hero in SN:W; cooldown levels do not advance pity and duplicate-level calls do not charge it twice. For network games, a deterministic schedule uses the shared map hash, hero ID and each rewarded level. It recomputes prior scheduled successes to enforce the same ten-level gap on all peers without depending on peer-local cooldown or an extra artifact-grant message. This sequence is deterministic rather than independent random rolls; its raw gate covers approximately5% of hash residues. The tenth-eligible-attempt guarantee and ten-level cooldown are reconstructed from the same deterministic history on every peer.

When multiple levels are gained together, each reward uses the original start level plus its own reward index. Thus a large experience award cannot bypass the ten-level gap. Network results do not depend on the order in which the schedule is queried. Component type is selected separately from the allowed standard Relic pool, so the number of allowed standard Relics no longer increases the component rate.

The original WoG code alone grants and displays one reward per level. These limits concern component **selections**; a failed native inventory grant is not refunded by this selector. Custom selections are logged in Debug/CloudTitansRewards.ini, including hero, level and artifact ID. Failed eligible attempts also update the latest attempt fields. Logs are not proof of inventory delivery.

## Compatibility and verification

The package changes only two reward-selection calls in the pinned 77 wog - map rules.erm. The human call passes its individual reward index; the AI call passes zero. Original SHA-256: 94db153050a700920454bc4e3a16eeae4e74d8c7b2aa85299abaa51633256c63. Recheck this override after WoG Scripts updates.

Tests execute the actual pure ERM arithmetic and schedule helper instructions in a limited offline evaluator. They check bounds, approximate gate frequency, ten-level spacing and order-independent network decisions. Other tests inspect the native integration and preservation of grants/dialogs. They do not execute ERA, prove inventory delivery or establish peer synchronization. The 0.5.4 balance and UI changes still need runtime testing.

Start a NEW map through Online Lobby with simultaneous turns off. Test level 18+, several levels gained together, a full backpack, save/load and further levels. Compare inventory and counters on both clients after turn transfer. With option126 active from level18, an uninterrupted new-map sequence selects its first component no later than level27. Later selections remain at least ten levels apart. An existing old save is not retroactively awarded missing rewards.

