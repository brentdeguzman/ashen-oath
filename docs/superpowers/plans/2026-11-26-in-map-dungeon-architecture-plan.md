# In-map Dungeon Architecture Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Move biome structures into playable dungeon rooms and connect architecture to walkable tile layouts.

**Architecture:** Keep logical maps immutable. Place solid props only on verified non-critical interior floor tiles, test BFS connectivity and block occupied coordinates in walk validation. Tile-paint biome corridor edges below actors and landmarks.

**Tech Stack:** Browser HTML5 Canvas, JavaScript, Pillow/Playwright QA.

**Spec:** `docs/superpowers/specs/2026-11-26-in-map-dungeon-architecture-design.md`

## Global Constraints
- Preserve original map coordinate graph except for verified safe solid prop footprints.
- Do not rewrite bosses, village, skill logic, saves or functional exits.
- Provide actual renderer captures only.

## Review Focus
- Staircase/elevation transitions do not become inaccessible.
- A prop cannot block a secret or locked gate.
- A multi-floor return route remains walkable.
- No overlapping props obscure entrance.
- A reloaded save remains at a valid coordinate.

### Task 1: In-map structure placement
- [ ] Write and run failing static test asserting new renderer and collision entrypoints.
- [ ] Implement `v127DungeonAnchors(zone)` and `v127DungeonBlocks(zone)`, reserving functional tiles and flood-fill route connectivity.
- [ ] Draw anchored props at terrain scale and remove the old void-mounted render call.
- [ ] Run tests and browser placement check.

### Task 2: Connected architecture and floor detail
- [ ] Create biome-specific corridor styling and boundary trims in `v127DrawCorridorTiles`.
- [ ] Add walkable floor detail below the player and biome room features.
- [ ] Run browser screenshots across seven themes, visually inspect, adjust.

### Task 3: Regression and delivery
- [ ] Run all maps, stairs, gates and settlement paths in browser tests.
- [ ] Run JavaScript syntax, manifest, and ZIP integrity checks.
- [ ] Package full updated game, link actual screenshot and ZIP.
