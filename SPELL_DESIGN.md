# Spell design

## Visual identity

- Theme: dark fantasy
- Main palette: deep crimson, dark red, near-black accents
- Material direction: glossy, flowing, liquid-like magical ribbons
- Motion: smooth streams, curling flow, subtle ripples and small stylized splashes
- Avoid: lightning-like bolts, noisy particle-only effects, excessive bloom, graphic gore

## Blood Drain — signature spell

### Intended input

Hold the spell input and point at a valid NPC.

### Intended sequence

1. Detect a valid target within the supported range.
2. Show a subtle casting cue.
3. Create a continuous-looking crimson magical stream between target and caster's palm.
4. Animate the stream toward the palm.
5. Build a swirling liquid-like aura around the caster's forearm while the input is held.
6. On release, remove the connecting stream and let the arm aura fade over a short configurable duration.
7. Clean up all spawned effects if the target becomes invalid or the spell is interrupted.

### NPC presentation

The intended fantasy presentation is a gradual loss of color toward a pale, desaturated appearance, followed by the game's ordinary defeat behavior when the spell completes. Keep the visual treatment stylized and non-graphic. Exact NPC appearance changes depend on what the current Nomad APIs support.

### Energy

The design may use an abstract stored-energy meter. Do not implement energy persistence until the supported mod framework and input APIs are confirmed.

## Additional spells

### Blood Orb
Cup the palm upward. Form a floating crimson sphere from stored magical energy. A later implementation may allow the orb to be launched.

### Blood Infusion
Grip a weapon and activate the spell. Apply a flowing crimson magical coating to the held weapon.

### Blood Barrier
Extend both hands forward. Form a defensive crimson magical barrier.

### Blood Tendrils
Spread the fingers outward. Create animated liquid-like magical extensions that follow hand movement.

## Gesture design caveat

The gestures above are design intentions, not verified input bindings. Implement only with controller/hand-tracking inputs officially supported by the current Nomad modding framework. Provide an accessible fallback input if gesture recognition is unavailable.