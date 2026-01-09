**Since Stellarity at its core is a datapack, this addon work by overwriting data/stellarity/loot_table/item/weapons/[weapon_name].json**
Therefore you need the pack to load after Stellarity, if Stellarity is installed as a mod this will always work, if it isn't then you should install Stellarity first, then this pack right after.

This addon will only add the Better Combat features to items obtained after installing the addon, if you obtained an item before installing the addon you need to manually update it with a command, I'll drop a tool for this later.

You can changes the Better Combat preset pretty easily if you want to, so you can do it yourself in like 30 seconds if the pack goes unmaintained / outdated by modifying the files.
This is what you need to look for in the files
```
            {
              "function": "minecraft:set_components",
              "components": {
                "minecraft:item_model": "stellarity:harvester",
                "bettercombat:preset_id": "bettercombat:sword",
                "minecraft:custom_data": {
                  "stellarity:item": "harvester",
                  "stellarity:harvester": {
                    "damage": 0,
                    "abilities": []
                  }
```
The line "bettercombat:presetid": "bettercombat:sword" is the preset settings, simply change sword to other presets found here:
https://github.com/ZsoltMolnarrr/BetterCombat/tree/1.21.11/common/src/main/resources/data/bettercombat/weapon_attributes

For example, you want the harvester to be a 2 handed greatsword, just change the bettercombat:sword to bettercombat:claymore, simple!


Also I had full permission to publish this please don't sue me
<img width="1101" height="122" alt="image" src="https://github.com/user-attachments/assets/388158b9-6113-4b7e-be3c-083742d9ec94" />
