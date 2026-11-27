# Ashen Oath v1.3.2 progressive dungeon room overhaul

Goal: exactly 1/2/3/3/4/4/5 independently explorable map stages before each of seven guardian rooms in story/boss order. Original boss maps remain separate.

Stage chains:
* Forest Briarhorn: 2
* Crystal Sentinel: 10 -> 3; keep legacy map 11 as a migration-only area.
* Marsh Fen: 30 -> 31 -> 6
* Shrine Warden: 32 -> 33 -> 4
* Highland Gryphon: 34 -> 35 -> 36 -> 7
* Spire Sovereign: 15 -> 16 -> 37 -> 8
* Echo Keeper: 38 -> 39 -> 40 -> 17 -> 18

Each stage has one entrance, one gated exit (U, or J on final guardian threshold), one unique switch, meaningful chests and scenery, and no j/k shortcuts. Separate map IDs preserve independent puzzle and treasure state in saves. World entrances are remapped to the start stage; prior stage always available by entrance O. All added maps have 3-level 2.5D elevation and terrain atlas per stage; keep existing rendered assets, bosses, bestiary, save schema.

Test plan:
1. Browser run validates chains and world entry route, no shortcuts anywhere, and all stage art loaded.
2. Logical BFS for each stage checks all walkable cells reachable under height/stairs rules; switch/exit reachable.
3. Traverse each transition by stepping onto U; verify lever gate; E at lever; floor return via O; entering final J only after visiting all stages.
4. Existing forest and crystal unchanged except shortcut removal and Crystal's two-room route.
5. Inspect actual game canvas captures from each new biome in Chromium; test no runtime errors.
6. ZIP integrity, syntax, save-format compatibility and full artifact verification.
