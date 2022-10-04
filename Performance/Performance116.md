# Performance Mods

A list of performance-enhancing mods for 1.16.x forge/fabric versions.

Any suggestions/complaints?
Join our [discord](https://discord.gg/8nzHYhVUQS) or use the issues.

[![Home](https://i.imgur.com/zGuelkW.png)](/README.md)

## Fabric 1.16.X

| Name | Known Incompatibilities | Description | Author | Performance Improvement | [Label](/README.md/#labels) |
| --- | :---: | :---: | :---: | :---: | :---: |
| [Alternate Current](https://www.curseforge.com/minecraft/mc-mods/alternate-current) | Unknown | Alternate Current is an efficient and non-locational redstone dust implementation. | SpaceWalkerRS | Server | none |
| [Angerable Patch](https://www.curseforge.com/minecraft/mc-mods/angerable-patch) | Unknown | Fixes MC-192362 / MC-189565, which causes drastically large log file sizes and lag | Draylar | Client | none |
| [Better Beds](https://www.curseforge.com/minecraft/mc-mods/better-beds) | Unknown | Removes the Block Entity Renderer from the bed and replaces it with the default minecraft model renderer. | Motschen | Client | none |
| [Better Biome Blend](https://www.curseforge.com/minecraft/mc-mods/better-biome-blend) | Sodium | Better Biome Blend is a mod  which accelerates the biome color blending algorithm. | FionaTheMortal | Client | none |
| [C2ME](https://github.com/YatopiaMC/C2ME-fabric/releases)| Tic-Tacs, + | A Fabric mod designed to improve the chunk performance of Minecraft. | YatopiaMC | Server | Alpha (1) |
| [Canvas](https://www.curseforge.com/minecraft/mc-mods/canvas-renderer) | Sodium | Advanced Rendering Engine for Fabric | grondag | Client | Alpha (1) |
| [Cull Leaves](https://www.curseforge.com/minecraft/mc-mods/cull-leaves) | Unknown | Adds culling to leaf blocks, providing a huge performance boost over vanilla. | Motschen | Client | none |
| [DashLoader](https://www.curseforge.com/minecraft/mc-mods/dashloader) | Hydrogen, Enhanced Block Entities | This mod launches minecraft faster by caching all of the content on first launch and then loading that cache on the next one | alphaqu | Client | Incompatible (4) |
| [Dimensional Threading](https://github.com/WearBlackAllDay/DimensionalThreading/releases)| Unknown | Minecraft mod which optimizes the processing of multiple Dimensions, by assigning them independent threads | WearBlackAllDay | Server | none |
| [Dynamic FPS](https://modrinth.com/mod/dynamic-fps) | Unknown | Automatically reduces rendering speed when minecraft is not focused (to 1 FPS) or hidden (no renders at all). | juliand665 | Client | none |
| [Enhanced Block Entities](https://modrinth.com/mod/ebe) | Sodium[⁴](/README.md#-some-of-the-mods-that-have-sodium-as-an-incompatibility-might-work-if-you-use-indium), DashLoader | EBE is a mod which aims to increase the performance of block entity rendering, as well as offer customizability via resource packs. | FoundationGames | Client | none|
| [Entity Distance](https://modrinth.com/mod/entity-distance) | Unknown | Allows the user to adjust the (client) distance at which different entities render | capnkork | Client | none |
| [EntityCulling](https://www.curseforge.com/minecraft/mc-mods/entityculling) | None | EntityCulling using async path-tracing to skip rendering Tiles/Entities that are not visible | tr9zw | Client | none |
| [FastBench](https://www.curseforge.com/minecraft/mc-mods/fastbench-for-fabric) | None | This is a mod aimed at improving performance of all crafting-related functions. | tfarecnim | Server | none |
| [FastChest](https://www.curseforge.com/minecraft/mc-mods/fastchest) | Unknown | This mod helps by removing dynamic models from chests and making them render as static chunk geometry. | fake_domi | Client | none |
| [FastFurnace](https://www.curseforge.com/minecraft/mc-mods/fast-furnace-for-fabric) | Recipe Cache | Similar to FastWorkbench, it caches the last recipe used, and checks this recipe first before re-scanning the entire registry | tfarecnim | Server | none |
| [Fat Experience Orbs](https://www.curseforge.com/minecraft/mc-mods/fat-experience-orbs) | Unknown | This mod makes it so that nearby experience orbs merge together | NinjaPhenix | Server | none |
| [FerriteCore](https://www.curseforge.com/minecraft/mc-mods/ferritecore-fabric) | Unknown | This mod reduces the memory usage of Minecraft in a few different ways | malte0811 | Both | none |
| [Hopper Optimizations](https://github.com/2No2Name/hopperOptimizations) | Unknown | A mod that optimizes hoppers and their interactions with entities and inventories | 2No2Name | Server | none |
| [Hydrogen](https://modrinth.com/mod/hydrogen) | DashLoader | Reduces the memory usage of the game in more modded scenarios | CaffeineMC | Client | Alpha (1) |
| [Krypton](https://www.curseforge.com/minecraft/mc-mods/krypton) | Unknown | Krypton is a Minecraft mod designed for the Fabric mod loader that implements a suite of optimizations focused on the Minecraft networking stack | astei | Both | Alpha (1) |
| [Ksyxis](https://www.curseforge.com/minecraft/mc-mods/ksyxis) | Unknown | Speeds up your world loading by not loading nearby chunks every time. | VidTu | Both | Reverse Features (1) |
| [LazyDFU](https://www.curseforge.com/minecraft/mc-mods/lazydfu) | None | LazyDFU is an optimization mod that makes the initialization of DataFixerUpper "lazy" | astei | Both | none |
| [Lithium](https://www.curseforge.com/minecraft/mc-mods/lithium) | None | Lithium is a general-purpose optimization mod for Minecraft which works to improve a number of systems without changing any behavior | CaffeineMC | Server | none |
| [MCMT-Fabric](https://github.com/himekifee/MCMTFabric) | Carpet, Dimensional Threading | This is a mod, that attempts to multithread minecraft's tick execution. | himekifee | Server | Corruption (1) |
| [Mipmaplevel and Language Fix](https://modrinth.com/mod/mipmaplevelandlanguagefix) | Unknown | Makes changing Mipmaplevels and Language faster, by instead of doing a full reload, only reloading the respective part of the game. | KingContaria | Client | none |
| [Observable](https://modrinth.com/mod/observable) | Unknown | Shows what's lagging your world/server by profiling (tile) entities. | tasgon | Server | none |
| [Overworld Two](https://www.curseforge.com/minecraft/mc-mods/overworld-two) | Unknown | Optimization mod that generates overworld and nether terrain much faster than vanilla minecraft at the cost of breaking parity. | gegy1000, SuperCoder79 | Server | none |
| [Phosphor](https://www.curseforge.com/minecraft/mc-mods/phosphor) | Starlight | Phosphor is a Minecraft mod which works to optimize one of game's most inefficient areas, the lighting engine | CaffeineMC | Both | none |
| [Recipe Cache](https://www.curseforge.com/minecraft/mc-mods/recipe-cache) | FastFurnace, FastBench (?) | Caches recipe lookup for crafting and furnaces to lessen server lag caused by crafting stacks of items and large amounts of furnaces ticking | biom4st3r1 | Server | none |
| [Resolution Control+](https://github.com/UltimateBoomer/Resolution-Control/releases) | Unknown | ResolutionControl+ allows you to change Minecraft's render resolution separately from the HUD elements. | Ultimate Boomer | Client | Buggy (4) |
| [Smoke Suppresion](https://www.curseforge.com/minecraft/mc-mods/smoke-suppression) | Unknown | This is to prevent client-side lag and general annoyance when using large numbers of campfires in farms. | supersaiyansubtlety | Client | none |
| [Smooth Boot](https://www.curseforge.com/minecraft/mc-mods/smooth-boot) | Unknown | Optimize Minecraft loading performance to be smoother on low end systems and scale better on high end systems | UltimateBoomer | Both | none |
| [Sodium](https://www.curseforge.com/minecraft/mc-mods/sodium) | Mods that utilize of the FRAPI[⁴](/README.md#-some-of-the-mods-that-have-sodium-as-an-incompatibility-might-work-if-you-use-indium) | Sodium is a free and open-source rendering engine replacement for the Minecraft client that greatly improves frame rates, reduces micro-stutter, and fixes graphical issues in Minecraft | CaffeineMC | Client | none |
| [Starlight](https://github.com/PaperMC/Starlight/releases) | Phosphor | Fabric mod for completely rewriting the vanilla light engine. | Spottedleaf (PaperMC) | Both | none |
| [Tic-Tacs](https://github.com/Gegy/tic-tacs/releases) | C2ME | Tic-TACS is an experimental reimplementation of Minecraft's chunk loading engine | gegy | Server | Alpha (3) |
| [VanillaFix](https://github.com/DimensionalDevelopment/VanillaFix/releases) | Unknown | Bug fixes and optimizations for Minecraft | BoogieMonster1O1 (Dimensional Development) | Both | none |

## Forge 1.16.X

| Name | Known Incompatibilities | Description | Author | Performance Improvement | [Label](/README.md/#labels) |
| --- | :---: | :---: | :---: | :---: | :---: |
| [AI Improvements](https://www.curseforge.com/minecraft/mc-mods/ai-improvements)[⁵](/README.md#-ai-improvements-newer-versions-114-dont-have-as-much-impact-as-the-older-versions-have-since-in-newer-versions-of-minecraft-a-lot-of-fixes-to-the-ai-are-implemented-sources-curseforge-page-faq-dev) | None | Simplified AI modification mod focused on performance and low-level modifications to AIs in the game | QueenOfMissiles | Server | none |
| [APTweaks](https://www.curseforge.com/minecraft/mc-mods/adaptive-performance-tweaks) | Dynamic View (View Distance Feature), Clumps | Adaptive Performance Tweaks is a Minecraft Forge Mod which automatically adjust specific settings on the server and client side to allow a balanced TPS/FPS. | Kaworru | Server | none |
| [Better Biome Blend](https://www.curseforge.com/minecraft/mc-mods/better-biome-blend) | None | Better Biome Blend is a mod  which accelerates the biome color blending algorithm. | FionaTheMortal | Client | none |
| [Better Fps - Render Distance](https://www.curseforge.com/minecraft/mc-mods/better-fps-render-distance) | Unknown | Better FPS Render Distance is a mod which adds a few performance improvements to increase fps. | someaddon | Client | none |
| [C2ME](https://github.com/YatopiaMC/C2ME-forge/releases) | Unknown | A Forge mod designed to improve the chunk performance of Minecraft. | YatopiaMC | Server | Alpha (1) |
| [Clumps](https://www.curseforge.com/minecraft/mc-mods/clumps) | APTweaks, MCMT | Clumps groups XP orbs together into a single entity to reduce lag when there are many in a small area | jaredlll08 | Both | none |
| [DataFixerSlayer](https://www.curseforge.com/minecraft/mc-mods/datafixerslayer)[³](/README.md#-do-not-blame-me-if-you-didnt-read-this-notice-if-you-try-to-load-a-older-world-in-a-newer-instance-of-the-game-and-you-have-one-of-these-mods-installed-bad-things-will-happen-uninstall-the-mod-first) | Any other mod that also removes DFU | DataFixerSlayer prevents the DataFixerUpper (DFU) system from loading | Vazkii | Both | none |
| [Does It Tick?](https://www.curseforge.com/minecraft/mc-mods/does-it-tick) | Unknown | performance enhancing mod that limits entity ticking outside view distance | TeamDeusVult | Server | none |
| [DrawerFPS](https://www.curseforge.com/minecraft/mc-mods/drawerfps) | Unknown | Simple, efficient mod which lets you configure at which range Storage Drawers do render items to improve fps. | someaddon | Client | none |
| [Dynamic View](https://www.curseforge.com/minecraft/mc-mods/dynamic-view) | APTweaks | This is a small/light serverside utility mod to help balancing lag (TPS) and chunk view/load distance. | someaddon | Server | none |
| [Entity Culling](https://www.curseforge.com/minecraft/mc-mods/entity-culling) | None | Entity Culling is a small client-side performance core mod which improves the rendering of entities and tile entities. | meldexun | Client | none |
| [EntityCulling](https://www.curseforge.com/minecraft/mc-mods/entityculling) | None | EntityCulling using async path-tracing to skip rendering Tiles/Entities that are not visible | tr9zw | Client | none |
| [Entity Collision FPS Fix](https://www.curseforge.com/minecraft/mc-mods/entity-collision-fps-fix) | Unknown | Client Side mod that optimizes entity's on the render thread. | CorgiTaco | Client | none |
| [FastFurnace minus Replacement](https://www.curseforge.com/minecraft/mc-mods/fastfurnace-minus-replacement) | None | Similar to FastWorkbench, it caches the last recipe used, and checks this recipe first before re-scanning the entire registry. | tfarecnim | Server | none |
| [FastSuite](https://www.curseforge.com/minecraft/mc-mods/fastsuite) | Unknown | FastSuite is a mod about improving recipe performance, it improves upon all mods that use the JSON recipe system, rather than just a specific subset of recipes | Shadows_of_Fire | Server | none |
| [FastWorkbench minus Replacement](https://www.curseforge.com/minecraft/mc-mods/fastworkbench-minus-replacement) | None | This is a mod aimed at improving performance of all crafting-related functions. | tfarecnim | Server | none |
| [FerriteCore](https://www.curseforge.com/minecraft/mc-mods/ferritecore) | Unknown | This mod reduces the memory usage of Minecraft in a few different ways | malte0811 | Both | none |
| [Get It Together, Drops!](https://www.curseforge.com/minecraft/mc-mods/get-it-together-drops) | Unknown | This mod adds two configuration options to control how dropped items combine on the ground. This can significantly improve performance in areas with lots of dropped items | bl4ckscor3 | Server | none |
| [Halogen⁶](https://www.curseforge.com/minecraft/mc-mods/halogen) | Performant, Immersive Portals | A Forge port of Sodium | spoorn | Client | none |
| [Helium](https://www.curseforge.com/minecraft/mc-mods/hydrogen-reforged) | Create | Formerly known as Hydrogen Reforged, Helium is an unofficial port of Hydrogen to Forge. | someoneelsewastaken | Both | none |
| [Krypton Reforged](https://www.curseforge.com/minecraft/mc-mods/krypton-reforged) | Unknown | Krypton Reforged is a Forge port of Krypton a Minecraft mod designed for the Fabric mod loader that implements a suite of optimizations focused on the Minecraft networking stack | TeamDeusVult | Both | Alpha (1) |
| [Ksyxis](https://www.curseforge.com/minecraft/mc-mods/ksyxis) | Unknown | Speeds up your world loading by not loading nearby chunks every time. | VidTu | Both | Reverse Features (1) |
| [LazyDFU](https://www.curseforge.com/minecraft/mc-mods/lazy-dfu-forge) | Mods that remove the DFU | LazyDFU is an optimization mod that makes the initialization of DataFixerUpper "lazy" | Corgi_Taco | Both | none |
| [Log Begone](https://www.curseforge.com/minecraft/mc-mods/log-begone) | Unknown | Log Begone is a fork of [Shut Up Console by Bravarly](https://www.curseforge.com/minecraft/mc-mods/shut-up-console) that simply allows you to remove annoying logs. Can also help with performance if there is a lot of log spam | AzureDoomC | Server | Configuration Needed (7) |
| [MCMT](https://hatebin.com/swopimmvaw) | Immersive Portals, Performant, Clumps, ***+++*** | This is a mod, that *attempts* to multithread minecraft's tick execution. | jediminer543 | Server | Corruption (1) |
| [Magnesium](https://www.curseforge.com/minecraft/mc-mods/sodium-reforged)[⁸](https://github.com/TheUsefulLists/UsefulMods#-some-of-the-mods-that-have-magnesiumrubidium-as-an-incompatibility-might-work-if-you-use-calcium) | Oculus, Rubidium | Unofficial port of Sodium to Forge. | someoneelsewastaken | Client | none |
| [Magnesium/Rubidium Extras](https://www.curseforge.com/minecraft/mc-mods/magnesium-extras) | Unknown | Pairing this with Magnesium/Rubidium is highly recommended. Fixes many issues and is compatible with almost everything. | TeamDeusVult | Client | none |
| [Observable](https://modrinth.com/mod/observable) | Unknown | Shows what's lagging your world/server by profiling (tile) entities. | tasgon | Server | none |
| [Out of Sight](https://www.curseforge.com/minecraft/mc-mods/out-of-sight) | Unknown | Out of Sight simply stops modded tile entities from rendering if they are further than 24 blocks away | Corosus | Client | Reverse Features (1) |
| [Overworld Two](https://www.curseforge.com/minecraft/mc-mods/overworld-two-forge) | Unknown | Optimization mod that generates overworld and nether terrain much faster than vanilla minecraft at the cost of breaking parity. | Corgi_Taco, gegy1000, SuperCoder79 | Server | none |
| [Performant](https://www.curseforge.com/minecraft/mc-mods/performant) | Phosphophyllite, Resourceful Bees, + | Lightweight mod project which hugely improves performance and blocklag. | someaddon | Server | Incompatible (2) |
| [RoadRunner](https://www.curseforge.com/minecraft/mc-mods/roadrunner) | Performant | RoadRunner is an unofficial fork of the popular performance-enhancing Fabric mod Lithium by jellysquid3 for the Forge mod loader. | MaxNeedsSnacks | Server | none |
| [Rubidium](https://www.curseforge.com/minecraft/mc-mods/rubidium)[⁸](https://github.com/TheUsefulLists/UsefulMods#-some-of-the-mods-that-have-magnesiumrubidium-as-an-incompatibility-might-work-if-you-use-calcium) | Magnesium | Another unofficial fork of Sodium to Forge. Pairs well with [Oculus](https://www.curseforge.com/minecraft/mc-mods/oculus) so a user can have Sodium's performance improvements with shaders. | Asek3 | Client | none |
| [Saturn](https://www.curseforge.com/minecraft/mc-mods/saturn) | Unknown | Saturn is a free and open-source performance mod for Minecraft Forge designed to optimize Minecraft's memoy usage | AbdElAziz333 | Both | none |
| [Smooth Boot](https://www.curseforge.com/minecraft/mc-mods/smooth-boot-forge) | Unknown | Optimize Minecraft loading performance to be smoother on low end systems and scale better on high end systems | UltimateBoomer | Both | none |
| [Spawner Bug Fix](https://www.curseforge.com/minecraft/mc-mods/spawner-fix) | Unknown | This addresses a bug which causes lag in mods that create custom spawners. | Lupicus | Client | none |
| [Starlight](https://github.com/PaperMC/Starlight/releases) | Create, Sulfuric | Mod for completely rewriting the vanilla light engine. | Spottedleaf (PaperMC) | Both | none |
| [Starlight x Create](https://www.curseforge.com/minecraft/mc-mods/starlight-x-create) | Sulfuric | Mod for completely rewriting the vanilla light engine. | Spottedleaf(PaperMC), Create Patch by: AeiouEnigma, Curseforge Upload and 1.16 Maintained by SirOMGitsYOU | Both | none |
| [Sulfuric](https://www.curseforge.com/minecraft/mc-mods/phosphor-reforged) | Starlight | Unofficial port of Phosphor to Forge. | someoneelsewastaken | Both | none |
| [~~⠀⠀Cull Particles⠀⠀~~](https://www.curseforge.com/minecraft/mc-mods/cull-particles)[²](/README.md#-cull-particles-isnt-needed-anymore-in-newer-forge-versions-as-it-was-implemented-in-forge)| None | This mod increases fps by not rendering particles that the player can't see | tfarecnim | Client | none |
| [Radon](https://www.curseforge.com/minecraft/mc-mods/radon) | Unknown | Radon is an Unofficial Port of CaffeineMC's "Phosphor," made to work with Forge Mod Loader | Asek3 | Both | none |

[![Home](https://i.imgur.com/zGuelkW.png)](/README.md)
