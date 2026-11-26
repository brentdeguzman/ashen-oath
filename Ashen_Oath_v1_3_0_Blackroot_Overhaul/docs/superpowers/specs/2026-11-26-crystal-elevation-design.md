# Crystal Hollow — visible elevation design

**Intent:** Update Crystal Hollow first, keeping all three v1.2.8 layouts and all game content but visually making actual height differences legible. Each existing 0→1 / 1→2 height boundary should have distinct high floor, continuous stone edge, visible face/shadow against the lower floor, and physically integrated stairs at its authored two-tile `L` transitions. Crystal-lined impassable walls remain on void cells. Preserve all movement, transitions, treasures, exits, saves and all other dungeon art.

**Approaches:** (a) add free-standing stairs and rock props (rejected: causes old floating/flat look), (b) bake coherent cliff-face and stair relief into the 1530×1050 pixel terrain atlas while retaining 30px collision correspondence (chosen: deterministic and faithful), (c) full 3D or per-depth sprite lift (rejected: disproportionate and risks breaking camera/collision).

**Constraints:** Terrain is top-down and the 30px tile coordinate system cannot shift; a pronounced 2.5D vertical wall face and shaded upper border will communicate elevation without physically moving sprite coordinates. Must show actual browser game captures, not generated mockups. Test all six transition pairs (two per floor) for correct stair artwork and existing playability.
