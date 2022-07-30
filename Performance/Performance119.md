# Performance Mods

A list of performance-enhancing mods for 1.19.x forge/fabric versions.

Any suggestions/complaints?

Join our [discord](https://discord.gg/8nzHYhVUQS) or use the issues.

[![Home](https://i.imgur.com/zGuelkW.png)](/README.md)

## Fabric 1.19.X

| Name | Known Incompatibilities | Description | Author | Performance Improvement | [Label](/README.md#labels) |
| --- | :---: | :---: | :---: | :---: | :---: |
| [Alternate Current](https://modrinth.com/mod/alternate-current) | Unknown | Alternate Current is an efficient and non-locational redstone dust implementation. | Space Walker | Server | None |
| [Better Beds](https://www.curseforge.com/minecraft/mc-mods/better-beds) | Unknown | Removes the Block Entity Renderer from the bed and replaces it with the default minecraft model renderer. | Motschen | Client | None |
| [C2ME](https://github.com/RelativityMC/C2ME-fabric/releases) | Unknown | A Fabric mod designed to improve the chunk performance of Minecraft. | YatopiaMC | Both | Alpha (1) |
| [Clumps](https://www.curseforge.com/minecraft/mc-mods/clumps) | Unknown | Clumps groups XP orbs together into a single entity to reduce lag when there are many in a small area. | jaredlll08 | Both | none |
| [Cull Leaves](https://www.curseforge.com/minecraft/mc-mods/cull-leaves) | Unknown | Adds culling to leaf blocks, providing a huge performance boost over vanilla. | Motschen | Client | none |
| [Cull Less Leaves](https://www.curseforge.com/minecraft/mc-mods/cull-less-leaves) | Unknown | Cull Less Leaves is an improved version of Cull Leaves. | XanderIsDev | Client | none |
| [DashLoader](https://www.curseforge.com/minecraft/mc-mods/dashloader) | Unknown | This mod launches minecraft faster by caching all of the content on first launch and then loading that cache on the next one | alphaqu | Client | Incompatible (2) |
| [Dynamic FPS](https://modrinth.com/mod/dynamic-fps) | Unknown | Automatically reduces rendering speed when minecraft is not focused (to 1 FPS) or hidden (no renders at all). | juliand665 | Client | none |
| [Entity Culling](https://www.curseforge.com/minecraft/mc-mods/entityculling) | Unknown | EntityCulling using async path-tracing to skip rendering Tiles/Entities that are not visible. | tr9zw | Client | none |
| [Entity Collision FPS Fix](https://modrinth.com/mod/entity-collision-fps-fix) | Unknown | Client Side mod that optimizes entity's on the render thread. | CorgiTaco | Client | none |
| [FastAnim](https://www.curseforge.com/minecraft/mc-mods/fastanim) | Unknown | FastAnim is a mod that improves the animation speed of entities. | Motschen | Client | none |
| [Fastload](https://www.curseforge.com/minecraft/mc-mods/fastload) | Unknown | Fastload, is a simple mod that reduces world loading time. This serves as an alternative to ksyxis, which uses an unsafe method of cutting down time. | overloadedwithmods | Both | none |
| [FerriteCore](https://www.curseforge.com/minecraft/mc-mods/ferritecore-fabric) | Unknown | This mod reduces the memory usage of Minecraft in a few different ways | malte0811 | Both | none |
| [ForgetMeChunk](https://modrinth.com/mod/forgetmechunk) | Unknown | Fixes the large lag spikes you sometimes get when crossing a chunk border | BreadLoaf | Client | none |
| [Krypton](https://www.curseforge.com/minecraft/mc-mods/krypton) | Unknown | Krypton is a Minecraft mod designed for the Fabric mod loader that implements a suite of optimizations focused on the Minecraft networking stack. | astei | Both | none |
| [LazyDFU](https://www.curseforge.com/minecraft/mc-mods/lazydfu) | Unknown | LazyDFU is an optimization mod that makes the initialization of DataFixerUpper "lazy" | tr9zw | Both | none |
| [Lithium](https://www.curseforge.com/minecraft/mc-mods/lithium) | Unknown | Lithium is a general-purpose optimization mod for Minecraft which works to improve a number of systems without changing any behavior | jellysquid3_ | Server | none |
| [MemoryLeakFix](https://www.curseforge.com/minecraft/mc-mods/memoryleakfix) | Unknown | A mod that fixes multiple memory leaks in minecraft. Both server-side & client-side. | FX_PR0CESS | Both | none |
| [Mipmaplevel and Language Fix](https://modrinth.com/mod/mipmaplevelandlanguagefix) | Unknown | Makes changing Mipmaplevels and Language faster, by instead of doing a full reload, only reloading the respective part of the game. | KingContaria | Client | none |
| [More Culling](https://www.curseforge.com/minecraft/mc-mods/moreculling) | See [MoreCulling#6](https://github.com/fxmorin/MoreCulling/issues/6) | changes how blockstate culling is handled in order to improve performance | FX_PR0CESS | Client | None |
| [Particle Blocker](https://modrinth.com/mod/particles) | Unknown | Adds a GUI to pick and choose particles to not render. | Declipsonator | Client | none |
| [Simply No Shading](https://www.curseforge.com/minecraft/mc-mods/simply-no-shading) | Unknown | This mod mimics OptiFine's Internal Shader with Old Lighting OFF by default. Benefits are less lag as this mod is not a shader, stability, and compatibility with other mods. | StartsMercury | Client | none |
| [Sodium](https://www.curseforge.com/minecraft/mc-mods/sodium) | Mods that utilize of the FRAPI[⁴](https://github.com/NordicGamerFE/usefulmods/tree/main#-some-of-the-mods-that-have-sodium-as-an-incompatibility-might-work-if-you-use-indium) | Sodium is a free and open-source rendering engine replacement for the Minecraft client that greatly improves frame rates, reduces micro-stutter, and fixes graphical issues in Minecraft. | jellysquid3_ | Client | none |
| [ServerCore](https://modrinth.com/mod/servercore) | Unknown | A fabric mod that aims to optimize & add multiplayer features to the minecraft server. | Wesley1808 | Server | none |
| [Smooth Boot](https://www.curseforge.com/minecraft/mc-mods/smooth-boot) | Unknown | Optimize Minecraft loading performance to be smoother on low end systems and scale better on high end systems. | UltimateBoomer | Both | none |
| [Starlight](https://www.curseforge.com/minecraft/mc-mods/starlight) | Unknown | Fabric mod for completely rewriting the vanilla light engine. | Spottedstar | Both | none |
| [Very Many Players](https://modrinth.com/mod/vmp-fabric) | Unknown | Very Many Players, or VMP for short, is a Fabric mod designed to improve general server performance at high playercount without sacrificing vanilla functionality or behavior. | ishland | Server | none |
| [VulkanMod](https://github.com/xCollateral/VulkanMod/releases) | Sodium | a fabric mod that rewrites Minecraft OpenGL renderer to use Vulkan API. | xCollateral | Client | Incompatible(6) |

## Forge 1.19.X

| Name | Known Incompatibilities | Description | Author | Performance Improvement | [Label](/README.md#labels) |
| --- | :---: | :---: | :---: | :---: | :---: |
| [Clumps](https://www.curseforge.com/minecraft/mc-mods/clumps) | Unknown | Clumps groups XP orbs together into a single entity to reduce lag when there are many in a small area. | jaredlll08 | Both | none |
| [Entity Culling](https://www.curseforge.com/minecraft/mc-mods/entityculling) | Unknown | EntityCulling using async path-tracing to skip rendering Tiles/Entities that are not visible. | tr9zw | Client | none |
| [Entity Collision FPS Fix](https://modrinth.com/mod/entity-collision-fps-fix) | Unknown | Client Side mod that optimizes entity's on the render thread. | CorgiTaco | Client | none |
| [FerriteCore](https://www.curseforge.com/minecraft/mc-mods/ferritecore) | Unknown | This mod reduces the memory usage of Minecraft in a few different ways | malte0811 | Both | none |
| [It Shall Not Tick (ISNT)](https://www.curseforge.com/minecraft/mc-mods/it-shall-not-tick) | Unknown | It Shall Not Tick (ISNT) is a performance enhancing mod that limits entity ticking to within a configurable range of players. | Gaz_ | Server | none |
| [Krypton Reforged](https://www.curseforge.com/minecraft/mc-mods/krypton-reforged) | Unknown | Krypton Reforged is a Minecraft mod that implements a suite of optimizations focused on the Minecraft networking stack. | TeamDeusVult | Both | none |
| [Radon](https://www.curseforge.com/minecraft/mc-mods/radon) | Unknown | Radon is an Unofficial Fork of CaffeineMC's "Phosphor", made to work with Forge Mod Loader. | Asek3 | Both | none |
| [Rubidium](https://www.curseforge.com/minecraft/mc-mods/rubidium) | Magnesium, Optifine | Rubidium is an Unofficial Fork of CaffeineMC's "Sodium", made to work with Forge Mod Loader. | Asek3 | Client | none |

[![Home](https://i.imgur.com/zGuelkW.png)](/README.md)
