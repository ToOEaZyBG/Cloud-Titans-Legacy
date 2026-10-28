# Commander sets - dev35

![The three assembled commander relics; artwork preview, not gameplay](Screens/commander-relics.png)

## Normal Commander equipment

Pick a new item up from the hero's backpack and give it to the normal
Commander icon, exactly as with original commander artifacts. It occupies
one of the actual six slots shown on the Commander screen. Click its icon
there to return it to the backpack; leave room first. Right-click shows
its description and green set progress. No Ctrl+N shortcut is required for
equipping or taking items off. New commander gear cannot be worn by the hero.
Items in a backpack give no bonus; disabled/dead or AI commanders get no bonus.

Parts may use any free native slot. Matching2/4/6 progress counts different
identities actually equipped on that commander, regardless of slot order.
Names and earned thresholds turn green; carried items remain inactive.

## Assembly and forge

Ctrl+N > Commander forge and relics is an optional crafting menu. Assemble one
of each of the six matching parts from native commander equipment and/or the
backpack, with no extra fee. The relic enters the backpack. Give it to the
normal Commander icon: it occupies one real slot, counts6/6 and leaves five
slots for original items, retaining their abilities and accumulated battles.
Represented same-set parts do not add duplicate bonuses alongside their relic.

To dismantle, return the relic to the backpack and leave five more free cells.
Choose Dismantle a backpack relic into six parts. Failures preserve all items
and resources. Only individual parts can be forged or found on the map;
complete relics never drop. Forging each part costs50,000Gold,20Wood,20Ore,
and requires a level20hero and a living enabled commander. Forging places
the part in the backpack; it does not silently equip it.

Exactly2copies of each72hero-set part and18commander parts appear on a
successful NEW map:180finds,90/90with underground. Separate adventure-map
monsters guard eligible locations under ordinary native movement rules.
The level18+7k hero-part rewards are unchanged.

Three universal sets, six items each. All nine standard towns and all ACM
commander classes can use every set. The sets share acquisition costs and a
480-point full-set attribute budget; actual combat balance awaits player review.

| Set | Favored modifiers | Items |
| --- | --- | --- |
| Ember Oath | Attack, Damage | Embercrest Helm; Rubycleaver; Shield of the Ember Oath; Emberforged Cuirass; Ashwarden Sabatons; Heart of the Ember Oath |
| Iron Covenant | Defense, Health | Ironwatch Helm; Covenant Mace; Shield of the Iron Covenant; Ironbound Breastplate; Covenant Greaves; Seal of the Iron Covenant |
| Astral Conclave | Spell, Passive | Astral Circlet; Conclave Scepter; Shield of the Astral Conclave; Starwoven Cuirass; Astral Treads; Conclave Astrolabe |

![All18 new commander artifacts](Screens/commander-sets.png)

Original artwork preview, not a gameplay screenshot. Native icons use the
existing44x44 inventory palette with clear margins. Artwork is pending player
approval and may be revised following feedback.

## Bonuses

Each active part adds **5 percentage points** to all eight ACM commander
attribute modifiers: Attack, Defense, Damage, Health, Speed, Spell, Passive and
Aura. Matching2/4/6 parts add another5/5/10 points to all eight. A complete set
adds40 further points to its favored pair.

Full set: **50 points to every modifier,90 to the favored two**. These are added
to ACM's existing modifiers. For example, an existing100% Damage modifier becomes
190% with a complete Ember Oath; an existing200% becomes290%, rather than380%.
No hero stat, learned ability or commander class is replaced. Mixed sets retain
their individual and earned same-set thresholds, without a full-set favored bonus.

## Comparison with existing equipment

The shipped WoG feature manual describes native commander equipment with growing
bonuses: Axe of Smashing gives5Attack and1 more per6victories; Mithril Mail
gives12%Health plus1 point per victory; Sword of Sharpness gives12%Damage plus1
point per victory; Pendant of Sorcery and Boots of Haste improve their respective
stats with victories. Other items offer revival, shooting, dragon properties or
advanced skills. Native utility effects are intentionally retained.

ACM changes this baseline. Its commander calculation gives10 points to all eight
modifiers for each worn Bow of Seeking, Dragon Eye Ring and Slava's Ring, plus
15Spell points and win scaling for Pendant of Sorcery. It also changes artifact
effects when those artifacts are worn by the hero. This is why new commander
gear is measured against the ACM calculation, rather than old tooltip text alone.

Our full sets offer a larger broad attribute budget and a role bonus. They do
not promise to beat every native utility effect or unbounded victory counter
in every situation. Further balance changes will follow actual play feedback.

## Compatibility and acceptance

Dev35 adds a checked native transfer/render bridge for the original six-slot
Commander screen. It preserves original artifacts, NPC record layout and
ordinary save/network transfer. ACM1.11's eight normal modifiers are augmented;
class previews and alternate resistance outputs are preserved. Other mods'
classes, original item growth and Enhanced Henchmen's Warlord Banner remain
unchanged. Existing metadata incompatibilities still apply; this is not
certification for every mod or future native-plugin version.

Close the game before updating, restart fully and use matching dev35 clients
with a NEW map. Old saved scripts and former equipment-page ledgers are not
migrated. The bridge refuses new equipment transactions on unsupported native
code or old scripts. No F12. Targeted headless tests and resource gates pass;
actual native UI, battle, save/load and two-computer acceptance remain pending.
No game, installed file, setting or save was changed during this development.
