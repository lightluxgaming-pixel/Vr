# ASCENSION — Become a God

An experimental, browser-based WebXR isometric-training game for Meta Quest headsets.

## Play it

1. Open this repository's **Settings → Pages**.
2. Set the publishing source to the `there-is-no-game-vr-prototype` branch and the `/ (root)` folder, then save.
3. After GitHub Pages finishes publishing, open:
   `https://lightluxgaming-pixel.github.io/Vr/ascension.html`
4. Open that HTTPS page in Meta Quest Browser, allow immersive VR, and select **Enter the Temple**.
5. Point either controller at one of the three training-path panels and press Trigger.

If GitHub Pages is configured to publish a different branch or folder, use the matching published URL instead. The page imports Three.js from jsDelivr, so an internet connection is required.

## Current features

- Immersive WebXR scene with controller rays, hand-shaped controller models, smooth stick locomotion, and a head-locked in-VR HUD.
- Three selectable paths: Foundation, Champion Path, and Sanctuary.
- Three distinct realm palettes and a procedural temple with a guardian statue, floating relics, pillars, particles, and a glowing altar.
- Timed isometric holds, rest intervals, exercise cues, and session completion.
- Local profile saved in the browser: XP, rank, completed sessions, streak, recent history, and achievements.
- Ten progression ranks with evolving visual effects.

## Controls

- Left thumbstick: move.
- Right thumbstick: smooth turn.
- Point a controller at a training panel and press Trigger to select.
- Trigger starts a ready hold or advances after the recovery period.

## Training and safety

ASCENSION is a timer and motivation tool. It does not measure force, validate exercise technique, or know whether a movement is appropriate for a player. Use gentle-to-moderate effort, breathe continuously, choose the easiest comfortable variation, and stop if pain, dizziness, numbness, or unusual discomfort occurs. The timer durations are intentionally short; do not treat XP, streaks, or rank as a reason to train through symptoms or skip recovery. Players should use exercises appropriate for their age, health, and experience, and seek qualified guidance when unsure.

Progress is stored in localStorage on the current browser/device. It does not sync between headsets or browsers. Clearing site data removes that local save.

## Development status

This is an early playable prototype. It has been syntax-checked, but real headset performance, controller mapping, comfort, and exercise usability still need to be tested on the target Quest hardware. The `main` branch is not changed by this prototype.
