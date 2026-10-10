# Rimuru Tempest Mod — Fabric 1.21.1

A first playable, fan-made Tensura-inspired prototype for Minecraft Java Edition 1.21.1. It adds Rimuru's mask and five skill items. This is a starting build, not yet a full character model or complete anime-accurate skill system.

## Included in this prototype

- **Rimuru's Mask** — right-click for temporary Resistance and Night Vision.
- **Great Sage Crystal** — temporary Haste, Night Vision, and Resistance.
- **Predator Core** — Strength, Absorption, and Regeneration.
- **Water Blade Skill** — short Strength and Speed boost.
- **Black Flame Skill** — Strength and Fire Resistance.
- **Tempest Slime Heart** — healing, Regeneration, and Absorption.

Each ability has a cooldown. The items are currently registered in the creative inventory through the standard item registry, and can be obtained with commands such as `/give @s rimuru_tempest:rimuru_mask`.

## Requirements

- Minecraft Java Edition **1.21.1**
- Java **21** JDK
- Fabric Loader 0.16.10 or newer
- Fabric API for 1.21.1
- Gradle 8.x (or import this folder in IntelliJ IDEA with the Gradle integration)

## Build the mod

From this folder, run:

```bash
gradle build
```

The built JAR should appear in `build/libs/`. Copy the non-sources JAR into your CurseForge profile's `mods` folder. Make sure that profile uses Minecraft 1.21.1, Fabric, and Fabric API for 1.21.1.

## Test items

In a creative world or with cheats enabled, run:

```mcfunction
/give @s rimuru_tempest:rimuru_mask
/give @s rimuru_tempest:great_sage_crystal
/give @s rimuru_tempest:predator_core
/give @s rimuru_tempest:water_blade
/give @s rimuru_tempest:black_flame
/give @s rimuru_tempest:slime_heart
```

Hold an item and right-click to activate it.

## Next development pass

The current version is deliberately a small prototype. The next major additions should be proper custom item textures, a wearable 3D mask/armor model, slime transformation, target-based Predator absorption, projectile attacks, and client-side skill keybinds with server networking. Those require additional model and gameplay work beyond this initial slice.
