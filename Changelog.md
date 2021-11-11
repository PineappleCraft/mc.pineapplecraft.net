# Changelog 11/11/21
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