# Updating through Heroes Launcher

Use the existing Mod Browser entry **Legacy of the Cloud Titans - TEST**. Normal future releases use **Update**; uninstall/reinstall is not the normal update procedure.

Launcher reads `mod_version` from the catalog and compares it with `Mods/Cloud Titans Legacy - Local Test/mod.json`. A different version exposes Update. The same version has only Uninstall, as expected. The 0.5.0-nettest-alpha screenshot with no Update therefore shows the current version installed.

For publishers: keep the same repository, catalog entry and folder identity. Change source `version` and public `mod_version` together for each gameplay release, publish the matching payload and manifest, and allow the catalog metadata to refresh. `info_version` is not used by the installed client's update comparison. Do not create another catalog entry for each release.

For players: close the game before updating; both online players must use the same version. Do not update during an active multiplayer session. If the catalog temporarily shows stale metadata, reopen it later. The earlier uninstall/install workaround was for the initial stale catalog only.

Read-only verification of the downloaded Launcher client comparison function passed: 0.4.2 -> 0.5.0 exposes Update, 0.5.0 -> 0.5.0 does not, and 0.5.0 -> a simulated 0.5.1 exposes Update. The simulated 0.5.1 was not published. No active game installation was altered for this check. Actual clicking through a future Update remains to be verified in an isolated profile when a real gameplay release is ready.
