# Development plan

## Current status

**Phase 0 — Repository and design setup.** This is documentation only. No compiled mod, Unity project, game scripts, or Quest-ready asset bundle exists yet.

## Phase 1 — Verify the current Nomad workflow

Before writing implementation code:

1. Confirm the latest installed Blade & Sorcery: Nomad game version.
2. Read the current official Nomad modding documentation and supported SDK/toolchain.
3. Confirm how Nomad mods are packaged, where files are installed, and which mod metadata format is required.
4. Confirm which scripting APIs and runtime features are supported on Quest.
5. Record the source links and tested game version here.

Do not copy PCVR-only instructions into a Nomad project without verification.

## Phase 2 — Blood Drain visual prototype

Goal: a low-cost, stylized liquid effect prototype.

- Build a continuous-looking crimson ribbon using supported Quest-compatible rendering techniques.
- Attach the receiving effect to the player's hand without visible lag.
- Add a temporary forearm aura that follows the arm.
- Use restrained transparency and overdraw to protect Quest performance.
- Provide a clean stop/fade-out when the spell input is released.

The visual prototype must first be tested independently of NPC gameplay interaction.

## Phase 3 — Input and target interaction

- Map the spell to supported Nomad controller inputs.
- Implement reliable target selection and range checks using supported APIs.
- Avoid accidental activation during ordinary movement.
- Ensure the effect stops safely when the target becomes invalid, leaves range, or the player releases the input.
- Keep NPC gameplay effects non-graphic and use normal game defeat behavior where supported.

## Phase 4 — Additional spells

Implement one at a time after Blood Drain is stable:

1. Blood Orb
2. Blood Infusion
3. Blood Barrier
4. Blood Tendrils

Use a shared energy resource only if the supported Nomad framework allows it reliably.

## Phase 5 — Optimization and release

- Test on actual Quest hardware.
- Check frame rate, memory use, particle count, transparency overdraw, and effect cleanup.
- Test with multiple NPCs and other mods.
- Package using the verified Nomad format.
- Prepare mod.io metadata, screenshots, version notes, and compatibility statement.

## Development constraints

The project owner currently has an Android phone only. Repository documentation and text files can be managed from the phone, but a complete Unity-based asset and mod build may require access to a Windows or macOS computer. Do not claim a mod is installable until it has been built and tested on Quest.