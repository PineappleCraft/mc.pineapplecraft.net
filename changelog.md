# PineappleCraft Changelog

## Proxy Changelog: 29/06/2022
* Updated WaterFall to 1.19-497
* * *

## Server Changelog: 18/04/2022
* Disabled EssentialsProtect preventing fire spread and lava flow above a certain height.
* Completely disabled EssentialsProtect in general as well.
* Added VanishNoPacket for Admins
* Additional permission changes for Admin and SuperAdmin
* * *

## Changelog: 4/4/2022
* Waterfall-BungeeCord: Updated Waterfall bridge docker container
  * reset locations.yml to force everyone to use the new server names
  * updated config.yml by adding legacy domain mc.explodingpineapple.net pointing at smp.pineapplecraft.net
* * *

## Changelog: 23/03/2022
* Updated a number of plugins and replaced 3 plugins. [here](plugin-changelog.md)
* Had an issue with dying not being able to recover items from grave, not being able to rollback inventory or restore grave with command, and to polish that all off their was no backup for that time (Luckily it happen to me and I was very very early game so no harm done.)
  * The [gravy](https://www.spigotmc.org/resources/gravy.45288/) plugin wasn't working correctly due to not being up to date with 1.18 and had to be replaced with [Graves](https://www.spigotmc.org/resources/graves.74208/)
  * The [InventoryRollback](https://www.spigotmc.org/resources/inventory-rollback.48074/) plugin was giving errors in the server console whenever trying to restore any backups so I replaced it with [InventoryRollbackPlus](https://www.spigotmc.org/resources/inventory-rollback-plus-1-8-1-18-x.85811/)
  * Removed [ServerRestorer]() even though it was still working it hadn't seen an update in some time, and was also redundant because DriveBackupV2 can do the same thing (now that it's configured correctly)
  * Added [eBackup](https://www.spigotmc.org/resources/ebackup-simple-and-reliable-backups-for-your-server-supports-ftp-sftp.69917/) Probably not actually needed, but thought I'd add it just incase the worst happens.
  * Naturally due to all these changes theirs been a number of permission updates to the server although these won't be the last because the permissions need an overhaul.
* Changed the config on TimeIsMoney to only give out rewards to non-afk players every hour instead of every minecraft day (10 minutes).
* Updated resource pack with support for 1.18.
* * *

## Changelog 15/03/22
* Moved all future plugin updates to a new [place](plugin-changelog.md)
* Finally completed updating the server to 1.18.2 [Read more here](https://discord.com/channels/447671375012823069/590190368725925898/952977353582186556)
* Server won't be online straight away as mentioned in the above message.

* * *

## Changelog 2/12/21
* Changed LWC config to not auto apply protections, all protections must now be manually applied.
* Various small config changes to a number of plugins.

* * *

## Changelog 23/11/21
* Updated [HolidayHunt](https://www.spigotmc.org/resources/holidayhunt-christmas-game.97167/)
* Updated [Towny](https://www.spigotmc.org/resources/towny-advanced.72694/)
* Added [Residence](https://www.spigotmc.org/resources/residence-1-7-10-up-to-1-17.11480/) 
  * [Free Version](http://zrips.net/Residence/)
  * Added Dependecy [CMILib](https://www.spigotmc.org/resources/cmilib.87610/)
* Added [dynmap-residence](https://www.spigotmc.org/resources/dynmap-residence.90206/)
* Attempted to add [Live-Atlas](https://www.spigotmc.org/resources/liveatlas-a-dynmap-pl3xmap-frontend-for-the-modern-web.86939/)
* Added QuickShop addon [QuickShopList](https://www.spigotmc.org/resources/quickshop-addon-quickshoplist.82143/)

* * *

## Changelog 22/11/21
* Added [Shopkeepers](https://www.spigotmc.org/resources/shopkeepers.80756/)
* Added [PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/)
* Added [ChestCommands](https://dev.bukkit.org/projects/chest-commands)
* Added [DriveBackupV2](https://www.spigotmc.org/resources/drivebackupv2.79519/)
* Added [Essentials WarpGUI](https://www.spigotmc.org/resources/essentials-warp-gui-opensource.13571/)
* Added [HolidayHunt](https://www.spigotmc.org/resources/holidayhunt-christmas-game.97167/)
* Updated Permissions

* * *

## Changelog 17/11/21
* Reset Towny again... Turns out world settings only apply to a world at first install of Towny
  * Setup Pineappleville and Kingdom of Pineapple using the Exploding Pineapple Minecraft account for a public hub/shopping district in the future.
* Removed Chunkmaster plugin
* Added Advanced Portals Plugin as a possible replacement to WarpSystem
* Fix respawns by changing respawn-at-home in the essentials config from false to true.
* Possible other changes that I've forgotten, I'll add them as I remember

* * *

## Changelog 16/11/21
* Removed Claimblocks Plugin
* Added Shulker kit that grants 2 shulker shells and is only useable every 24 hours, Costs $1000
* Added Time Is Money plugin that adds a ATM GUI and gives players money for the time they're online playing.

* * *

## Changelog 11/11/21
* Regenerated a ton of chunks around everyone's bases to update them to include 1.17 generation with:
  * deepslate
  * calcite
  * amathyest geodes
  * glow lichen
  * dripstone
  * copper ore
(Basically anything that generates in 1.17.)
* moved world border from 3000 to 1500 until 1.18 comes out (might do a similar chunk regeneration when 1.18 comes out)
* Added more plugins, 
  * [AcoWorth](https://www.spigotmc.org/resources/acoworth.74173/)
  * [AsyncWorldEdit](https://www.spigotmc.org/resources/asyncworldedit.327/)
  * AsyncWorldEditBossBar
  * BlocksHub
  * Chunky and ChunkyBorder
  * Citizens
  * ClaimBlocks
  * ConsoleSpamFix
  * LandClaim
  * mcMMO
  * OpenINV
  * QuickShop
* Changed mcMMO config to use modern levelup mode as to not spam chat with level up messages.
* Change gravy config to allow for creating a users grave without the need for a token
* Updated the Essentials [Worth.json](https://gist.github.com/KadeWolfe/d8a8812564f2e80c20cb7a303ed19543), items.json files
* Reset Towny configs and database to default and setup the config from scratch again (This means you'll have to create your towns again, but hopefully now their should be less problems. or alternatively use one of the other land claim plugins)
* Updated Vanillatweaks Texture packs and updated and removed some of the Datapacks.
* [Changed bukkit.yml, spigot.yml, paper.yml to apply some server optimisations.](https://www.spigotmc.org/threads/guide-server-optimization%E2%9A%A1.283181/)
* Changed ServerRestorer config from 10gb to 50gb (Although it seems to be getting reset after a server reboot)

* * *

## 13/03/2020:
- Updated Server to Minecraft 1.17.2 and PaperMC-132
- Reset World for a fresh start, Using Seed WLLBYUG (Same seed used for HermitCraft Season 7)
- Added Custom Vanilla Tweaks Datapack, you can download it manually from here https://vanillatweaks.net/share/#rDeLYa


* * *
