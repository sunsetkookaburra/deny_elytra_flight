# Deny Elytra Flight

A tiny Minecraft datapack. No flying with elytra: unsets the glider data component once equipped.

With the new 1.21.2 glider data component, disabling elytra is able to be done cleanly with commands. This tiny datapack is optimised for performance by using a hidden advancement to only modify elytra upon being equipped, instead of checking every tick.

## Restoring Elytra

Run the following command once you've disabled the datapack to restore all elytra currently worn back to Vanilla behaviour:

```mcfunction
/item modify entity @a[nbt={equipment:{chest:{id:"minecraft:elytra"}}}] armor.chest {function: "minecraft:set_components", components: {"minecraft:glider": {}}}
```

## License

[Mozilla Public License 2.0](https://www.mozilla.org/en-US/MPL/2.0/)

Copyright (C) 2025 Oli Lenehan ~sunsetkookaburra
