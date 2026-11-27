# Ashen Oath v1.2.5: World Revitalization

**Intent:** The user's actual v1.2.4 game must show a lively Emberfield Meadows village, a visually distinct Glimmer Rest and Lumin Coast waystation, and more memorable, biome-specific scenery throughout the seven existing dungeons. This must appear in real gameplay, not a mocked-up screenshot.

**Goals:** Preserve existing game save keys and important route/interactable coordinates; add separate village/cart/stall/building art, ambient details, and named NPCs with dialogue and caravan trade; add coherent ornamental sets across forest, marsh, crystal, spire, echo, shrine, and highland dungeons with subtle animation and no terrain obstruction; provide actual tested screenshots and complete ZIP.

**Non-goals:** No main quest rewriting, no player/boss combat balancing, no changes to boss/map floor progression or existing dungeon interactables; do not substitute a static screenshot for playable graphics.

**Design choices:** Implement as new isolated scene and ambient layers in the existing canvas renderer. Load transparent WebP art and composite with existing live terrain. Fixed prop anchors and NPC IDs avoid affecting save compatibility. Protect routes and interactable coordinates. Dungeon micro-props are deterministic, seeded, and decorative; larger features are drawn on existing inaccessible cliff/abyss regions or on low-traffic floor edges. Reuse existing biome art only as ingredients for distinct new ornamental variants, not as the sole new scenery.

**Approaches considered:** (1) replace the whole map with a static screenshot (rejected, breaks interaction and misrepresents implementation); (2) extensively rewrite world maps (rejected, risks progress and routes); (3) new layered scenery and NPCs on unchanged maps (chosen for visual improvement without route regressions).

**Constraints:** Fully offline; preserve core renderer, story and save structure; sprite art scaled to 480x360 logical canvas; all new images carry transparent alpha. Avoid accidental duplicated rendering of campfires, chests, doors, staircases.
