# In-map Dungeon Architecture Design

## Intent
Retain the existing seven dungeon route layouts and biome artwork. Replace the disjointed off-map scenery with physical, visible landmarks in walkable rooms, connected architectural edges for corridors, and varied in-floor environmental storytelling. Use only actual game assets, no promotional/mockup image.

## Constraints
- Protect all original encounter rooms, entrances, ladders, chests, lever requirements, boss gates.
- No NPC or character passes through a landmark; solid landmarks must not disconnect any accessible route.
- Every biome has its own environment language and floor decorations; no generic crystals outside Crystal Hollow.
- Only change exploration rendering and collision; retain battles, saves, and towns.

## Considered Approaches
1. Place more stickers in void: cheapest, but disconnected (rejected).
2. Replace level backgrounds with screenshots: impressive stills, incorrect gameplay (rejected).
3. Anchor existing detailed props on actual floors plus per-tile connected structures/corridor edges; preserve collision/path connectivity (chosen).

## Acceptance
- At least 3 in-floor anchored landmarks per regular dungeon, with 7 distinct biome sets; no large void-mounted prop rendering.
- Visible connected corridor treatment for every biome and ground details on walkable floor.
- All pre-existing interactive tiles reachable, boss exits preserved, existing NPC and save behavior unchanged.
- Actual browser screenshot captures from revised game, no concept mockups.
