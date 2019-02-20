# Homeworld: DoK - More Maps v1.1 Changelog
- Added `FFA - Prime Anomaly [2,6]` (a 2, 3, 4, 5 and 6 player FFA map)
- Replaced `Salvage Facility [2]` with `Salvage Facility [2,4]` by HottestManEver
- Replaced `Cape Wrath [2]` with `Cape Wrath [2,4]` by HottestManEver
  (Many thanks to HottestManEver for his maps and help!)
- Added wrecks (wrap the resources you want to spawn in `<wreck> </wreck>` and specify an x, y and angle)
- Added support for non-square rectangular map bounds
- Removed `patch.json` from multiplayer to reduce chances for desyncs
- Nerfed Fathership faction (still godmode faction but it won't be made into anything resembling Soban or Khaaneph, don't want to step on BBI's payed DLC)
- Added ability to have multiple layouts per layout file
- Added ability to give different layouts depending on number of players (the brackets after a map name indicate the least and most allowed players)
- Added ability to change which layout is presented depending on the gamemode and map to allow for map packs
- All new maps have been updated to adapt to the number of players
  (Many thanks to FrostyTeeth for help with this!)
- Fixed artifact UI (a max of 4 artifacts may show in the UI)
- Fixed black background when loading into a new map for the second time
- Packed extra replay files into one file (instead of sharing 3 files just share the `.dokreplay` and `.dokreplayx` files)
- Overhauled `Prime Anomaly [2,6]` to make it less like Khar-Toba (for old anomaly do `/l anomaly-old`)
- `blockallheights` attribute on `<blocker/>` will default to whatever `blocklof` is
- Spawn points can have camera angle modified (use the `camera="<angle>"` attribute in `<spawn/>`)
- None faction removed but replaced with a layout specific option to despawn all starting units (use the `fleet="false"` attribute in `<spawn/>`)
- Mission 6 from the campaign has been fixed
- Updated Subsystem to 0.5.0
- With the new tools it is now possible to recreate the existing maps (do `/l gt-alt` to see an alternate version of Gaalsien Territories)
