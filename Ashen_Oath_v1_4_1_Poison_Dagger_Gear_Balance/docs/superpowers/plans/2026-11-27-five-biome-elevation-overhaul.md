# Five remaining dungeon biome overhaul

Source: browser-playable Ashen Oath v1.3.0a. Preserve Crystal Hollow (maps 10,11,3), Blackroot (map 2,23), combat, saves, and the story state.

## Geometry
Rebuild maps 6,7,4,15,16,8,17,18 as distinct interconnected halls, marsh islands, ruins, cliff routes, and branching rooms. Preserve entrance [2,9], boss or upper-floor portals, puzzle lever, locked door, camp, treasure and shortcut. Each exploration map includes two elevation connections, real 2-tile carved stairs. Keep all traversable goals reachable with elevation and puzzle rules. New event tile symbols continue to work with existing handlers.

## Guardian rooms
Provide biome-specific atlas artwork and preserve original boss encounter at [17,10], entrance [2,11], exit [25,11], relic and Q gate rules. No invisible blocking props.

## Visuals
Create a complete terrain atlas per changed map, based on existing art textures. Paint walkable pathways, biome-specific impassable outer borders, clifffaces, two level changes, shadowed vertical walls, and integrated stairs. Do not render legacy generic cliff/landmark/stair layers over these maps. Keep v1.2.8/9 Crystal floor atlas and v1.3.0a Blackroot untouched.

## Verification
First fail structural tests without a geometry file. Verify 13 maps, gate and floor links, JavaScript syntax, browser screenshots and no missing new atlas. Deliver ZIP and actual screenshot contact sheet. If browser limitations prevent evidence, disclose rather than invent.
