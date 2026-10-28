# Validation for0.6.0-batch-dev34

15targeted tests pass:9authored ERM map/replication/pickup/terrain/access tests,
3catalog tests and3Launcher release tests. Exact180coordinates, two copies of
each of90parts,90/90layers, original external-monster proximity at every selected
site and identical sender/receiver native object-mutation order are verified.
Surface-only generation, old third-copy packet181 rejection, no-monster cells,
blocked terrain, AI/full-bag pickup refusal and unchanged level reward script
are covered. These use fake native map/transport bindings, not a native game.

393of398runtime files are byte-identical to33, including all images, configs,
native plugins, rewards, equipment and champions. Five map-related scripts change.
The prior776test/dev32 evidence applies to retained components with its original
limitations; the full suite was not repeated. Current candidate parser/resource/
arity/fingerprint gates and release450-file hashes pass. No new native combat,
real save/load or two-computer acceptance is claimed. No game/UI/install changes.

The retained external guard rule checks for a native map monster within3x3.
Ordinary game movement, flight, teleport and guarding rules remain unchanged;
this is not an embedded army or an unconditional scripted battle on pickup.
