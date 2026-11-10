# Minecraft AR — Roomcraft

A browser-based mixed-reality voxel sandbox prototype for Meta Quest.

## Run it

1. Publish the `minecraft-ar-prototype` branch from **Settings → Pages** (root folder).
2. Open `https://lightluxgaming-pixel.github.io/Vr/minecraft-ar.html` in Meta Quest Browser.
3. Allow immersive AR, hand tracking, and room/plane access.
4. Complete Space Setup if the headset asks. If no room planes arrive, the page asks the headset to start room capture when supported.
5. Point with an index finger and pinch to interact.

## Current prototype

- Transparent immersive-AR passthrough session.
- Requests WebXR hand tracking and plane detection.
- Reads detected room planes and draws their outlines.
- Requests Meta room capture through `XRSession.initiateRoomCapture()` when no planes are detected.
- Room-sized starter island with grass, dirt, stone, an oak tree, and a seven-block hotbar.
- BUILD mode places the selected block on a targeted block face or floor grid.
- MINE mode breaks targeted blocks.
- Hand pinch gestures select hotbar blocks and interact with the world.

## Controls

- Point with your index finger.
- Pinch thumb and index finger to interact.
- Pinch a hotbar cube to select its block type.
- Pinch BUILD or MINE to switch modes.
- In BUILD mode, pinch a block face to place an adjacent block.
- In MINE mode, pinch a block to break it.

## Important limitations

This is the first playable foundation, not a complete Minecraft replacement yet. It currently has a starter island and basic voxel editing; survival, crafting, mobs, world saving, multiplayer, full terrain generation, and robust collision/occlusion are not implemented yet. Room-plane detection and hand tracking must be tested on the target headset/browser. The page uses Three.js from jsDelivr and requires an internet connection.

The project lives on its own branch, `minecraft-ar-prototype`. The existing `main` branch and other prototype branch are not modified by this work.
