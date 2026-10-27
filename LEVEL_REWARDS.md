# Option126 level-up rewards - 0.6.0-batch-dev25

Enable WoG option126. Standard reward classes remain Treasure at levels1-5, Minor at6-11, Major at12-17 and Relic from18. AI retains native rewards and cannot receive custom items.

## Balance

All nine factions receive one missing own-faction component on levels18,23,28,33 and every5 levels thereafter. Hero class determines faction. Check components in equipment and backpacks of all player-owned heroes; an assembled relic counts as all eight. Choose cyclically from a random local or deterministic network starting part, skipping owned pieces. If all eight are owned, return an ordinary allowed native Relic. No complete custom relic drops.

The original native option126 code alone grants and displays one reward per level. The selector adds no grant or separate RPC. Multiple-level gains pass each rewarded level individually, with earlier loop grants visible to later duplicate checks. Local last-selected state rejects repeated/out-of-order selections; network schedule is independent of query order and extra RNG. No prior missed rewards are reconstructed. Native full-bag grant failures are not refunded.

Map finds and quest claims remain separate; acquiring a part does not consume its quest. Start a NEW map after updating; old embedded scripts are not migrated.

## Verification

Executed ERM fixtures cover all18 hero classes, every ownership mask, other owned/enemy heroes, assembled relics, scheduled/off-schedule levels, multiple-level indices, reload state and ordinary fallback. These fixtures do not execute ERA inventory, save/load or Lobby transport. Native local evidence is recorded separately. Two independent computers must still verify turn transfer and saved inventories.

