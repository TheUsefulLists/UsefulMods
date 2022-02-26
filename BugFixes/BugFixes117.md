# Bugfixing Mods
A list of bugfix mods for 1.17.x forge/fabric versions.

Any suggestions/complaints?<br>
Join our [discord](https://discord.gg/8nzHYhVUQS) or use the issues.<br><br>

[![Home](https://i.imgur.com/zGuelkW.png)](/README.md)

## Fabric 1.17.X

| Name | Known Incompatibilities | Description | Author | Bugfixing | [Label](/README.md#labels) |
| --- | :---: | :---: | :---: | :---: | :---: |
| [Advancements Debug](https://www.curseforge.com/minecraft/mc-mods/advancements-debug)[^1] | Unknown | Rewrites one function of the advancements logic to make advancements checking faster, and use less recursion. | thetechnici4n | Client | none |
| [AntiGhost](https://www.curseforge.com/minecraft/mc-mods/antighost) | Unknown | Removes all ghost blocks whithin a 4 block radius cube with press of a configurable key. | Giselbaer | Client | none |
| [Carpet Fixes](https://www.curseforge.com/minecraft/mc-mods/carpet-fixes) | Unknown | Fabric Carpet extension mod which attempts to fix as many vanilla Minecraft bugs as possible | FX_PR0CESS | Server | none |
| [Chat Lag Fix](https://www.modrinth.com/mod/chat-lag-fix) | Unknown | Fixes Minecraft client lag from receiving chat messages | adryd | Client | none |
| [Dynamic FPS](https://modrinth.com/mod/dynamic-fps) | Unknown | Fixes a bug in Vanilla Minecraft that makes it take much more performance in the background than it should. | juliand665 | Client | none | 
| [Erroring Entity Remover](https://www.curseforge.com/minecraft/mc-mods/erroring-entity-remover)| Unknown | Removes entities that throw errors and crash the game while ticking. | The_Fireplace | Both | Unstable (2) |
| [FastOpenLinksAndFolders](https://www.curseforge.com/minecraft/mc-mods/fastopenlinksandfolders) | Stops the game from freezing when opening external links or folders | altrisi | Client | none |
| [NetherPortalFix](https://www.curseforge.com/minecraft/mc-mods/netherportalfix-fabric) | Unknown | Keeps track of what portals a player went through in order to ensure correct destinations when the player is going back through the same portals. | BlayTheNinth | Server | none |
| [Night Vision flash be gone](https://www.curseforge.com/minecraft/mc-mods/night-vision-flash-be-gone)[^1] | Unknown | Fixes night vision flashing | AshIndigo | Client | none |
| [No Null Processors](https://www.curseforge.com/minecraft/mc-mods/no-null-processors) | Unknown | Fixes crashing when trying to pre-generate large areas of a world. | telepathicgrunt | Server | none |
| [ToolTipFix](https://www.curseforge.com/minecraft/mc-mods/tooltipfix) | Unknown | Stops tooltips that are too large to fit on the screen from running off the screen | Kryptonaught | Client | none |
| [Why Am I on Fire?](https://www.curseforge.com/minecraft/mc-mods/why-am-i-on-fire)[^1] | Unknown | Hides the obstructive fire overlay when it's not needed. | Ellivers | Both | none |
| [XL Packets Fabric](https://www.curseforge.com/minecraft/mc-mods/xl-packets-fabric) | Unknown | Fixes https://bugs.mojang.com/browse/MC-185901 by raising the packet size limit from 2MB to 2GB, so that servers with large datapacks, packets, etc don't kick the client. | tfarecnim | Both | none |

## Forge 1.17.X

| Name | Known Incompatibilities | Description | Author | Bugfixing | [Label](/README.md#labels) |
| --- | :---: | :---: | :---: | :---: | :---: |
| [AntiGhost](https://www.curseforge.com/minecraft/mc-mods/antighost) | Unknown | Removes all ghost blocks whithin a 4 block radius cube with press of a configurable key. | Giselbaer | Client | none |
| [AttributeFix](https://www.curseforge.com/minecraft/mc-mods/attributefix) | Unknown | Removes attribute caps, which can cause unintended behavior with some mods | DarkhaxDev | Server | none |
| [Bee Fix](https://www.curseforge.com/minecraft/mc-mods/bee-fix) | Unknown | This mod fixes MC-229321 : Bees Can Despawn This bug causes multiple issues that cause bees to despawn or fail to be saved under different edge cases. Also fixes MC-168329 : Bees refuse to leave hive in end/nether. | lupicus | Server | none |
| [Connectivity](https://www.curseforge.com/minecraft/mc-mods/connectivity) | Randompatches | Lightweight mod which solves several connection problems like DecoderException, Packet size larget than X bytes, Payload too large and more. | someaddon | Both | none |
| [FlickerFix](https://www.curseforge.com/minecraft/mc-mods/flickerfix) | Unknown | By default, when the night vision effect goes below 10 seconds, the screen starts flickering. This mod replaces that behavior with a fast fade-out at 1 second remaining duration. |  MutantGumdrop | Client | none |
| [No Null Processors](https://www.curseforge.com/minecraft/mc-mods/no-null-processors) | Unknown | Fixes crashing when trying to pre-generate large areas of a world.  | telepathicgrunt | Server | none |
| [Potion ID Packet Fixer](https://www.curseforge.com/minecraft/mc-mods/potion-id-packet-fixer) | Unknown | If you have more than 255 potion effects registered, the client will receive incorrect information for potion effects above ID 255, due to an issue with vanilla packets. This mod fixes that issue. | stepcros | Both | none |

[![Home](https://i.imgur.com/zGuelkW.png)](/README.md)

[^1]: These mods work on 1.17.x , despite having only 1.16 and 1.18 releases in curseforge, no workarounds needed. Install them like any other mods and your fabric loader won't complain about missing dependencies.
