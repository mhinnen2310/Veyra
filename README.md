# Veyra
**Minecraft graphics on Vulkan — native ray-traced rendering and experimental support for existing shaderpacks.**

> **In active development · Closed alpha planned · No public download yet**

Veyra is an independent, client-side graphics project for **Minecraft Java Edition**. It explores two complementary ways to render Minecraft on Vulkan: an in-house renderer for ray-traced effects and an experimental **Legacy** renderer for existing Iris/OptiFine-format shaderpacks.

## What Veyra does

**Native renderer:** Configurable ray-traced lighting and indirect illumination, soft shadows, reflections, water and glass effects, material-aware shading, and atmospheric effects. Veyra also includes experimental **FSR 3.1 upscaling**, **Native AA**, and optional **frame generation**. Availability depends on the GPU and configuration. Generated frames do not improve simulation speed or input responsiveness.

**Legacy shaderpacks on Vulkan:** An experimental way to load existing shaderpacks without needing Iris or OptiFine installed. Shader compatibility and visual accuracy are still under development.

## Native renderer showcase

The upcoming screenshot gallery contains **only captures of Veyra's own native renderer**, not external shaderpacks. Planned scenes include water reflections, a nighttime village, a sea-lantern-lit interior, lava lighting and an experimental tinted-glass test. These are development previews, not claims of flawless effects or proven visual accuracy.

*Screenshots are being prepared for upload.*

## Current shaderpack compatibility baseline

Four shaderpack versions have been manually tested and reported to launch, render and remain playable during normal gameplay on the **primary development PC**:

| Shaderpack | Version |
| --- | --- |
| Complementary Unbound | r5.9.3 |
| Sildur's Vibrant Shaders | v2.02 Extreme-VL |
| MakeUp UltraFast | 9.5g |
| BSL | v10.1.8 |

This intentionally limited baseline **does not guarantee** full visual parity with Iris, perfect behavior for every shader option, long-session stability or compatibility on other hardware. More shaderpacks will be introduced and tested individually. Earlier exploratory runs with additional or older packs are not part of the present compatibility baseline. Third-party shaderpacks are not bundled.

## Development status

- **Minecraft target:** Java Edition 26.3
- **Mod loader:** NeoForge 26.3.0.45-beta
- **Java:** 25
- **Graphics backend:** Vulkan
- **Primary validation:** Windows x64 with an AMD Radeon RX 9070
- **Release stage:** experimental development; optimization, visual quality and broader compatibility remain works in progress

## Closed alpha — testers wanted

A limited, manually selected closed alpha is planned. The goal is to test stability, rendering differences, shaderpack behavior, performance, and different GPU configurations.

There is **no public download or open registration yet**. Watch this repository for updates. A Discord invitation and tester application details will be added when available.

## Source code and rights

Veyra's development source code is **private** and is not distributed through this showcase repository. No public binaries or blanket redistribution permission are provided here. Third-party shaderpacks remain the property of their respective authors.

Veyra is an independent project, not affiliated with Mojang Studios or Microsoft.
