# Homeworld: DoK - More Maps v0.15 Changelog
- Added Khalash Wreck 1v1 by Begil and Torin Crater 3v3 by SSSS! Many thanks to Begil for his awesome maps
- Updated Subsystem to v0.4.0 (Note: delete `patch.json`, the way to use patches is to now use the /patch command)
  (`patch.json` still works but the /patch command overrides it)
- Custom layouts and custom patches are now compatible with replays even if you change patch.json
  (To share replays you must give 3 files for now, `<replayname>.dokreplay`, `<replayname>.dokreplay.json` and `<replayname>.dokreplay.dokmap`)
- Improved the installer to give better error checking thanks to Katsushiro!
- Custom layouts can be applied to original maps using the `/layout` command
- `/layout <id>` loads a custom layout from pastebin `<id>` is the end of a pastebin URL (eg https://pastebin.com/Jkyr8upc -> Jkyr8upc)
- `/layout-clear` clears any custom layouts
