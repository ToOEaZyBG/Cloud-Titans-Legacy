# Validation for 0.6.0-batch-dev38

29 targeted offline tests pass: 19 map/resource/generation checks, four global frame namespace checks, three catalog checks and three Launcher release checks. Resource verification additionally checks all90 parts, their loose/packed DEF/MSK/MSG parity, native compression3 shadow runs, nonempty shadow drawing masks and unchanged painted subject pixels/palettes. The old empty shadow mask is explicitly rejected. Candidate ERM/parser/config checks and the55-file baseline pass.

The native plugin and inventory archive are byte-identical to dev37. The terrain comparison board is an offline approximation, not a native renderer test. Actual in-game map appearance, battle/save/load, sustained AI/fullscreen and two-computer acceptance remain pending. This release does not modify the third-party Warlord's Banner.
