<div align="center">

# 🩸 BLOODBOUND

### THE FORBIDDEN ART OF BLOOD

*A dark-fantasy, gesture-driven magic concept for* **Blade & Sorcery: Nomad**

**Crimson flows. Shadows answer. Magic obeys.**

[Project](#-the-project) · [Spellbook](#-the-spellbook) · [Roadmap](#-development-status) · [Documentation](#-project-documents)

</div>

---

> [!IMPORTANT]
> **Early development — documentation and design foundation only.** This repository does not yet contain a playable, installable, or Quest-tested mod. Spell descriptions below are design goals, not implemented features.

## 🕯️ The project

BLOODBOUND is planned as a dark-fantasy magic expansion built around **smooth, liquid-like crimson energy** and physical spell gestures.

The signature experience is **Blood Drain**: hold the spell input and point toward a valid NPC. A supernatural crimson stream is intended to flow toward the caster's palm while a ribbon-like aura circles the forearm. Releasing the input ends the stream; the remaining aura fades away.

The visual direction is elegant and ominous—not a storm of generic particles.

## 📖 The spellbook

| Spell | Gesture concept | Intended effect |
|:--|:--|:--|
| **I · Blood Drain** | Hold input and point | A flowing crimson stream and temporary forearm aura |
| **II · Blood Orb** | Cup the palm upward | Gather stored energy into a floating orb |
| **III · Blood Infusion** | Grip a weapon and cast | Wrap a held weapon in crimson magic |
| **IV · Blood Barrier** | Extend both hands | Form a defensive magical barrier |
| **V · Blood Tendrils** | Spread the fingers | Extend flowing magical ribbons from the hand |

Gesture recognition and all gameplay interactions must use inputs and APIs verified for the current Nomad modding framework. If a gesture is not supported, an accessible controller-input alternative will be needed.

## 🎨 Visual identity

- **Palette:** near-black, deep wine, dark crimson, restrained ember-red highlights.
- **Motion:** continuous flow, curling ribbons, ripples and subtle splashes.
- **Materials:** glossy supernatural liquid with controlled transparency.
- **Casting feel:** deliberate, weighty, responsive and readable in VR.
- **Performance:** designed around Quest hardware limits; avoid expensive effects and excessive transparent overdraw.

See [BRAND_GUIDE.md](BRAND_GUIDE.md) for the visual direction.

## 🧭 Development status

| Milestone | Status |
|:--|:--|
| Project concept and spell list | 🟢 Documented |
| Visual direction | 🟢 Documented |
| Verify current Nomad toolchain and APIs | 🟡 Not started |
| Blood Drain visual prototype | ⚪ Not started |
| Gesture/input implementation | ⚪ Not started |
| Additional spells | ⚪ Not started |
| Quest performance testing | ⚪ Not started |
| mod.io packaging and release | ⚪ Not started |

**First playable milestone:** Blood Drain's liquid stream and hand-following forearm aura, tested on actual Quest hardware.

## 🗂️ Project documents

- [Development plan](DEVELOPMENT.md) — technical phases and constraints
- [Spell design](SPELL_DESIGN.md) — behavior and visual goals
- [Testing checklist](TESTING.md) — compatibility and release checks
- [Brand guide](BRAND_GUIDE.md) — palette, effects and presentation
- [Changelog](CHANGELOG.md) — project history
- [Contributing](CONTRIBUTING.md) — project contribution guidelines

## ⚙️ Target platform

- **Game:** Blade & Sorcery: Nomad
- **Device family:** Meta Quest
- **Game version:** to be recorded when implementation and testing begin

Nomad and PCVR have different technical constraints. The current official Nomad documentation must be checked before choosing a project template, asset format, scripting approach, or package structure. PCVR-only instructions, Unity features, and arbitrary configuration files must not be assumed to work on Quest.

## 🤝 Project principles

1. Build one feature at a time and test it in-game.
2. Prefer polished, readable effects over visual clutter.
3. Keep Quest performance and VR comfort in mind.
4. Clearly label prototypes, untested code, and known limitations.
5. Use original or properly licensed assets only.

---

<div align="center">

**BLOODBOUND** · *A spell is a promise. A gesture is its price.*

<sub>Independent fan-made project. Not affiliated with or endorsed by Warpfrog or mod.io.</sub>

</div>
