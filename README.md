# BLOODBOUND

**A dark-fantasy magic mod concept for Blade & Sorcery: Nomad**

BLOODBOUND is a planned gesture-based magic expansion built around supernatural crimson liquid effects. The first milestone is a polished Blood Drain prototype with a hand-following liquid stream and a temporary swirling forearm aura.

> **Development status:** Design and repository setup. This repository does not yet contain a working, installable game mod. No gameplay features have been tested in Nomad.

## Planned spells

- **Blood Drain** — hold the spell input and point at a valid NPC; a stylized crimson liquid effect connects the target to the caster's hand. The energy gathers into a temporary swirling forearm aura.
- **Blood Orb** — form stored energy into a floating orb.
- **Blood Infusion** — coat a held weapon in a crimson magical effect.
- **Blood Barrier** — form a defensive magical barrier.
- **Blood Tendrils** — create animated liquid-like magical extensions.

## Target platform

- Game: Blade & Sorcery: Nomad
- Platform: Meta Quest
- Target game version: latest version at time of implementation; exact version must be recorded during testing.

## Important technical note

Nomad mod support and available APIs differ from the PCVR version. Before implementation, verify the current Nomad SDK/modding workflow, supported scripting or asset formats, and game-version compatibility against current official documentation. Do not assume that Unity Editor, PCVR scripts, VFX Graph, or arbitrary JSON files can run directly on Quest.

## Repository map

- `DEVELOPMENT.md` — setup and implementation plan
- `SPELL_DESIGN.md` — spell behavior and visual direction
- `TESTING.md` — compatibility and performance checklist
- `manifest/` — reserved for verified mod metadata once the correct format is confirmed
- `Assets/` — reserved for compatible, optimized assets

## Contribution and safety

All effects are intended to be stylized fantasy magic, not realistic injury simulation. Do not add copyrighted assets without permission.