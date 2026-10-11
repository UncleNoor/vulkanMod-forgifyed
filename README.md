<div align='center'>

# VulkanMod for Forge 1.20.1

A Forge 1.20.1 port of **VulkanMod**, the mod that rewrites Minecraft's OpenGL renderer to use the Vulkan API,
with optional hardware ray traced effects on top.

</div>

## Credits

**VulkanMod was created by [Collateral (xCollateral)](https://github.com/xCollateral/VulkanMod).**
The renderer, the Vulkan backend and nearly everything this port builds on is their work, and the full
history of their commits is kept in this repository. If you enjoy this port, go support the original mod.

Forge 1.20.1 port, ray tracing features and modpack compatibility fixes by **uncle-Noor**.

## What this port adds

- Runs on Forge 1.20.1 (47.x) instead of Fabric
- Ray traced sun and moon shadows, with player and mob shadows (needs a GPU with Vulkan ray queries:
  NVIDIA RTX, AMD RX 6000 or newer, Intel Arc)
- Volumetric sun rays
- Colored light with ray traced shadows from torches, lava and other light emitting blocks,
  and dynamic light from held or dropped glowing items
- A redesigned settings screen, a GPU picker, extra detail and performance options, and pipeline
  preloading to avoid stutter
- Compatibility fixes for mods such as Replay Mod, TaCZ, CustomNPCs, LibGui, SecurityCraft and Warium

All ray tracing features can be turned off in Video Settings, on the Ray Tracing page.

## Installation

- Forge 1.20.1 (47.x) is needed.
- Move the VulkanMod jar to the `mods` folder of your Minecraft instance.
- Not compatible with Oculus, Embeddium, Rubidium, Xaero's World Map or ImmediatelyFast.

## Building

```
./gradlew build
```

The jar is written to `build/libs`.

## License

LGPL-3.0, like the original VulkanMod. See [LICENSE](LICENSE).
