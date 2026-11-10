# Testing checklist

No tests have been completed yet.

## Compatibility record

- Game: Blade & Sorcery: Nomad
- Game version: TBD
- Quest device: TBD
- Mod build/version: Not built
- Test date: TBD

## Installation and loading

- [ ] Confirm current official Nomad mod installation workflow.
- [ ] Confirm required metadata and folder structure.
- [ ] Install on a test device.
- [ ] Confirm the game loads with the mod enabled.
- [ ] Confirm the game loads with the mod disabled/removed.

## Blood Drain

- [ ] Spell input activates only when intended.
- [ ] Valid NPC target is detected.
- [ ] Invalid or out-of-range target is handled safely.
- [ ] Liquid stream follows the hand smoothly.
- [ ] Forearm aura follows the arm smoothly.
- [ ] Releasing input removes the connecting stream.
- [ ] Aura fades and all effects clean up correctly.
- [ ] NPC interaction uses supported game behavior.

## Quest performance

- [ ] Stable frame rate during one effect.
- [ ] Stable frame rate with multiple effects.
- [ ] No excessive transparent overdraw.
- [ ] No persistent particle or object leaks.
- [ ] No errors after repeated casting.
- [ ] Test alongside common Nomad mods.

## Release readiness

- [ ] Tested on actual Quest hardware.
- [ ] Compatibility version documented.
- [ ] Known issues documented.
- [ ] mod.io description and screenshots prepared.
- [ ] Package verified before publishing.