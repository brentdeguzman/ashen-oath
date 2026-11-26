ASHEN OATH v1.2.0 — COMBAT ARTS & GUARDIAN BALANCE

New in v1.2.0: unique painted skill effects for all 18 hero skills. Legacy overlays
no longer stack. Normal enemies deal an extra 20% damage compared with v1.1.1.
All seven bosses have tiered HP from 500 to 2000 in 250-point steps, stronger attacks,
and tactical target focus. See UPDATE_v1_2_0.txt for details.

ASHEN OATH v1.1.1 — ENEMY VISUAL HOTFIX
==========================================

Corrects the new 70-monster dungeon bestiary visual presentation:
- Mirror enemy battle sprites horizontally to face the heroes on the right.
- Re-extract every monster from the larger original approved biome concept sheets,
  rather than the tight 70-unit overview with neighboring sprite fragments.
- Clean cut-out silhouettes, and preserve proper width/height without distortion.
- Rebuilt all 6 animation frames for each enemy: 4 idle, 1 attack, 1 hit.
- Specifically repaired the Frost Wolf, Fire Drake, Storm Drake, and similar wide creatures.
- No changes to enemies' battle statistics, behaviors, world-map rosters, loot,
  boss encounters, combat skills, inventory, merchants or save data.

PLAY: Extract ZIP and run PLAY_GAME_WINDOWS.bat.
SAVES: Existing v1.0.0 / v1.1.0 exported saves remain compatible.

--- PREVIOUS RELEASE NOTES ---
ASHEN OATH v1.1.0 — SEVEN DUNGEON BESTIARIES
==============================================

LATEST UPDATE (built on GitHub v1.0.0):
70 new biome-specific dungeon enemies (10 per biome), 70 named enemy skills,
six sprite frames per monster (4 animated idle, attack, hit), elemental
weaknesses and resistances, enemy status effects, dungeon loot and depth-based
encounter rarity. All original overworld enemies are preserved and remain
separate from dungeon encounter pools. See UPDATE_v1_1_0.txt.

PLAY: On Windows open PLAY_GAME_WINDOWS.bat, or open index.html directly.
SAVES: Import the previous exported save through the System menu.
The save format, dungeon geometry, bosses and equipment are unchanged.

--- PREVIOUS DEVELOPMENT RELEASE NOTES ---

ASHEN OATH v3.23 — SEVEN LIVING DUNGEONS
=======================================

This is the full offline HTML5 RPG, continuing directly from v3.22.3.
The entire dungeon rendering layer and biome scenery have been rebuilt around
seven boss identities. It is not a standalone demo or a change to the main world.

PLAY: Windows: double-click PLAY_GAME_WINDOWS.bat, or open index.html.
SAVES: Import your previously exported save from System -> Import Save File.
Existing party, inventory, defeated bosses, quest progress and treasure records
remain compatible. Saves in older dungeon layouts retain their coordinates
where possible; unsafe legacy positions are relocated by existing migration.

NEW IN v3.23
------------
BLACKROOT WILDS - forest rootways, ancient elderwood monuments, leafy mossy
  sanctuaries, winding living-grove clearings and Briarhorn's root chamber.
DUSKFEN MARSH - rotten causeways, fetid water and ruined swamp stone, deadwood
  sentinels, poison pools, mud islands and Fen Devourer's sinking pit.
CRYSTAL HOLLOW - three distinct mine-gallery routes with crystalline shafts,
  abandoned rails, prism formations and Crystal Sentinel's ritual crucible.
ASHEN SPIRE - three blackstone citadel floors with lava seams, forge courts,
  battlements, towers, ember gateways and the Ashen Sovereign's throne.
TRIAL OF ECHOES - two broken arcane-memory halls with violet glyph masonry,
  mirror arches, fractured cloisters and the Keeper's ritual chamber.
SUNKEN SHRINE - tidal temple stones, flood-channel textures, coral monuments,
  drowned cloisters and the Tidebound Warden's submerged altar.
STORMPEAK HIGHLANDS - snow-scoured cliff paths, watchtowers, sky bridges,
  pale rock, dangerous precipices and Stormclaw's exposed eyrie.

