# Veyra

**A new way to explore Minecraft graphics, built on Vulkan.**

> In development · Closed alpha testers wanted · No public build yet

Veyra is an independent, client-side **graphics project for Minecraft Java Edition**, built around Vulkan. It isn't a new shaderpack. It's a rendering layer with its own graphics features, settings, and experimental support for existing shaderpacks.

The idea started with a question: **what if Minecraft had a graphics platform that could grow beyond a single shaderpack or one rendering technique?**

I'm working on two approaches in the same project: Veyra's own native renderer and a Legacy renderer for community shaderpacks. Both are still in development, but they're steps toward a bigger goal: giving players more choice over how Minecraft looks and runs.

## What I'm trying to build

My long-term goal is for Veyra to become a **flexible graphics platform for Minecraft**, not just a collection of visual effects.

That means working toward:

- **More rendering choice:** continue developing native Vulkan rendering while improving the ability to use existing shaderpacks through the Legacy renderer.
- **Better materials:** build on normal maps, specular maps, LabPBR support, and experimental material generation so blocks can respond more convincingly to light.
- **Controls that matter:** give players understandable quality presets and deeper controls for lighting, reflections, reconstruction, and other effects.
- **A wider range of hardware:** test different GPUs and find sensible ways to scale graphics quality. Hardware support and performance still need real-world validation.
- **A foundation that can keep evolving:** improve the renderer's architecture, visual consistency, and compatibility rather than treating any one visual feature as the finish line.

Those are **directions I'm working toward, not a promised feature list or release schedule**. The near-term priority is getting the current renderer stable, improving image quality and performance, and learning from testers.

## Two ways to render

### Native rendering

Veyra's own renderer is where I'm experimenting with **hardware ray tracing**, indirect lighting, soft shadows, reflections, water and glass, materials, and atmospheric effects.

It also includes **FSR 3.1 upscaling**, **Native AA**, and experimental **frame generation**. Which options work depends on your hardware and configuration. Frame generation can make motion appear smoother, but it doesn't increase the game's simulation speed or reduce input latency.

There's still plenty to improve, especially when it comes to image quality, stability, and performance. That's part of why I'm sharing the project now.

### Existing shaderpacks, through Vulkan

I'm also working on a **Legacy renderer** that can load existing Iris/OptiFine-format shaderpacks without Iris or OptiFine being installed.

Some packs already launch and render in Veyra. Compatibility is still a work in progress, though: a pack running doesn't necessarily mean every effect looks or behaves exactly as it does in Iris.

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
