# Minecraft AR — Roomcraft

A room-scale mixed-reality voxel survival sandbox prototype for Meta Quest Browser.

## Run it on Quest

1. Publish the `minecraft-ar-prototype` branch from **Settings → Pages** (root folder).
2. Open `https://lightluxgaming-pixel.github.io/Vr/minecraft-ar.html` in Meta Quest Browser.
3. Allow immersive AR, hand tracking, and room/plane access.
4. Complete Space Setup if prompted. If no room planes arrive, the page asks the headset to start room capture when supported.
5. Point with your index finger and pinch to interact. Walk around the small island physically.

## Current playable systems

- Transparent immersive-AR passthrough with WebXR `immersive-ar`.
- Requests `local-floor`, `hand-tracking`, and `plane-detection`; room plane outlines appear when supplied by Quest.
- Quest hand aiming uses the tracked index fingertip and distal finger joint to form a direct pointing ray, with the runtime target ray as fallback.
- Pinch selection uses Meta's regular hand-pinch Gamepad button, with joint-distance fallback when the runtime does not expose that button.
- Procedurally shaped starter biome with grass, dirt, stone, sand, coal/iron ore pockets, trees, leaves, and a small water feature.
- BUILD mode places selected blocks and consumes that block from the starter inventory.
- MINE mode mines blocks and adds the mined resource to inventory. Stone and ore need a crafted pickaxe.
- Floating hotbar supports block selection, BUILD/MINE, HAND/PICK tool selection, and CRAFT.
- Basic recipes: planks, bricks, glass, stone pickaxe, and logs.
- Survival loop: health, food, day/night cycle, respawning, and hostile slimes that appear at night.
- HUD reports room surfaces, tracked hands, block count, health/food, selected item count, and in-game time.

## Controls

- Point with your index finger; pinch thumb and index finger to activate.
- Select a block in the floating hotbar.
- BUILD: pinch a block face to place an adjacent block (consumes inventory).
- MINE: pinch a block to mine it (hard blocks require a pickaxe).
- CRAFT: crafts the first recipe for which you have enough materials.
- Walk around the island in your real room; keep a clear physical play area.

## Important limitations

This is a much larger playable prototype, not yet a complete Minecraft replacement. It does not yet include full infinite chunk streaming, caves, a complete recipe/inventory screen, reliable persistent world saving, multiplayer, farming, animals, sound/music, full player collision, or robust real-world occlusion. Slime combat and survival balancing are still prototype-level. The world is intentionally kept compact for Quest browser performance.

Hand tracking, room capture, and frame rate must be tested on the actual headset/browser. The assistant can syntax-check the source but cannot physically validate Quest tracking from here. The page loads Three.js from jsDelivr and requires internet access.

The work is isolated on `minecraft-ar-prototype`; `main` and the existing other prototype branch are untouched.