ALL SEVEN BOSSES - dedicated chamber architecture, larger overworld guardian
  portraits and a post-boss exit behind each sanctuary. The rear exit is sealed
  until the guardian falls, then returns the party to the outdoor world.

TREASURE - fully repainted 3D-style wood/brass chests with a glowing gem and
  seven different region palettes, keeping their existing rewards and records.

VISUALS - new high-detail, contiguous dungeon ground art; biome-specific
  chasms, cliff faces, setpieces and foreground scenery, with the old shared
  cartoon-like grass tickmarks and triangular filler decorations removed.

All dungeon topology changes are additive to the previously validated paths.
The game retains its existing turn-based battle system, party, side quests,
equipment, world map, switches, camps, shortcuts, and save system.

--- OLDER RELEASE NOTES ---


A full continuation of v3.21. All existing classes, equipment, town quests,
turn-based battles, world routes and save exports remain part of the game.

PHASE 1 — WILDS, MARSH & CRYSTAL
--------------------------------
* BLACKROOT WILDS: winding elevated elderwood and hollow-root passages, eerie
  canopy scenery, thorn hazards, side stashes and a root-ring boss sanctum.
* DUSKFEN MARSH: drifting islands and broken boardwalk-style routes, gas and
  bubbling mire, toxic stepping hazards and a dedicated acid-pit boss arena.
* CRYSTAL HOLLOW: three separate large floors with miners' galleries, crystal
  ledges, split paths, resonance tiles and a polished Prismatic Crucible.

PHASE 2 — SPIRE, ECHOES & SHRINE
--------------------------------
* ASHEN SPIRE: three linked levels featuring ruined fire halls, magma fissures,
  ember vents, dark stronghold textures and an Infernal Throne boss arena.
* TRIAL OF ECHOES: two large mystical floors, faintly floating sigils, memory
  glyphs, old rune halls and a circular Chamber of Lost Voices boss arena.
* SUNKEN SHRINE: a full tidal reliquary with worn pillars and current hazards.
  NEW: the Tidebound Warden now guards its own Drowned Altar encounter. Defeat
  the Warden, then approach the relic pedestal and press E to reclaim the shrine.
* STORMPEAK HIGHLANDS has also been rebuilt with its own cliff-and-skybridge
  approach and a dedicated Stormclaw Eyrie boss room.

PHASE 3 — VISUALS, TREASURE & PROGRESSION
----------------------------------------
* Five returning guardian artworks have new thematic halos / effects while
  Crystal Sentinel keeps its polished artwork; the Tidebound Warden has
  been fully redrawn as a detailed aquatic guardian to match the rest of the
  boss lineup. All seven chambers have unique arena markings.
* Every expedition floor is now larger (49–51 tiles wide x 35 tall), with
  crafted multi-tier routes and optional branches; 4–5 reachable chests per floor.
* Find a lever (a) and press E to unlock that floor's sealed door/gate.
* Reach the upper shortcut rune (k) to unlock travel back to its entrance (j).
  Press E near either shortcut rune after unlocking it to use it.
* Mid-route camps (R) allow resting and saving; hidden alcoves can be searched.
* Environmental special tiles now differ by biome, and trigger only once per
  tile per save: thorn damage, mire poison, ember vents, magical MP effects,
  tidal surges or mountain gusts.
* The Adventure Menu Map tab shows a local fog-of-war Explorer's Sketch when
  inside a dungeon; outside it shows the existing world map.
* Old dungeon save coordinates safely relocate to that level's new entrance.
  Existing heroes, gold, gear and beaten guardians remain saved.

PLAY / UPGRADE
--------------
1. Extract the ENTIRE ZIP before launching.
2. On Windows double-click PLAY_GAME_WINDOWS.bat; on other platforms open
   index.html in a modern desktop browser. No internet connection is needed.
3. If moving from a different folder or browser, export your save from the old
   version's System menu and import it via System > Import Save File in v3.22.
4. Use WASD / Arrow keys to move, E / Enter / Space to interact, and M for the
   Adventure Menu. A four-member party is chosen at the beginning.

