# Crystal Hollow Elevation Implementation Plan

> **For agentic workers:** Implement this plan with superpowers:executing-plans and test-driven development.

**Goal:** Give the six existing height transitions of Crystal Hollow visible, integrated cliff walls and stairs without changing dungeon collision geometry.

**Architecture:** A Python/Pillow deterministic postprocess paints tier-boundary risers, parapet trim, cast shadows, and stairs into the existing three cave terrain atlases. The game suppresses its old flat staircase sprite only for the three remodeled maps, retaining the original `L` collision semantics and every other biome's render path.

**Tech Stack:** Python 3, Pillow, HTML5 canvas, JavaScript, Playwright Chromium.

**Spec:** `docs/superpowers/specs/2026-11-26-crystal-elevation-design.md`

## Tasks
- [ ] Write and run a failing test that requires 2 `L` pairs per map and integrated relief generated for each pair.
- [ ] Implement terrain atlas postprocessing for all six transitions and tier boundaries, preserving map geometry.
- [ ] Patch the HTML5 renderer to omit duplicate staircase sprites for the remodeled Crystal Hollow floors only.
- [ ] Verify all six stair pairs via in-game movement; capture actual same-camera before/after screenshots and a short real-game traversal.
- [ ] Run map, boss-exit, JS syntax, asset and archive integrity checks; package the complete v1.2.9 game.

## Review Focus
- [ ] `L` pairs on both vertical and horizontal axes are rendered without reversed ascents.
- [ ] No unrelated dungeon assets or save schema changes.
- [ ] All existing crystal symbols, movement and links still work.
- [ ] Terrain relief does not erase interactable icons or cover a required passage.
- [ ] Browser screenshots show height relief at normal gameplay scale.
