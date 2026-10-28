# Validation for 0.6.0-batch-dev30

32 targeted background tests passed: 10 headless production x86 book/backpack
fixtures, 5 shipped popup/message-contract checks (including 2 isolated x86
emulations), 11 relic-book checks, 3 catalog checks and 3 Launcher release checks.
The popup regression fails against the dev29 handler and passes with CloseDialog.
Shipped CloseDialog ends the modal in the same call; the old synthetic Escape
leaves it running. Cached provider cells are destroyed before sorting/reopening.

Native x86 bridge rebuilt with source fingerprints. Candidate parser/resource/
function/archive gates, all 55 baseline snapshot hashes and the public manifest
passed. Complete artifact-record permutation and conflict protection are covered
by the existing headless sort fixture. The full suite was not repeated; 716 is
the previous recorded full-suite result from dev28 development, not a new run.

These checks do not execute the game renderer, a real ERA save/load or a Lobby
connection. No game was launched, controlled or updated. Actual first-click
response in the player's game and two-computer synchronization remain pending.
See CHANGELOG.md for separately established earlier native spot coverage.
