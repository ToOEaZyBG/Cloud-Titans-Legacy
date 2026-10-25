# 25/10/2026 dev18 > dev20 - 0.6.0-batch-dev20

- Explicit hero enrollment for both component and champion quests; only the bound hero earns progress. First acceptance permanently locks one faction per player. Hero loss resets unfinished progress and permits a same-faction replacement; previously claimed components and delivered champions remain once-only.
- Include hero/generation identity in progress/trial packets and exact identity in reset packets, rejecting late old-hero traffic. Keep completion green outside town; require the recorded hero present for claims and champion delivery.
- Reduce every component target by another10%, rounded up:364/2907/7268/72675/1454/728/110/7268. Compact objective rows while retaining all upgrade eligibility in full details.
- Add colored lists of all eight set parts to artifact descriptions. Provide Sort backpack by name through Ctrl+N in the hero screen; omit the extra town Inventory tools entry, preserving complete artifact records and sending the chosen permutation online.
- Use the official adventure mouse event/modifier data for Alt-click trials; add Ctrl+J for the recorded quest hero.
- The installed private QA helper is removed during the closed-game update; no QA helper is shipped. A sort button inside HD Backpack is still pending and is not claimed in this release.
- 539 offline tests pass. Native acceptance is pending while this candidate is reviewed; no actual save/load or two-computer pass is claimed here.
- Fully close the game before updating. Start a NEW map and match the complete build/profile with the other player.

# 20/10/2026 dev17 > dev18 - 0.6.0-batch-dev18

- Separate the internal map-frame names from inventory frames for all64 added faction components. Read-only inspection of the failed dev17 game found46 map templates using the exact44x44 inventory payload instead of their32x32 adventure frame. All5 observed Tower templates used their correct map frame and already had distinct names.
- Change only those internal frame names in map resources; retain artwork, palettes, geometry, masks, Tower resources, inventory, native plugin, slots, budgets, equal surface/underground counts and quests.
- Reject case-insensitive global DEF frame-name conflicts across every bundled archive and loose resource before release. Identical packed/loose copies remain permitted.
- 257 offline tests pass. Native spot checks on a new G map covered16 identified map items across all nine sets and all eight Inferno component types. All48 different loaded custom map frames matched their correct32x32 map payloads, before and after one actual save/reload. The map had62 sites,31 per layer.
- Close the game fully before updating, then use a NEW map. Individual pickup/equipment checks for all72 parts, full quest/power lifecycles and two-computer Lobby acceptance remain pending.

# 20/10/2026 dev16 > dev17 — 0.6.0-batch-dev17

- Compile all72 map components into a32x32 sprite with matching one-cell MSK/MSG bounds, eliminating the unused blank left tile. The artwork fits within a one-pixel gutter and retains its independent palette.
- Applies to every town and component. Inventory artwork, identities, slots, map budgets,1:1 layers and quests are unchanged.
- Show the current public build and six dated changelog entries before the mod description; preserve the complete additive GitHub history.
- 253 offline tests pass. This is a candidate correction for reported half-visible map artifacts; actual terrain rendering still requires player acceptance. No native gameplay or Lobby pass is claimed.

# 0.6.0-batch-dev16 - clearer adventure-map components

- Increase component map artwork to a maximum30 pixels with a clear tile gutter.
- Compile every component with its own map palette, preserving faction colors independently from the inventory palette. Tower and the eight additional towns use the same map compiler.
- Inventory icons, artifact identities/slots, object masks, placement budgets, equal layers and gameplay rules are unchanged.
- 249 offline tests pass, including decoded native sprite geometry, color fidelity and Tower archive/mask preservation. Native map appearance still needs player acceptance.

# 0.6.0-batch-dev15 - startup call hotfix

- Fix the AI artifact-guard readiness call: an explicit STDCALL convention is required even for a function with no arguments.
- The access fixture now rejects the original malformed call and uses the real framework convention constants.
- All dev14 balance and AI-policy changes remain included. 245 offline tests pass; native startup, AI behavior, save/load and Lobby acceptance still require player verification.

# 0.6.0-batch-dev14 — experimental local / Online Lobby test

