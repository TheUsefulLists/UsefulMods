# Useful Mods
Note: Alkyaly has stopped maintaining their list, and they have given me the responsibility to maintain their list ([original list here](https://gist.github.com/alkyaly/02830c560d15256855bc529e1e232e88)).

A list of useful mods for most commonly-played versions.<br>

Any suggestions/complaints?<br>
Join our [discord](https://discord.gg/8nzHYhVUQS) or submit an issue (or a pull request fixing it!)

## NOTICE - Security vulnerability with 1.8 through 1.18
Read about the [Security Vulnerability information](https://www.minecraft.net/en-us/article/important-message--security-vulnerability-java-edition), and follow [this guide](https://www.creeperhost.net/wiki/books/minecraft-java-edition/page/mitigating-cve-2021-44228-in-minecraft) to fix it.

## Mods Under Consideration
Everything that is under consideration to be added is found [here](https://docs.google.com/document/d/127YtDboB7mQIH3SK8jd4d3_I7ur0LPHT46l9I1zRrwA/edit?usp=sharing).<br>
Keep in mind that nothing in the document is screened for harmful code (or malware). Download at your own caution.

## Version List - Performance Mods
| Version | Loaders |
| :-: | :---: |
| [1.18.x](Performance/Performance118.md) | Fabric & Forge |
| [1.17.x](Performance/Performance117.md) | Fabric & Forge |
| [1.16.x](Performance/Performance116.md) | Fabric & Forge |
| [1.15.x](Performance/Performance115.md) | Forge |
| [1.12.x](Performance/Performance112.md) | Forge |
| [1.8.9 and below](Performance/PerformanceOld.md) | Forge |

## Version List - Bugfixing Mods
| Version | WIP? | Loaders |
| :-----: | :--: | :-----: |
| [1.18.x](BugFixes/BugFixes118.md) | No | Fabric & Forge |
| [1.17.x](BugFixes/BugFixes117.md) | Yes | Fabric & Forge |
| [1.16.x](BugFixes/BugFixes116.md) | Yes | Fabric & Forge |
| [1.15.x](BugFixes/BugFixes115.md) | Yes | Forge |
| [1.12.x](BugFixes/BugFixes112.md) | Yes | Forge |
| [1.8.9 and below](BugFixes/BugFixesOld.md) | Yes | Forge |

## External Software (handy, fixes bugs, or enhances performance, alongside others)
| Theme |
| ----- |
| [Launchers](Software/SoftwareLaunchers.md) |
| [Bukkit, Spigot & ETC](Software/SoftwareBukkitSpigotETC.md) |
| [Graphical](Software/SoftwareGraphical.md) |
| [World Management](Software/SoftwareWorldManagement.md) |
| [Server Management](Software/SoftwareServerManagement.md) |

## Threat Levels
Threat levels are used alongside labels for a clearer understanding of the mod's danger.

| Level | Meaning |
| :---: | :-----: |
| 1 | Low chance to affect user |
| 2 | Low to medium chance to affect user |
| 3 | Medium chance to affect user |
| 4 | Medium to high chance to affect user |
| 5 | High chance to affect user |
| 6 | Very high chance to affect user |
| 7 | Will affect user |

## Labels
Labels are used to give you a better understanding of how a mod may act.

| Name | Meaning |
| :--: | :-----: |
| Alpha | Mod is in alpha and therefore might be unstable. |
| Unstable | Mod is unstable and may act unpredictably. |
| Corruption | Mod has a chance to corrupt save files. |
| Incompatible | Mod is incompatible with some mods. |
| Buggy | Mod is buggy. |
| Reverse Features | Mod takes away features for sake of performance or bugfixes. |
| Configuration Needed | Mod needs to be configured to act at its best. |

## Extra Information
You might find small numbers around the gist that look like this(¹,²,³,⁴,⁵,⁶) these are used to tell extra information.
&nbsp;

###### ¹ The mod should work if [Mixin-0-7-0-8-Compatibility](https://www.curseforge.com/minecraft/mc-mods/mixin-0-7-0-8-compatibility) is applied. 
###### ² Cull Particles isn't needed anymore in newer Forge versions, as it was implemented in Forge.
###### ³ Do not blame me if you didn't read this notice. *If you try to load a older world in a newer instance of the game, and you have one of these mods installed, bad things will happen*, make sure to uninstall the mod first.
###### ⁴ Some of the mods that have Sodium as an incompatibility, might work if you use [Indium](https://modrinth.com/mod/indium).
###### ⁵ AI Improvements newer versions (1.14+) don't have as much impact as the older versions have, since in newer versions of Minecraft, a lot of fixes to the AI are implemented ([Sources: Curseforge page FAQ, [Dev](https://media.discordapp.net/attachments/254806806516203520/831525756143534150/unknown.png)]).
###### ⁶ Halogen has issues with Forge's ExplosionEvent, see [sodium-forge#33](https://github.com/spoorn/sodium-forge/issues/33).
