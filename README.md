# Veyra

**A new way to explore Minecraft graphics, built on Vulkan.**

> In development · Closed alpha testers wanted · No public build yet

I'm building Veyra because I want to explore what Minecraft rendering can look like with Vulkan — both with a renderer built specifically for Veyra and with the shaderpacks the community already knows.

Veyra is a client-side graphics project for **Minecraft Java Edition**, with two parts that I'm developing side by side.

## Two ways to render

### Native rendering

Veyra's own renderer is where I'm experimenting with **hardware ray tracing**, indirect lighting, soft shadows, reflections, water and glass, materials, and atmospheric effects.

It also includes **FSR 3.1 upscaling**, **Native AA**, and experimental **frame generation**. Which options work depends on your hardware and configuration. Frame generation can make motion appear smoother, but it doesn't increase the game's simulation speed or reduce input latency.

There's still plenty to improve, especially when it comes to image quality, stability, and performance. That's part of why I'm sharing the project now.

### Existing shaderpacks, through Vulkan

I'm also working on a **Legacy renderer** that can load existing Iris/OptiFine-format shaderpacks without Iris or OptiFine being installed.

Some packs already launch and render in Veyra. Compatibility is still a work in progress, though: a pack running doesn't necessarily mean every effect looks or behaves exactly as it does in Iris.

## Native renderer screenshots

Here are five **unedited in-game screenshots from Veyra's native renderer** — not from third-party shaderpacks. They show the renderer as it looks during development.

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

That's a starting point, not a full compatibility list. I'm still checking visual differences, individual settings, longer sessions, and how things behave on other hardware. Shaderpacks aren't included with Veyra.

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
