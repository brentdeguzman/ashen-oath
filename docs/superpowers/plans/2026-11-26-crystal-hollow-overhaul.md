# Crystal Hollow Overhaul Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Three fully remade, connected Crystal Hollow levels with legible rock-and-crystal boundaries and proven real gameplay screenshots/video.

**Architecture:** Original 51×35 authored tile geometry is serialized as an inlined JS constant. Painted terrain sheets corresponding to that geometry are rendered in the existing scrolling canvas as a background layer; interactive actors and gameplay state remain intact. All modifications are scoped to zone IDs 10, 11, 3.

**Tech Stack:** Existing HTML5/JS RPG, Pillow, Python Playwright/Chromium, ffmpeg.

**Spec:** `docs/superpowers/specs/2026-11-26-crystal-hollow-overhaul-design.md`

## Global Constraints

- No artificial mockups; visuals come from browser snapshots of the actual modified game.
- Reuse old special tiles and coordinates; preserve non-crystal content.
- Crystal edge walls must be visible, continuous, and impassable.

## Review Focus

- Ladder elevation crossing passable in both directions: browser integration check.
- Gate/lever/treasure reachable from floor entrance under gameplay movement restrictions: BFS.
- No full-screen decorative overlay conceals UI/player: browser screenshots.
- No regression outside Crystal: compare names/room counts and boss gate tests.
- No broken media in offline extraction: ZIP integrity and routed asset coverage.

### Task 1: Authored map geometry and regression test
**Files:** Create `/mnt/data/v128_create_crystal.py`, `/mnt/data/v128_test_crystal.py`, output `crystal_overhaul/map_layout.json`.
- [ ] Write test asserting IDs 10,11,3, specials, reachable entrance→exit and several chamber links.
- [ ] Run test RED on baseline old layout where v128 geometry does not exist.
- [ ] Create connected caves from hand-selected room graph and tier transition coordinates.
- [ ] Run test GREEN and inspect map ASCII.

### Task 2: Original connected terrain art and renderer integration
**Files:** Create `worldart/crystal_overhaul/*_terrain.webp`; modify `index.html` in isolated copy.
- [ ] Write test asserting atlas existence, matching 51×35 tile layout, render hook, no old void crystals.
- [ ] Run test RED.
- [ ] Paint dense bordering crystals and walkable cave floors, distinct art on each level.
- [ ] Integrate terrain images into real scrolling canvas and suppress obsolete terrain decorations only for these maps.
- [ ] Run test GREEN and JavaScript syntax check.

### Task 3: Gameplay browser captures and package
**Files:** Create `/mnt/data/v128_browser_test.py`, PNG captures, MP4 walkthrough, ZIP.
- [ ] Execute real gameplay and verify 3 routes/stair access/key assets; capture screenshots and traversal frames.
- [ ] Inspect screenshots; correct edge readability and player visibility.
- [ ] Run tests, Node syntax, ZIP integrity; package full RPG.