TESTED
------
* Main JavaScript passes syntax validation.
* All 12 expedition floors and 7 guardian sanctums pass automated route checks
  for reachable entry, lever, gate, bosses and relic/treasure destinations.
* Actual graphical interaction in a browser was not available in the build
  environment; report any runtime problems with a save or screenshot.

------------------------------------------------------------
PREVIOUS RELEASE NOTES (v3.21 and earlier)
------------------------------------------------------------

ASHEN OATH v3.21 — LIVING DUNGEONS & CRYSTAL SENTINEL
=================================================

NEW IN v3.21 — LIVING DUNGEONS
---------------------------
- Twelve scrolling dungeon/guardian-approach floors now use terrain textures
  matched to their biomes: crystal caves, forests, tidal shrine, poisoned
  marshes, snowy highlands, royal ruins and the Trial of Echoes.
- Distinct abyss materials, cutaway cliff textures, animated glow effects,
  safe-to-walk ledge boundaries, and special scenery placed over void tiles.
- Three optional side alcoves / treasure detours on each non-crystal expedition.
- All SIX guardian-only chambers have individual colored ceremonial runes,
  altar plinths and local effects; no random encounters inside.
- Crystal Sentinel features a newly illustrated, alpha-transparent boss sprite
  in combat and visible on the dungeon map.
- Sunken Shrine is now a 39x27 scrolling dungeon. Its original relic and
  Dawnreaver reward are retained on the new altar at the end of the route.
- Compatible with exported saves from older versions; use System -> Import.
- Same turn-based combat, roles, skills, equipment, shops, and chapter unlocks.

HOW TO PLAY
-----------
1. Extract this whole ZIP to a permanent folder. Do not launch it from a
   compressed archive or WinRAR's temporary directory.
2. On Windows, double-click PLAY_GAME_WINDOWS.bat. Otherwise open index.html
   in a modern browser. Everything runs offline; no install or web access needed.
3. Select any four classes to start a new journey. The first selected hero is
   the visible walking character on the map.

PATHWAY FIXES IN v3.20.2
----------------------
- The overworld now follows a connected network of walkable tracks sampled from
  the ACTUAL illustrated landscape; hidden random tree / stone blocks from older
  versions no longer interrupt a visible dirt road.
- Real walking tests confirmed routes from the starting area to Blackroot Wilds,
  Crystal Hollow, Duskfen Marsh, and Trial of Echoes; the remaining world
  destinations were checked for connected paths as well.
- Crystal Hollow's mine entrance is at the foot of the cave (27,28), not on
  the waterfall ledge (26,25). The forest, marsh, and Trial entrances are
  likewise positioned on their visible roads.
- Water and sheer cave cliffs remain blocked to walkers. Raft access still
  controls deep water, and the stone bridge opens only after Crystal Sentinel,
  WITHOUT requiring a raft.
- Old save locations on the misplaced cave waterfall are relocated safely to
  the lower trail when loaded. Classes, equipment, chapter unlocks, NPCs,
  combat, boss chambers and +20% enemy damage are unchanged.

WHAT'S NEW IN v3.20
-------------------
- The world map uses original, illustrated 1800x1200 terrain artwork in the
  live, scrolling exploration renderer, with painted rivers, forests,
  coastlines, mountain ranges and paths. The World Map menu uses this art too.
- Crystal Hollow is now a 3-stage expedition. The two gallery floors and the
  final ascent are 51x35 tiles with different winding routes, three heights,
  additional side passages, larger treasure detours, glowing crystals and
  a luminous underground river below the cliffs.
- Crystal Sentinel is still alone in the Prismatic Crucible, now with a
  glowing rune-dais and more prominent map sprite. No random encounters
  occur inside guardian-only chambers. Solo bosses remain centered in battle.
- Briarwatch keeps its hand-illustrated, navigable architecture and safe-zone
  behavior; drifting leaves and wandering birds make the town livelier.
- Save file export/import has been added to System for carrying saved journeys
  between future versions or browser installations. Saving a new checkpoint
  still requires a town, inn or safe wilderness campsite.
