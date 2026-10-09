# Veyra

**A new way to explore Minecraft graphics, built on Vulkan.**

> In development · Closed alpha testers wanted · No public build yet

Veyra is a Vulkan-based graphics project for **Minecraft Java Edition**. It combines a native renderer with hardware ray-traced effects and experimental support for existing shaderpacks.

The longer-term aim is to build a graphics platform that serves both players and shader creators.

## Project direction

Veyra is being developed with three goals in mind:

- **Modern rendering:** continue improving native lighting, reflections, materials, and other graphics features.
- **Choice for players:** support different hardware and preferences, from advanced native rendering to familiar shaderpacks, with optional upscaling and frame generation.
- **Tools for creators:** work toward a Veyra-native shader format and tools that let shader developers use modern rendering features directly.

The creator tools and Veyra-native shader format are **long-term plans**, not available features. Development currently focuses on the renderer, shader compatibility, image quality, and stability.

## Rendering options

### Native renderer

Veyra's native Vulkan renderer includes hardware ray tracing, indirect lighting, soft shadows, reflections, water and glass effects, material-aware shading, and atmospheric effects.

It also offers **FSR 3.1 upscaling**, **Native AA**, and experimental **frame generation**, depending on hardware and settings. These are optional: players can render at native resolution or use reconstruction features when they want to trade some image quality for performance. Frame generation improves displayed frame rate, not game simulation speed or input latency.

### Legacy shaderpacks

The experimental Legacy renderer can run existing Iris/OptiFine-format shaderpacks through Vulkan, without Iris or OptiFine installed.

Players can use compatible packs at native resolution or choose upscaling and experimental frame generation where supported. Shader compatibility and visual accuracy are still being improved.

### Future creator support

Over time, I want shader developers to be able to create **Veyra-native shaders** that work with the platform's rendering capabilities. The aim is to develop the shader format and creator tools alongside the renderer, rather than treat them as a one-off feature.

## Current focus

The next steps are better visual consistency, broader Legacy compatibility, more performance testing, and feedback from closed alpha testers. These results will help shape the longer-term creator platform.

## Native renderer screenshots

Here are five in-game screenshots of Veyra's native renderer.

![Veyra native renderer — screenshot 1](assets/screenshots/veyra-native-01.png)

![Veyra native renderer — screenshot 2](assets/screenshots/veyra-native-02.png)

![Veyra native renderer — screenshot 3](assets/screenshots/veyra-native-03.png)

![Veyra native renderer — screenshot 4](assets/screenshots/veyra-native-04.png)

![Veyra native renderer — screenshot 5](assets/screenshots/veyra-native-05.png)

## Shaderpacks tested so far

These four versions have been **manually tested on my development PC** and have launched, rendered, and remained playable during normal gameplay:

| Shaderpack | Version |
| --- | --- |
| Complementary Unbound | r5.9.3 |
| Sildur's Vibrant Shaders | v2.02 Extreme-VL |
| MakeUp UltraFast | 9.5g |
| BSL | v10.1.8 |

That's a starting point, not a full compatibility list. I'm still checking visual differences, individual settings, longer sessions, and how things behave on other hardware.

## Current development setup

- **Minecraft:** Java Edition 26.3
- **Mod loader:** NeoForge 26.3.0.45-beta
- **Java:** 25
- **Graphics API:** Vulkan
- **Main test system:** Windows x64, AMD Radeon RX 9070

## Help test Veyra

I'm preparing a **small closed alpha** and looking for people who want to help test it — especially on different GPUs and with different shaderpacks.

I'm interested in what works, what breaks, how performance compares, and where the visuals need attention. Real feedback will help me figure out what to focus on next.

**Want to get involved?** Join the Discord and visit **#alpha-testing** to register your interest.

**[Join the Veyra Discord — Closed Alpha](https://discord.gg/aFFZhCYBSV)**

I'll select testers manually as the alpha becomes ready. There isn't a public download yet, and joining Discord doesn't guarantee a test spot.

---

Veyra is an independent project and is not affiliated with Mojang Studios or Microsoft.
