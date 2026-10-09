# Veyra

**A new way to explore Minecraft graphics, built on Vulkan.**

> In development · Closed alpha testers wanted · No public build yet

Veyra is an independent graphics project for **Minecraft Java Edition**, built around Vulkan. Today, it brings together a native renderer with hardware ray-traced effects and an experimental way to run existing shaderpacks. But that's only the beginning of what I want Veyra to become.

## The vision: a graphics platform for Minecraft

I don't want Veyra to end as just another graphics mod with a fixed set of effects. My goal is to build a **platform that players and creators can grow with**.

For players, that means more ways to experience Minecraft: from native rendering with advanced lighting and materials, to familiar shaderpacks running through Vulkan, with control over how much work the GPU does.

For creators, the bigger ambition is a new generation of **Veyra shaders**: shaders designed to build on the platform's rendering technology rather than being limited to today's legacy shader formats. I want shader developers to be able to experiment with modern techniques and eventually have tools that make creating, testing, and refining those effects easier.

Just as important, I want the platform itself to keep moving forward. Rendering methods, shader capabilities, material systems, and creator tools should be things we continue improving — not features we implement once and leave untouched.

**That creator ecosystem is a long-term goal, not a toolset I'm claiming is ready today.** The current development work is laying the rendering and compatibility groundwork for it.

## Built for different ways to play

Advanced rendering can be demanding, and not everyone wants or needs the same setup. I want Veyra to offer meaningful choices rather than a single graphics mode.

### Native renderer

Veyra's own Vulkan renderer is being developed around hardware ray tracing, indirect lighting, soft shadows, reflections, water and glass, material-aware shading, and atmospheric effects. It's the place where I can explore rendering techniques directly and keep expanding the visual toolkit.

The current renderer also includes **FSR 3.1 upscaling**, **Native AA**, and experimental **frame generation**. These are options, not requirements: the aim is to let players choose the balance between image quality and performance that makes sense for their hardware. Frame generation can increase displayed frame rate, but doesn't increase game simulation speed or make input more responsive.

### Legacy shaderpacks

Veyra also has an experimental **Legacy** renderer for existing Iris/OptiFine-format shaderpacks, without requiring Iris or OptiFine to be installed.

I want players to be able to keep using the shaders they already enjoy, including **at native resolution without upscaling or frame generation**. Those features can also be useful as optional performance tools when running Legacy packs on less powerful hardware.

Some shaderpacks already launch and render in Veyra. Getting broader compatibility — including the visual details and settings that make each pack unique — is ongoing work.

### Future Veyra shaders and creator tools

Legacy compatibility matters, but it isn't the end goal for shader creation. The longer-term plan is to develop a **Veyra-native shader path** that creators can build for directly, with access to modern rendering capabilities and an evolving set of creator tools.

I want this to grow through experimentation and feedback from shader developers. The exact format, APIs, tooling, and release milestones still need to be designed and proven; Veyra-native shader authoring is **not yet being presented as a finished or publicly available feature**.

## Where development goes next

Right now, the priorities are improving the native renderer's visual quality and stability, testing Legacy shaderpacks more thoroughly, and measuring performance on different hardware. The closed alpha will help identify what works well and what still needs attention.

From there, the broader direction is to expand the rendering foundation, improve scalability across hardware, and develop the creator-facing side of Veyra over time. I want the platform to keep evolving alongside new graphics techniques and the people building with them.

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