- Map component budgets increase by 10% on all map sizes, rounded up per layer; underground maps retain equal complete pairs. G supports up to 70/70 sites when eligible locations suffice. A bounded spacing top-up helps plans that previously stopped below the nominal cap.
- All nine component quest targets receive a further 5% reduction from dev13, rounded up. Champion requirements and option 126 chance/spacing are unchanged.
- Native equipped, backpack and automatic grant paths reject custom artifacts for AI. Safe load/day/prebattle cleanup removes existing AI custom inventory. Human and ordinary artifact grants are preserved. Actual native enforcement needs local acceptance.
- Explicit local world counts and an artifact-guard readiness diagnostic support the first new-map test.
- 244 offline tests pass. No actual game, native save/load or two-computer Lobby test ran. Earlier AI-turn/fullscreen incidents remain unresolved; this is an experimental build requiring a NEW map.

# 0.6.0-batch-dev13 — experimental Online Lobby test

- Champion delivery now verifies the hero's actual town coordinates. A refused initial move remains retryable; an already prepared champion keeps later progress and must return to the delivery town.
- A completed map plan cannot shrink or gain new sites from late packets. Inconsistent completion counts are rejected, and map errors are written to the network diagnostic file immediately. Equal surface/underground counts remain 1:1.
- Very large battle kill totals saturate quest counters before integer overflow. Quest targets and rewards are unchanged.
- 233 offline tests pass, including the combined battle-result/quest path, replay cancellation, independent receivers, initial placement and inspected ACM attack dispatch. Native gameplay, actual save/load and two-computer Lobby acceptance remain pending. Earlier AI-turn/fullscreen incidents have no established fix.


# 0.6.0-batch-dev12 — experimental all-faction Online Lobby test

- Nine faction sets, champion quests/portraits/specialties and matching commanders.
- Correct map hints/pictures/shield silhouette; own-faction controlled rewards and no complete relics in native loot.
- Equal surface/underground component counts, bounded candidate space reserved for both levels and 15% lower set objectives.
- Painted in-book relic page, eight manual powers and additional Necropolis physical Life Leech.
- Verified champion delivery retry phases; real ACM mana capacity; backpack-preserving forge rollback.
- Immutable map packet identity and complete-plan validation; expanded persistence/replication fixtures.
- 213 offline tests pass. Native gameplay and two-computer Lobby acceptance remain pending; old AI-turn/fullscreen incidents have no established fix.

# 0.5.4-nettest-alpha — combined test update

Includes the 0.5.3 hover and quest display fixes, plus all currently agreed changes for the next test:

- Option 126: 5% component gate from level 18, with at least ten levels between selections per hero. Local saved cooldown; deterministic map-salted schedule online. Multiple-level gains respect the same spacing.
- Quest ownership labels count components held by all owned heroes, including parts represented by the assembled relic. Owning a part never blocks the separate once-per-player quest reward.
- Quest list/detail use one numeric state reader; requirement strings use the correct string assignment command.
- Map sites retain custom graphics and pickup names, with unsafe custom map hints removed.
- Network status exposes quest write errors separately.
- 50 offline tests pass. Runtime verification is pending for these changes; start a NEW map and keep both clients on the same version.
- The reported crash during fullscreen switching remains unresolved; no speculative graphics/native patch is included.

# 0.5.3-nettest-alpha

- Stop assigning trigger-local string references as persistent map-object hints. This targets the generic legacy hover error reported as File: erm, Line: 9614.
- Correct two VR:Z assignments on a local string in quest requirements (use VR:S).
- Read quest list/detail progress through one numeric helper; refresh town owner and hero after the selection dialog. Targets the reported Aegis 1275/10000 versus 0/10000 mismatch.
- Start a NEW map: existing native hint state in saves is not migrated.
- 44 offline checks pass; these fixes still need user-driven runtime verification. Two clients on one computer are not a substitute for a two-computer test.
- Option 126 balance is unchanged; the requested lower rate and ten-level limit remain pending.

# 0.5.2-nettest-alpha

- Enable the eight human Relic component rewards for WoG option 126 in network games, from level 18 onward.
- Use deterministic hero/reward-level selection online, without an extra RNG call, separate grant packet or extra item.
- Preserve native grants/dialogs and distinct reward-level inputs when several levels are gained together.
- Keep AI, lower reward classes and gameplay balance unchanged.
- 34 automated checks pass; ERA and Online Lobby verification remain pending. Both players must close the game and update together. Start a new map for the test.

