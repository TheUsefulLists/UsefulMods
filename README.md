# Performance Mods
A list of performance-enhancing mods for 1.17.x forge/fabric versions.

Any suggestions/complaints?<br>
Join our [discord](https://discord.gg/8nzHYhVUQS) or use the issues.<br><br>
Mods marked as "*Dangerous*" might be unstable, and cause some unexpected behaviour.

[![Home](https://i.imgur.com/zGuelkW.png)](https://github.com/NordicGamerFE/usefulmods/tree/main)


## Fabric 1.17.X

| Name | Known Incompatibilities | Description | Author | Performance Improvement |
| --- | :---: | :---: | :---: | :---: |
| [Starlight](https://modrinth.com/mod/starlight) | Unknown | Fabric mod for completely rewriting the vanilla light engine. | Spottedleaf (PaperMC) | Both |
| [LazyDFU](https://www.curseforge.com/minecraft/mc-mods/lazydfu) | Mods that remove the DFU | LazyDFU is an optimization mod that makes the initialization of DataFixerUpper "lazy" | astei | Both |
| [Smooth Boot](https://www.curseforge.com/minecraft/mc-mods/smooth-boot) | Unknown | Optimize Minecraft loading performance to be smoother on low end systems and scale better on high end systems | UltimateBoomer | Both |
| [FerriteCore](https://www.curseforge.com/minecraft/mc-mods/ferritecore-fabric) | Unknown | This mod reduces the memory usage of Minecraft in a few different ways | malte0811 | Both |
| [Clumps](https://www.curseforge.com/minecraft/mc-mods/clumps) | Unknown | Clumps groups XP orbs together into a single entity to reduce lag when there are many in a small area. | jaredlll08 | Both |
| [Sodium](https://modrinth.com/mod/sodium) | Mods that utilize of the FRAPI[⁴](https://github.com/NordicGamerFE/usefulmods/tree/main#-some-of-the-mods-that-have-sodium-as-an-incompatibility-might-work-if-you-use-indium) | Sodium is a free and open-source rendering engine replacement for the Minecraft client that greatly improves frame rates, reduces micro-stutter, and fixes graphical issues in Minecraft | CaffeineMC | Client |
| [DashLoader](https://www.curseforge.com/minecraft/mc-mods/dashloader) (Dangerous) | Enhanced Block Entities | This mod launches minecraft faster by caching all of the content on first launch and then loading that cache on the next one | alphaqu | Client |
| [lazy-language-loader](https://www.curseforge.com/minecraft/mc-mods/lazy-language-loader) | Unknown | lazy-language-loader improves loading times when changing your language by only reloading the language instead of all the game resources! | chachylmao | Client |
| [Canvas](https://www.curseforge.com/minecraft/mc-mods/canvas-renderer) | Sodium | Advanced Rendering Engine for Fabric | grondag | Client |
| [Hydrogen](https://modrinth.com/mod/hydrogen) | Unknown | Reduces the memory usage of the game in more modded scenarios | CaffeineMC | Client |
| [EntityCulling](https://www.curseforge.com/minecraft/mc-mods/entityculling) | None | EntityCulling using async path-tracing to skip rendering Tiles/Entities that are not visible | tr9zw | Client |
| [Cull Leaves](https://www.curseforge.com/minecraft/mc-mods/cull-leaves) | Unknown | Adds culling to leaf blocks, providing a huge performance boost over vanilla. | Motschen | Client |
| [Enhanced Block Entities](https://modrinth.com/mod/ebe) | Sodium[⁴](https://github.com/NordicGamerFE/usefulmods/tree/main#-some-of-the-mods-that-have-sodium-as-an-incompatibility-might-work-if-you-use-indium), DashLoader | EBE is a mod which aims to increase the performance of block entity rendering, as well as offer customizability via resource packs. | FoundationGames | Client |
| [Entity Distance](https://modrinth.com/mod/entity-distance) | Unknown | Allows the user to adjust the (client) distance at which different entities render | capnkork | Client | 
| [Better Beds](https://www.curseforge.com/minecraft/mc-mods/better-beds) | Unknown | Removes the Block Entity Renderer from the bed and replaces it with the default minecraft model renderer. | Motschen | Client |
| [FastChest](https://www.curseforge.com/minecraft/mc-mods/fastchest) | Unknown | This mod helps by removing dynamic models from chests and making them render as static chunk geometry. | fake_domi | Client |
| [Better Biome Blend](https://www.curseforge.com/minecraft/mc-mods/better-biome-blend) | Sodium | Better Biome Blend is a mod  which accelerates the biome color blending algorithm. | FionaTheMortal | Client | 
| [Resolution Control](https://www.curseforge.com/minecraft/mc-mods/resolutioncontrol) | Unknown | ResolutionControl+ allows you to change Minecraft's render resolution separately from the HUD elements. | Ultimate Boomer | Client |
| [Smoke Suppresion](https://www.curseforge.com/minecraft/mc-mods/smoke-suppression) | Unknown | This is to prevent client-side lag and general annoyance when using large numbers of campfires in farms. | supersaiyansubtlety | Client |
| [Lithium](https://www.curseforge.com/minecraft/mc-mods/lithium) | None | Lithium is a general-purpose optimization mod for Minecraft which works to improve a number of systems without changing any behavior | CaffeineMC | Server |
| [Krypton](https://www.curseforge.com/minecraft/mc-mods/krypton) | Unknown | Krypton is a Minecraft mod designed for the Fabric mod loader that implements a suite of optimizations focused on the Minecraft networking stack | astei | Server |
| [C2ME](https://github.com/YatopiaMC/C2ME-fabric/releases) (***DANGEROUS***) | Tic-Tacs, + | A Fabric mod designed to improve the chunk performance of Minecraft. | YatopiaMC | Server |
| [Dimensional Threading](https://github.com/WearBlackAllDay/DimensionalThreading/releases) (Dangerous) | Unknown | Minecraft mod which optimizes the processing of multiple Dimensions, by assigning them independent threads | WearBlackAllDay | Server |
| [Alternate Current](https://modrinth.com/mod/alternate-current) (Dangerous) | Unknown | Alternate Current is an efficient and non-locational redstone dust implementation | Space Walker | Server |
| [FastFurnace](https://www.curseforge.com/minecraft/mc-mods/fast-furnace-for-fabric) | None | Similar to FastWorkbench, it caches the last recipe used, and checks this recipe first before re-scanning the entire registry | tfarecnim | Server |
| [Recipe Cache](https://www.curseforge.com/minecraft/mc-mods/recipe-cache) | FastFurnace, FastBench (?) | Caches recipe lookup for crafting and furnaces to lessen server lag caused by crafting stacks of items and large amounts of furnaces ticking | biom4st3r1 | Server | 
| [ServerCore](https://modrinth.com/mod/servercore) (Dangerous) | Unknown | A fabric mod that aims to optimize & add multiplayer features to the minecraft server. | Wesley1808 | Server |
| [Very Many Players](https://modrinth.com/mod/vmp-fabric) (Dangerous) | Unknown | Very Many Players, or VMP for short, is a Fabric mod designed to improve general server performance at high playercount without sacrificing vanilla functionality or behavior. | ishland | Server |



## Forge 1.17.X

| Name | Known Incompatibilities | Description | Author | Performance Improvement |
| --- | :---: | :---: | :---: | :---: |
| [FerriteCore](https://www.curseforge.com/minecraft/mc-mods/ferritecore) | Unknown | This mod reduces the memory usage of Minecraft in a few different ways | malte0811 | Both |
| [Clumps](https://www.curseforge.com/minecraft/mc-mods/clumps) | Unknown | Clumps groups XP orbs together into a single entity to reduce lag when there are many in a small area. | jaredlll08 | Both |
| [EntityCulling](https://www.curseforge.com/minecraft/mc-mods/entityculling) | None | EntityCulling using async path-tracing to skip rendering Tiles/Entities that are not visible | tr9zw | Client |
| [Better Fps - Render Distance](https://www.curseforge.com/minecraft/mc-mods/better-fps-render-distance) | Unknown | Better FPS Render Distance is a mod which adds a few performance improvements to increase fps. | someaddon | Client |
| [Better Biome Blend](https://www.curseforge.com/minecraft/mc-mods/better-biome-blend) | Probably any Sodium port | Better Biome Blend is a mod  which accelerates the biome color blending algorithm. | FionaTheMortal | Client | 
| [Get It Together, Drops!](https://www.curseforge.com/minecraft/mc-mods/get-it-together-drops) | Unknown | This mod adds two configuration options to control how dropped items combine on the ground. This can significantly improve performance in areas with lots of dropped items | bl4ckscor3 | Server |
| [Get It Together, Drops!](https://www.curseforge.com/minecraft/mc-mods/get-it-together-drops) | Unknown | This mod adds two configuration options to control how dropped items combine on the ground. This can significantly improve performance in areas with lots of dropped items | bl4ckscor3 | Server |
| [FastWorkbench](https://www.curseforge.com/minecraft/mc-mods/fastworkbench) | Unknown | This is a mod aimed at improving performance of all crafting-related functions. | 
Shadows_of_Fire | Server |
| [FastFurnace](https://www.curseforge.com/minecraft/mc-mods/fastfurnace) | Unknown | Similar to FastWorkbench, it caches the last recipe used, and checks this recipe first before re-scanning the entire registry. | Shadows_of_Fire | Server |
| [FastSuite](https://www.curseforge.com/minecraft/mc-mods/fastsuite) | Unknown | FastSuite is a mod about improving recipe performance, it improves upon all mods that use the JSON recipe system, rather than just a specific subset of recipes | Shadows_of_Fire | Server |
| [AI Improvements](https://www.curseforge.com/minecraft/mc-mods/ai-improvements)[⁵](https://github.com/NordicGamerFE/usefulmods/tree/main#-ai-improvements-newer-versions-114-dont-have-as-much-impact-as-the-older-versions-have-since-in-newer-versions-of-minecraft-a-lot-of-fixes-to-the-ai-are-implemented-sources-curseforge-page-faq-dev) | None | Simplified AI modification mod focused on performance and low-level modifications to AIs in the game | QueenOfMissiles | Server |

[![Home](https://i.imgur.com/zGuelkW.png)](https://github.com/NordicGamerFE/usefulmods/tree/main)
