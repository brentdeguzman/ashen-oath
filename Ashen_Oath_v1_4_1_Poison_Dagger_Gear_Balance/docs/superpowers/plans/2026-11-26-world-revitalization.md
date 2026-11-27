# World Revitalization Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Ship the fully playable Ashen Oath v1.2.5 featuring villages and distinct, lively dungeon scenery.

**Architecture:** Static, transparent artwork under `worldart/v125_village` and optional biome ornaments; render with independent canvas functions using existing camera/tile projections. Register new ambient NPcs in `TOWN_NPCS`, preserve original map routes, and keep walkability unchanged except decorative NPC occupancy.

**Tech Stack:** JS Canvas 2D in existing index.html, PNG/WebP art via Pillow, Python Playwright browser tests, zip packaging.

**Spec:** `docs/superpowers/specs/2026-11-26-world-revitalization-design.md`

## Global Constraints
- Existing v1.2.4 battle code and quest state intact.
- Do not remove any route or change dungeon collision geometry.
- Only playable, source-level updates count as game modifications.

## Tasks

### Task 1. Add regression coverage and real village props
- [ ] Write failing assertions for v1.2.5 anchors, NPC hooks, biome scene function, and protected routes.
- [ ] Run tests, confirm expected failure.
- [ ] Slice transparent original village prop sheet; add stand-alone WebP assets.
- [ ] Implement Emberfield village layer and additional rest-stop/coast props.
- [ ] Test and capture actual 480x360 canvas with route-safe play.

### Task 2. Add lively region NPC behavior
- [ ] Write failing tests for settlement NPC interaction and no random encounters in safe meadows.
- [ ] Implement NPC registration, wandering, collision, E dialogue, caravan trade.
- [ ] Test NPC dialogue, caravan trade, existing Briarwatch interactions and save compatibility.

### Task 3. Seven biome decor layers
- [ ] Write failing tests for biome-specific scenic motifs on all dungeon parents and floor/sanctums.
- [ ] Create original deterministic decorative canvas compositions and biome art variants.
- [ ] Integrate with existing terraced renderer, avoiding paths/actors.
- [ ] Capture screenshots for every biome, verify stair/exit routes remain traversable.

### Task 4. Package, verify, report
- [ ] Execute JS syntax and full browser smoke/route checks.
- [ ] Generate real in-game comparison and biome gallery; add release notes.
- [ ] Zip, verify archive and output sizes.
