# Performance Mods

A list of performance-enhancing mods for 1.17.x forge/fabric versions.

Any suggestions/complaints?
Join our [discord](https://discord.gg/8nzHYhVUQS) or use the issues.

[![Home](https://i.imgur.com/zGuelkW.png)](/README.md)

## Fabric 1.17.X

| Name | Known Incompatibilities | Description | Author | Performance Improvement | [Label](/README.md/#labels) |
| --- | :---: | :---: | :---: | :---: | :---: |
| [Alternate Current](https://modrinth.com/mod/alternate-current) | Unknown | Alternate Current is an efficient and non-locational redstone dust implementation | Space Walker | Server | none |
| [Better Beds](https://www.curseforge.com/minecraft/mc-mods/better-beds) | Unknown | Removes the Block Entity Renderer from the bed and replaces it with the default minecraft model renderer. | Motschen | Client | none |
| [Better Biome Blend](https://www.curseforge.com/minecraft/mc-mods/better-biome-blend) | Sodium | Better Biome Blend is a mod  which accelerates the biome color blending algorithm. | FionaTheMortal | Client | none |
| [C2ME](https://github.com/YatopiaMC/C2ME-fabric/releases)| Tic-Tacs, + | A Fabric mod designed to improve the chunk performance of Minecraft. | YatopiaMC | Server | Alpha (1) |
| [Canvas](https://www.curseforge.com/minecraft/mc-mods/canvas-renderer) | Sodium | Advanced Rendering Engine for Fabric | grondag | Client | Alpha (1) |
| [Clumps](https://www.curseforge.com/minecraft/mc-mods/clumps) | Unknown | Clumps groups XP orbs together into a single entity to reduce lag when there are many in a small area. | jaredlll08 | Both | none |
| [Cull Leaves](https://www.curseforge.com/minecraft/mc-mods/cull-leaves) | Unknown | Adds culling to leaf blocks, providing a huge performance boost over vanilla. | Motschen | Client | none |
| [DashLoader](https://www.curseforge.com/minecraft/mc-mods/dashloader)| Enhanced Block Entities | This mod launches minecraft faster by caching all of the content on first launch and then loading that cache on the next one | alphaqu | Client | Incompatible (4) |
| [Dimensional Threading](https://github.com/WearBlackAllDay/DimensionalThreading/releases)| Unknown | Minecraft mod which optimizes the processing of multiple Dimensions, by assigning them independent threads | WearBlackAllDay | Server | none |
| [Dynamic FPS](https://modrinth.com/mod/dynamic-fps) | Unknown | Automatically reduces rendering speed when minecraft is not focused (to 1 FPS) or hidden (no renders at all). | juliand665 | Client | none |
| [Dynamic View](https://www.curseforge.com/minecraft/mc-mods/dynamic-view) | APTweaks | This is a small/light serverside utility mod to help balancing lag (TPS) and chunk view/load distance. | someaddon | Server | none |
| [Enhanced Block Entities](https://modrinth.com/mod/ebe) | Sodium[⁴](https://github.com/NordicGamerFE/usefulmods/tree/main#-some-of-the-mods-that-have-sodium-as-an-incompatibility-might-work-if-you-use-indium), DashLoader | EBE is a mod which aims to increase the performance of block entity rendering, as well as offer customizability via resource packs. | FoundationGames | Client | none |
| [Entity Distance](https://modrinth.com/mod/entity-distance) | Unknown | Allows the user to adjust the (client) distance at which different entities render | capnkork | Client | none |
| [EntityCulling](https://www.curseforge.com/minecraft/mc-mods/entityculling) | none | EntityCulling using async path-tracing to skip rendering Tiles/Entities that are not visible | tr9zw | Client | none |
| [FastChest](https://www.curseforge.com/minecraft/mc-mods/fastchest) | Unknown | This mod helps by removing dynamic models from chests and making them render as static chunk geometry. | fake_domi | Client | none |
| [FastFurnace](https://www.curseforge.com/minecraft/mc-mods/fast-furnace-for-fabric) | Recipe Cache | Similar to FastWorkbench, it caches the last recipe used, and checks this recipe first before re-scanning the entire registry | tfarecnim | Server | none |
| [FerriteCore](https://www.curseforge.com/minecraft/mc-mods/ferritecore-fabric) | Unknown | This mod reduces the memory usage of Minecraft in a few different ways | malte0811 | Both | none |
| [Hydrogen](https://modrinth.com/mod/hydrogen) | Unknown | Reduces the memory usage of the game in more modded scenarios | CaffeineMC | Client | Alpha (1) |
| [Krypton](https://www.curseforge.com/minecraft/mc-mods/krypton) | Unknown | Krypton is a Minecraft mod designed for the Fabric mod loader that implements a suite of optimizations focused on the Minecraft networking stack | astei | Both | Alpha (1) |
| [Ksyxis](https://www.curseforge.com/minecraft/mc-mods/ksyxis) | Unknown | Speeds up your world loading by not loading nearby chunks every time. | VidTu | Both | Reverse Features (1) |
| [LazyDFU](https://www.curseforge.com/minecraft/mc-mods/lazydfu) | None | LazyDFU is an optimization mod that makes the initialization of DataFixerUpper "lazy" | astei | Both | none |
| [Lazy Language Loader](https://www.curseforge.com/minecraft/mc-mods/lazy-language-loader) | Unknown | Lazy Language Loader improves loading times when changing your language by only reloading the language instead of all the game resources! | chachylmao | Client | none |
| [Lithium](https://www.curseforge.com/minecraft/mc-mods/lithium) | none | Lithium is a general-purpose optimization mod for Minecraft which works to improve a number of systems without changing any behavior | CaffeineMC | Server | none |
| [MemoryLeakFix](https://www.curseforge.com/minecraft/mc-mods/memoryleakfix) | Unknown | A mod that fixes multiple memory leaks in minecraft. Both server-side & client-side. | FX_PR0CESS | Both | none |
| [Mipmaplevel and Language Fix](https://modrinth.com/mod/mipmaplevelandlanguagefix) | Unknown | Makes changing Mipmaplevels and Language faster, by instead of doing a full reload, only reloading the respective part of the game. | KingContaria | Client | none |
| [Observable](https://github.com/tasgon/observable/releases/tag/0.1.2-1.17) | Unknown | Shows what's lagging your world/server by profiling (tile) entities. | tasgon | Server | none |
| [Phosphor](https://www.curseforge.com/minecraft/mc-mods/phosphor) | Starlight | Phosphor is a Minecraft mod which works to optimize one of game's most inefficient areas, the lighting engine | CaffeineMC | Both | none |
| [Recipe Cache](https://www.curseforge.com/minecraft/mc-mods/recipe-cache) | FastFurnace, FastBench (?) | Caches recipe lookup for crafting and furnaces to lessen server lag caused by crafting stacks of items and large amounts of furnaces ticking | biom4st3r1 | Server |  none |
| [Resolution Control+](https://github.com/UltimateBoomer/Resolution-Control/releases) | Unknown | ResolutionControl+ allows you to change Minecraft's render resolution separately from the HUD elements. | Ultimate Boomer | Client | none |
| [ServerCore](https://modrinth.com/mod/servercore) | Unknown | A fabric mod that aims to optimize & add multiplayer features to the minecraft server. | Wesley1808 | Server | Buggy (2) |
| [Simply No Shading](https://www.curseforge.com/minecraft/mc-mods/simply-no-shading) | This mod mimics OptiFine's Internal Shader with Old Lighting OFF by default. Benefits are less lag as this mod is not a shader, stability, and compatibility with other mods. | StartsMercury | Client | none |
| [Smoke Suppresion](https://www.curseforge.com/minecraft/mc-mods/smoke-suppression) | Unknown | This is to prevent client-side lag and general annoyance when using large numbers of campfires in farms. | supersaiyansubtlety | Client | none |
| [Smooth Boot](https://www.curseforge.com/minecraft/mc-mods/smooth-boot) | Unknown | Optimize Minecraft loading performance to be smoother on low end systems and scale better on high end systems | UltimateBoomer | Both | none |
| [Sodium](https://modrinth.com/mod/sodium) | Mods that utilize the FRAPI[⁴](https://github.com/NordicGamerFE/usefulmods/tree/main#-some-of-the-mods-that-have-sodium-as-an-incompatibility-might-work-if-you-use-indium) | Sodium is a free and open-source rendering engine replacement for the Minecraft client that greatly improves frame rates, reduces micro-stutter, and fixes graphical issues in Minecraft | CaffeineMC | Client |  none |
| [Starlight](https://modrinth.com/mod/starlight) | Unknown | Fabric mod for completely rewriting the vanilla light engine. | Spottedleaf (PaperMC) | Both |  none |
| [Very Many Players](https://modrinth.com/mod/vmp-fabric) | Unknown | Very Many Players, or VMP for short, is a Fabric mod designed to improve general server performance at high playercount without sacrificing vanilla functionality or behavior. | ishland | Server |  Alpha (4) |
| [VulkanMod](https://github.com/xCollateral/VulkanMod/releases) | Unknown | a fabric mod that rewrites Minecraft OpenGL renderer to use Vulkan API. | xCollateral | Client | Incompatible (6) |

## Forge 1.17.X

| Name | Known Incompatibilities | Description | Author | Performance Improvement | [Label](/README.md/#labels) |
| --- | :---: | :---: | :---: | :---: | :---: |
| [AI Improvements](https://www.curseforge.com/minecraft/mc-mods/ai-improvements)[⁵](/README.md#-ai-improvements-newer-versions-114-dont-have-as-much-impact-as-the-older-versions-have-since-in-newer-versions-of-minecraft-a-lot-of-fixes-to-the-ai-are-implemented-sources-curseforge-page-faq-dev) | none | Simplified AI modification mod focused on performance and low-level modifications to AIs in the game | QueenOfMissiles | Server | none |
| [Better Biome Blend](https://www.curseforge.com/minecraft/mc-mods/better-biome-blend) | Probably any Sodium port | Better Biome Blend is a mod  which accelerates the biome color blending algorithm. | FionaTheMortal | Client |  none |
| [Better Fps - Render Distance](https://www.curseforge.com/minecraft/mc-mods/better-fps-render-distance) | Unknown | Better FPS Render Distance is a mod which adds a few performance improvements to increase fps. | someaddon | Client | none |
| [Clumps](https://www.curseforge.com/minecraft/mc-mods/clumps) | Unknown | Clumps groups XP orbs together into a single entity to reduce lag when there are many in a small area. | jaredlll08 | Both | none |
| [Dynamic View](https://www.curseforge.com/minecraft/mc-mods/dynamic-view) | APTweaks | This is a small/light serverside utility mod to help balancing lag (TPS) and chunk view/load distance. | someaddon | Server | none |
| [EntityCulling](https://www.curseforge.com/minecraft/mc-mods/entityculling) | none | EntityCulling using async path-tracing to skip rendering Tiles/Entities that are not visible | tr9zw | Client | none |
| [FastFurnace](https://www.curseforge.com/minecraft/mc-mods/fastfurnace) | Unknown | Similar to FastWorkbench, it caches the last recipe used, and checks this recipe first before re-scanning the entire registry. | Shadows_of_Fire | Server | none |
| [FastSuite](https://www.curseforge.com/minecraft/mc-mods/fastsuite) | Unknown | FastSuite is a mod about improving recipe performance, it improves upon all mods that use the JSON recipe system, rather than just a specific subset of recipes | Shadows_of_Fire | Server | none |
| [FastWorkbench](https://www.curseforge.com/minecraft/mc-mods/fastworkbench) | Unknown | This is a mod aimed at improving performance of all crafting-related functions. | Shadows_of_Fire | Server | none |
| [FerriteCore](https://www.curseforge.com/minecraft/mc-mods/ferritecore) | Unknown | This mod reduces the memory usage of Minecraft in a few different ways | malte0811 | Both | none |
| [Get It Together, Drops!](https://www.curseforge.com/minecraft/mc-mods/get-it-together-drops) | Unknown | This mod adds two configuration options to control how dropped items combine on the ground. This can significantly improve performance in areas with lots of dropped items | bl4ckscor3 | Server | none |
| [Ksyxis](https://www.curseforge.com/minecraft/mc-mods/ksyxis) | Unknown | Speeds up your world loading by not loading nearby chunks every time. | VidTu | Both | Reverse Features (1) |

[![Home](https://i.imgur.com/zGuelkW.png)](/README.md)
