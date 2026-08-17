- Update Veil to fix an issue where sub-levels weren't directionally shaded when Iris was installed 
- Allow UUIDs to be used to target sub-levels in commands
- Removed LittleTiles as a marked incompatibility
- Add a `/sable forceload query` command
- Fix Create Mechanical Rollers not working when Sable is installed
- Update some mixins for small optimizations

- Fix empty cached sub-level storage and region files not getting discarded from the cache on save
- Add a server config option for pruning sub-level storage files. This is experimental, and there is a chance of data loss. Please backup regularly if testing this.

- Fix a crash where a broken log pipe would cause Sable Rapier to panic. This was most commonly experienced by launching the game through Modrinth/CurseForge and closing the launcher before entering a world.
- Fix a crash with empty Create contraptions
- Fix a crash with block properties and some modded blocks
- Prevent lightning in sub-level plots
