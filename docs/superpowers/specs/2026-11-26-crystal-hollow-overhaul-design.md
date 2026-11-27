# Crystal Hollow — Cave Architecture Overhaul Design

**Intent:** Rebuild only Crystal Hollow's three traversable floors so they look like a coherent navigable classic RPG cave instead of irregular photo-textured terrace plates with floating/out-of-bounds decorations. The linked Final Fantasy II Snow Cavern serves as a guide for readability and connected rooms, NOT a source of copied tiles, maps or artwork.

**Scope:** The three map IDs 10 (Miners' Galleries), 11 (Facet Labyrinth), and 3 (Sentinel Ascent). Keep the Crystal Sentinel boss room, the world, the seven other biomes, combat and saves unchanged.

**Visual rules:** Continuous 2D painted rock floors, identifiable tunnel joins and natural chambers, dense connected crystal growth marking every boundary, limited architecture grounded on the room floor, zone-specific atmosphere (timbers/railwork; faceted caverns; royal ascent). No prop collections randomly placed in void. Real renderer screenshots/video only.

**Game rules:** Preserve exact special interaction tiles from v1.2.7 (entrances, exit, stairs, chests, rest fire, switches, sealed gates, shortcuts). Every interactable and main route remains reachable through legal elevation transitions; keep collision aligned with painted geometry. No external asset dependencies.

**Tradeoffs:** Use a full-resolution, original procedural pixel-painted terrain atlas per floor with the logical collision map retained separately. This makes continuous borders and room-to-corridor joins easier to control than dozens of independent sprites. It is not replacing the full gameplay screen with a picture: characters, combat, collisions, saves, quest triggers and UI remain live. Other seven biomes retain v1.2.7.

**Testing:** Verify complete route and key tile reachability for every floor, screenshot eight locations from actual browser renderer, walk a real path across map 10, test boss route entrance/upstairs, test no page errors/no missing images, ZIP integrity, and source JS syntax.
