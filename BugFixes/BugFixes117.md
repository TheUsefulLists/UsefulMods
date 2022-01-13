# Bugfixing Mods
A list of bugfix mods for 1.17.x forge/fabric versions.

Any suggestions/complaints?<br>
Join our [discord](https://discord.gg/8nzHYhVUQS) or use the issues.<br><br>

[![Home](https://i.imgur.com/zGuelkW.png)](https://github.com/NordicGamerFE/usefulmods/blob/main/README.md)

## Fabric 1.17.X

| Name | Known Incompatibilities | Description | Author | Bugfixing |
| --- | :---: | :---: | :---: | :---: |
| [Advancements Debug](https://www.curseforge.com/minecraft/mc-mods/advancements-debug) <br>(use 1.18 version) | Unknown | This little mod rewrites one function of the advancements logic to make advancements checking faster, and use less recursion. It should prevent StackOverflowErrors with advancements. | thetechnici4n | Client |
| [AntiGhost](https://www.curseforge.com/minecraft/mc-mods/antighost) | Unknown | Generally, the only way to fix this is relogging, or porting away and back, to unload and re-load the chunks. This mod asks the server to resend all blocks around the player when you type /ghost, within a 4 block radius cube, thus making relogging unneccesary. Or, just press the G key. | Giselbaer | Client |
| [Carpet Fixes](https://www.curseforge.com/minecraft/mc-mods/carpet-fixes) | Unknown | Fabric Carpet extension mod which attempts to fix as many vanilla Minecraft bugs as possible | FX_PR0CESS | Server |
| [CleanCut](https://www.curseforge.com/minecraft/mc-mods/cleancut) | Unknown | Attack enemies through obstructions! | Rongmario | Client |
| [Chat Lag Fix](https://www.modrinth.com/mod/chat-lag-fix) | Unknown | Fixes Minecraft client lag from receiving chat messages | adryd | Client |
| [Erroring Entity Remover](https://www.curseforge.com/minecraft/mc-mods/erroring-entity-remover) (Dangrous) | Unknown | This mod removes entities that throw errors and crash the game while ticking. Warning: Use at your own risk. This should generally be used as a last resort, and if the crash is clearly caused by a mod, you should report it so the author can fix it. Not Enough Crashes is good at identifying what mods might be causing crashes, and I recommend using it first then using this if the problem continues. | The_Fireplace | Both |
| [NetherPortalFix](https://www.curseforge.com/minecraft/mc-mods/netherportalfix-fabric) | Unknown | Ever played on a multiplayer server, built near other players and when returning from the Nether, surprisingly found yourself in another player's base? It's because of the 8:1 block ratio between the Nether and the Overworld. It's really weird though that you enter a portal in the overworld, and then when going back through where you came, come out of a different portal in the overworld. This mod fixes that issue. | BlayTheNinth | Server |
| [Night Vision flash be gone](https://www.curseforge.com/minecraft/mc-mods/night-vision-flash-be-gone) <br>(use 1.18 version) | Unknown | Fixes night vision flashing | AshIndigo | Client |
| [No Null Processors](https://www.curseforge.com/minecraft/mc-mods/no-null-processors) | Unknown | Have you been trying to pre-generate large areas of your world with pregenerator mods and keep randomly crashing with this error?<br><br> If so, congrats! You found a really wacky bug in 1.18 Minecraft! This mod aims to fix that.  | telepathicgrunt | Server |
| [Why Am I on Fire?](https://www.curseforge.com/minecraft/mc-mods/why-am-i-on-fire) <br>(use 1.18 version) | Unknown | Hides the obstructive fire overlay when it's not needed. | Ellivers | Both |
| [XL Packets Fabric](https://www.curseforge.com/minecraft/mc-mods/xl-packets-fabric) | Unknown | Fixes https://bugs.mojang.com/browse/MC-185901 by raising the packet size limit from 2MB to 2GB, so that servers with large datapacks, packets, etc don't kick the client. | tfarecnim | Both |


#### Notes
* Mods marked as "*use 1.18 version*" also work on 1.17.x , despite having only 1.16 and 1.18 releases in curseforge, no workarounds needed : install them like any other mods and your fabric loader won't complain about missing dependencies
* Mods marked as "*Dangerous*" might be unstable, and cause some unexpected behaviour.


## Forge 1.17.X

| Name | Known Incompatibilities | Description | Author | Bugfixing |
| --- | :---: | :---: | :---: | :---: |
| [Connectivity](https://www.curseforge.com/minecraft/mc-mods/connectivity) | Unknown | Lightweight mod which solves several connection problems like DecoderException, Packet size larget than X bytes, Payload too large and more. | someaddon | Both |
| [CleanCut](https://www.curseforge.com/minecraft/mc-mods/cleancut) | Unknown | Attack enemies through obstructions! | Rongmario | Client |
| [FlickerFix](https://www.curseforge.com/minecraft/mc-mods/flickerfix) | Unknown | By default, when the night vision effect goes below 10 seconds, the screen starts flickering. This mod replaces that behavior with a fast fade-out at 1 second remaining duration. |  MutantGumdrop | Client |
| [No Null Processors](https://www.curseforge.com/minecraft/mc-mods/no-null-processors) | Unknown | Have you been trying to pre-generate large areas of your world with pregenerator mods and keep randomly crashing with this error?<br><br> If so, congrats! You found a really wacky bug in 1.18 Minecraft! This mod aims to fix that.  | telepathicgrunt | Server |

[![Home](https://i.imgur.com/zGuelkW.png)](https://github.com/NordicGamerFE/usefulmods/blob/main/README.md)
