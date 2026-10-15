# Updating through Heroes Launcher

Use the existing **Legacy of the Cloud Titans - TEST** entry. Close the game before updating, and keep the same installed version on both computers. Start a new map when a release requires one.

## Version display and repeated Update button

Launcher obtains catalog metadata from its server, but Install/Update downloads the current GitHub branch archive. These sources can temporarily disagree. On October 15, 2026, the catalog still reported 0.5.0-nettest-alpha while the downloaded files and installed mod.json contained 0.5.1-nettest-alpha.

When versions differ, the version cell displays the installed version above the catalog version, separated by an arrow. A narrow row may clip the lower text. The button checks for any version difference, including an older catalog version; it does not establish that the catalog version is newer.

After extraction, Launcher hides Update without reading the installed version again. Reopening Mod Browser runs the comparison again, so a stale catalog can make Update reappear after a successful installation.

The authoritative installed version is `Mods/Cloud Titans Legacy - Local Test/mod.json`, field `mod_version`. If it is already 0.5.1-nettest-alpha, repeated installation is unnecessary. The server's catalog refresh schedule has not been established; no fixed waiting time is promised.

## Publishing

Keep the repository, catalog entry and installation folder unchanged. Change the version together with each gameplay release and publish matching files. `info_version` is not used by this client's update comparison. Do not create duplicate catalog entries for releases.
