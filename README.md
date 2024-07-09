# Minecraft Stats Plugin 📊

Welcome to the Stats Plugin, enhancing your Minecraft server with detailed player statistics and an interactive GUI!

## Features 🌟

- **Stats GUI:** View player stats such as kills, deaths, playtime, money balance, placed and broken blocks, and mob kills in a convenient GUI.
  
- **Customizable Layout:** Easily customize the layout and appearance of the stats GUI using YAML configuration.
  
- **Integration with Vault:** Display player money balance using Vault economy integration.
  
- **Extendable:** Add custom items to the stats GUI for additional player information or server-specific data.

## Configuration Example 📝

### Stats GUI Configuration

```yaml
statsgui:
  title: "#2F6EFBViewing Stats from {player}"
  rows: 4
  items:
    kills:
      material: DIAMOND_SWORD
      displayname: "#FF0000Kills"
      lore:
        - "&fTotal Kills: #FF0000%plrstatics_player_kills%"
      slot: 10
    deaths:
      material: SKELETON_SKULL
      displayname: "#FF0000Deaths"
      lore:
        - "&fTotal Deaths: #FF0000%plrstatics_player_deaths%"
      slot: 11
    playtime:
      material: CLOCK
      displayname: "&ePlaytime"
      lore:
        - "&fPlaytime: &e%plrstatics_playtime_dh%"
      slot: 12
    money:
      material: GOLD_INGOT
      displayname: "&aMoney"
      lore:
        - "&fBalance: &a%vault_eco_balance_formatted%"
      slot: 13
    placedblocks:
      material: GRASS_BLOCK
      displayname: "&7Placed Blocks"
      lore:
        - "&fBlocks Placed: &7%plrstatics_placed_blocks%"
      slot: 14
    brokenblocks:
      material: IRON_PICKAXE
      displayname: "&7Broken Blocks"
      lore:
        - "&fBlocks Broken: &7%plrstatics_broken_blocks%"
      slot: 15
    mobkills:
      material: IRON_SWORD
      displayname: "&2Mob Kills"
      lore:
        - "&fMob Kills: &2%plrstatics_mob_kills%"
      slot: 16
  custom_items:
    custom_item1:
      material: AMETHYST_SHARD
      displayname: "#FF00ECShards"
      lore:
        - "&fShards: #FF00EC%vault_eco_balance_formatted%"
        - "&fEdit or Remove this Line in plugins/ZenCore/config.yml"
      slot: 19
```