- All existing classes, gear, boss rewards, quests, regional encounters,
  combat and skill visuals remain included.

CRYSTAL HOLLOW GUIDE
--------------------
Restore the Bark Seal by defeating Briarhorn Ancient in Blackroot Wilds.
This unlocks Crystal Hollow. Then:
1. Enter Crystal Hollow on the world map (27,28).
2. Follow stone trails across the first floor; climb the wooden ladders and
   find the rune lever. Press E beside it. Locate the now-unsealed exit.
3. Repeat on the second floor, taking optional treasure passages.
4. On the third floor, follow the rising ledges to the guardian arch.
5. Enter the Prismatic Crucible, a separate chamber holding Crystal Sentinel.
   Defeat the guardian to restore the eastern bridge.
Open M -> Journal or Map if you need story and route guidance.

CONTROLS
--------
WASD or Arrow Keys : Move
E / Enter / Space : Talk, search, use levers and doorways
M / Escape : Main menu (Status, Equipment, Skills, Inventory, Journal, Map, System)
I : Equipment / inventory
Save : Only in safe areas, inn or campsite
System > Export Save File : Create a portable JSON backup (requires an
    existing save made in a safe area)
System > Import Save File : Restore a previously exported journey

NOTE ON SAVES
-------------
Browser localStorage is isolated by website/path/browser and may not follow
new extracted game folders automatically. For future upgrades, export a save
file from your previous playable version first, then import it into the new
version. Versions before v3.20 may not offer an export button. Existing saves
loaded in the same storage origin remain format-compatible.

All scenery, character and item graphics used in this game are original
project assets; nothing is copied from Final Fantasy artwork or map files.


HOTFIX SUMMARY
--------------
* Replaced the placeholder-like Tidebound Warden portrait with a fully rendered
  aquatic guardian illustration that matches the other boss artworks.
* Added Tidebound Warden-specific encounter and victory flavor text.
* No balance or map progression changes were made in this hotfix.


V3.22.2 GUARDIAN VISUAL PASS
----------------------------
* Briarhorn Ancient: completely new, detailed treant illustration.
* Fen Devourer, Crystal Sentinel, Stormclaw Gryphon, Ashen Sovereign and
  Keeper of Echoes: refined existing art, additional themed ceremonial
  sigils and detailed ambient effects.
* All seven bosses now have unique animated encounter auras, background
  motes and personalized guardian titles during battle.
* Tidebound Warden artwork from v3.22.1 is preserved.
* No dungeon, loot, statistics or save structure changes.


v3.23.1 INTERACTABLE REFRESH
----------------------------
Dungeon interactables were resized and restyled to better fit the new dungeon art, and rear boss exits can now be used reliably after victory.


v3.23.2 INTERACTABLE FIXES
--------------------------
Stairs, campfires, chests, sanctuary exits, and the forest entrance marker were revised again for better fit and readability. Rear boss exits now have more reliable activation.


v3.24 INTERACTABLE ART AND EXIT FIXES
--------------------------------------
For each dungeon biome, updated chests, campfires, stairs, levers, altars, boss entrances and unlockable rear exits are now drawn from matching fantasy art sprites in-game. Normal dungeon entrances now function as exits on all floors. See UPDATE_v3_24.txt.


v3.24.2 OVERWORLD ENTRANCE RESTORATION
--------------------------------------
Restored the full overworld forest entrance artwork after a regression introduced a tiny fallback marker. Staircase fixes remain in place.


v3.26: MERCHANT & INVENTORY
- Visit Torren at Ironwood Workshop in Briarwatch, interact with him, choose Buy or Sell.
- Selling equipment returns 50% of its listed price (rounded down, minimum 1 Gold).
- Tonics sell for 6 Gold each. Sell one or all at once.
- To discard equipment or tonics, open the Menu > Inventory tab, select an item and choose Drop.
- Selling/dropping equipped items automatically unequips them after confirmation.
- Unique rewards can be sold/dropped with extra warning, so be careful.
- Dropped items are permanently discarded, not placed on the ground.


v1.2.2: Illustrated skill effects reduced another 15% and set to 50% opacity. Gameplay is unchanged.