# 0.5.1-nettest-alpha

Published test candidate; the user will verify changes through Online Lobby. No native/runtime pass is claimed for this update.

- Apply idempotent operations locally before broadcast; add progress readback diagnostics.
- Browse quest progress without a hero; label counted objectives.
- Native-ID map proxies and guarded, idempotent component pickup; consume only after delivery.
- Fixed wire entry 26897 for pickup; existing six IDs unchanged.
- New random map required. Old 0.5.0 maps are not migrated.
- Hard quest targets, level 25/full ordinary Tower claim requirements and balance unchanged.

See NETWORK_TEST.md. VALIDATION.md describes earlier 0.5.0 local checks, not this update.


## Preserved project beginnings and local development milestones

This appendix fills gaps in the original public changelog without deleting its
existing release entries. Dates below are recorded milestone dates in
Europe/Berlin. Local/private milestones are explicitly distinguished from
public releases. The earliest preserved source baseline is0.2.13 on15/10/2026;
work before that baseline is not completely documented, so no missing dates,
versions or successful tests are invented here.

### 15/10/2026 — earliest preserved Tower baseline0.2.13

- One Tower faction collection, equipment/set effects and local test roadmap.
- Guarded random-map acquisition without starting gifts; startup checkpoints
  and original Tower map drawings followed on the same date.
- Local human component rewards were classified as Relic from level18.
- Tower component quests, hero/town development requirements and assembly.

### 15/10/2026 — first public distribution0.4.2

- Published the original Tower local test through the existing Mod Browser
  repository. Installation checks remained distinct from multiplayer acceptance.

### 15/10/2026 — public network test0.5.0

- Added explicit network receiver transactions and a controlled Lobby guide.
- Later0.5.1–0.5.4 changes retain their original detailed entries above.

### 16/10/2026 — all-faction development begins

- Eight additional standard-town sets and painted artifact masters were
  prepared and reviewed. Existing Tower content remained the reference.
- Signature abilities and nine champions were designed. A reported network
  AI-evaluation crash was recorded; no universal fix was established.

### 17/10/2026 — local combined prototype and dev2–dev5

- Integrated nine faction champions, native portraits and commanders.
- Initial combined startup failed and the prior local version was restored.
- Subsequent local repairs addressed artifact configuration bounds, ERA input,
  artifact prose/tooltips and quest display. Dev5 was installed for local tests.
- These local candidates were not separate public Mod Browser releases.

### 17/10/2026 dev5 > dev6 — local candidate

- Added the relic battle-book entry and additional Necropolis life drain.

### 17/10/2026 dev6 > dev7 — local candidate

- Corrected native ERA command framing and expanded book/champion checks.

### 18/10/2026 dev7 > dev8 — local candidate

- Added an isolated relic icon page and readable low-mana entries.

### 18/10/2026 dev8 > dev9 — local candidate

- Revised faction loot exclusions, champion quest flow, relic page and
  component acquisition balance following player screenshots.

### 18/10/2026 dev9 > dev10 — local candidate

- Repaired component map identity, Inferno shield silhouette, pickup pictures
  and collection capacity.

### 18/10/2026 dev10 > dev11 — private audit candidate

- Audited equipment transactions and book lifecycle; equalized map layers1:1.
- Used actual maximum mana and preserved backpack inventory on rollback.

### 18/10/2026 dev11 > dev12 — public test resumes

- Added verified delivery recovery and reviewed release gates. Detailed public
  dev12 and later changes remain in the main changelog above.

All dates and local/public labels derive from preserved Git milestones and
release records. They are not additional gameplay or multiplayer acceptance.

### Publication date index for subsequent public dev builds

- 18/10/2026 dev11 > dev12
- 19/10/2026 dev12 > dev13
- 20/10/2026 dev13 > dev14
- 20/10/2026 dev14 > dev15
- 20/10/2026 dev15 > dev16

Dates are preserved release commit timestamps in Europe/Berlin. Later releases
add their dated transition at the top without deleting this history.
