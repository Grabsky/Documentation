---
title: Recipes
type: docs
weight: 2
icon: adjustments

toc: false
---
Everything you need to know about recipes and their JSON structure.

Place your `.json` recipes inside the `plugins/Recipes/recipes` folder, or any sub-folder within this directory. Plugin automatically search them recursively and add their relative path to the recipe key.

<br>

<div class="ent">
  <h4>Recipe Components</h4>
</div>

{{% steps %}}

#### Item
Item is an object that represents an item in the recipes. It can be used as an ingredient, input or as a result.
All properties except for `type` *or* `registered_items` are optional.
```jsonata
"type": "diamond_sword",
"amount": 1,
"name": "<green>Emerald Sword",
"lore": ["Line 1", "Line 2"],
"components": "[item_model=myresourcepack:emerald_sword]"
```
Custom items must first be registered using `/recipes register_item (identifier)` in-game command.
```jsonata
"registered_item": "ruby"
```

#### Tag
Tags, specifically type tags, may be described as groups of types. They're an actual vanilla feature and are commonly referenced in various parts of the game.

They can be used in all ingredient or input slots, but cannot be mixed together with different choice types.
When the input field of a smelting recipe is set to tag `mincraft:boats` and result is set to `coal_block`, this allows all types of boats to be smelted into a block of coal.

Please note that some tags, including those added or modified by data-packs, may not work due to API limitations.
```jsonata
"tag": "minecraft:logs"
```
List of all available tags for latest version of Minecraft can be found here:  
**https://minecraft.wiki/w/Item_tag_(Java_Edition)**

#### Recipe Choice
Choice represents set of **items** *or* a **tag**, which can be used in a specific ingredient or input slot.

Most ingredient or input slots are expected to consist of exactly one choice, which - if not tag - can be an array with multiple elements. Some recipe types may accept an array of choices.

```jsonata
"input": { "type": "minecraft:iron_axe", "components": "[damage=157]" }
```
```jsonata
"input": { "registered_item": "ruby" }
```
```jsonata
"input": [
    { "type": "minecraft:cod" },
    { "type": "minecraft:salmon" },
    { "registered_item": "raw_mackerel" },
    { "registered_item": "raw_shrimp" },
    { "registered_item": "raw_tuna" },
    { "registered_item": "raw_carp" },
    { "registered_item": "raw_koi" }
]
```
Tag choice can be used to select individual group of items. Recipe will compare items based on their type.
```jsonata
"input": { "tag": "minecraft:boats" }
```

#### Discover Trigger
Recipe discover trigger can make any recipe discoverable by players when they pick up an item.
This feature is optional and if left unspecified, the recipe will be automatically discovered and visible by default.
```jsonata
"discover": {
    "items": [
        { "type": "emerald" }
    ]
}
```

{{% /steps %}}

<br>

<!------  Crafting Shaped  ------->

<div class="ent">
  <h4>Crafting Shaped</h4>
  <div>
    {{< badge color="green" content="Crafting Table" >}}
    {{< badge color="green" content="Inventory" >}}
    {{< badge color="green" content="Crafter" >}}
  </div>
</div>

Represents a crafting recipe with shape in a crafting table, player inventory, and the crafter.

| Property      | Required | Decsription |
| :------------ | :------- | :---------- |
| `key`         | No       | Identifier of the recipe. Fallbacks to `<CONFIGURED_NAMESPACE>:<FILE_PATH>` and should be omitted unless you want to override vanilla, or other plugins' recipes. |
| `pattern`     | Yes      | Pattern is an array of exactly 2 or 3 elements, reflecting an inventory or crafting table grids. Each array entry must be exactly two or three chracters. |
| `pattern_key` | Yes      | Key to the pattern represented as characters mapped to recipe choice definitions. Each character must be mapped to exactly one recipe choice.             |
| `result`      | Yes      | Result item definition. |
| `discover`    | No       | Recipe discover trigger. |

```json {filename="plugins/Recipes/recipes/emerald_sword.json"}
{
    "type": "crafting_shaped",
    "pattern": [
        " E ",
        " E ",
        " S "
    ],
    "key": {
        "E": { "type": "emerald" },
        "S": [
            { "type": "stick" },
            { "type": "blaze_rod" }
        ]
    },
    "result": {
        "type": "diamond_sword",
        "amount": 1,
        "name": "Emerald Sword",
        "components": "[item_model=myresourcepack:emerald_sword]"
    },
    "discover": {
        "items": [
            { "type": "emerald" }
        ]
    }
}
```

<br>
<br>

<!------  Crafting Shapeless  ------->

<div class="ent">
  <h4>Crafting Shapeless</h4>
  <div>
    {{< badge color="green" content="Crafting Table" >}}
    {{< badge color="green" content="Inventory" >}}
    {{< badge color="green" content="Crafter" >}}
  </div>
</div>

Represents a shapeless crafting recipe in a crafting table, player inventory, and the crafter.

| Property      | Required | Decsription |
| :------------ | :------- | :---------- |
| `key`         | No       | Identifier of the recipe. Fallbacks to `<CONFIGURED_NAMESPACE>:<FILE_PATH>` and should be omitted unless you want to override vanilla, or other plugins' recipes. |
| `ingredients` | Yes      | List of recipe ingredients. Each list element is a recipe choice, which can be a single item definition or tag, or list of item definitions or tags. |
| `result`      | Yes      | Result item definition.  |
| `discover`    | No       | Recipe discover trigger. |

```json {filename="plugins/Recipes/recipes/charcoal_from_crafting.json"}
{
    "type": "crafting_shapeless",
    "ingredients": [
        { "tag": "minecraft:logs" },
        { "type": "flint_and_steel" }
    ],
    "result": { "type": "charcoal" },
    "discover": {
        "items": [
            { "tag": "minecraft:logs" },
            { "type": "flint_and_steel" }
        ]
    }
}
```

<br>
<br>

<!------  Smelting, Blasting, Smoking, Campfire Cooking  ------->

<div class="ent">
  <h4>Smelting</h4>
  <div>
    {{< badge color="orange" content="Furnace" >}}
    {{< badge color="orange" content="Blast Furnace" >}}
    {{< badge color="orange" content="Smoker" >}}
    {{< badge color="orange" content="Campfire" >}}
  </div>
</div>

Represents a smelting recipe in a regular furnace, blast furnace, smoker or campfire.

| Property       | Required | Decsription |
| :------------- | :------- | :---------- |
| `key`          | No       | Identifier of the recipe. Fallbacks to `<CONFIGURED_NAMESPACE>:<FILE_PATH>` and should be omitted unless you want to override vanilla, or other plugins' recipes. |
| `type`         | Yes      | Type of the smelting recipe. Can be either:<br> `smelting`, `blasting`, `smoking` or `campfire_cooking` |
| `input`        | Yes      | Input recipe choice. Can be a single item definition or tag, or list of item definitions or tags.       |
| `result`       | Yes      | Result item definition.                                                                                 |
| `experience`   | No       | Experience to award player after taking the smelting result. (Default: 0.0)                             |
| `cooking_time` | No       | Time required to cook this recipe. Measured in ticks. (Default: 200)                                    |
| `discover`     | No       | Recipe discover trigger.                                                                                |

```json {filename="plugins/Recipes/recipes/diamomnd_armor_to_diamond_from_smelting.json"}
{
    "type": "smelting",
    "input": [
        { "type": "diamond_helmet" },
        { "type": "diamond_chestplate" },
        { "type": "diamond_leggings" },
        { "type": "diamond_boots" }
    ],
    "result": { "type": "diamond" },
    "experience": 0.7,
    "cooking_time": 200,
    "discover": {
        "items": [
            { "type": "diamond_helmet" },
            { "type": "diamond_chestplate" },
            { "type": "diamond_leggings" },
            { "type": "diamond_boots" }
        ]
    }
}
```

<br>
<br>

<!------  Smithing  ------->

<div class="ent">
  <h4>Smithing</h4>
  <div>
    {{< badge color="purple" content="Smithing Table" >}}
  </div>
</div>

Represents an upgrading recipe in a smithing table.

| Property          | Required | Decsription |
| :---------------- | :------- | :---------- |
| `key`             | No       | Identifier of the recipe. Fallbacks to `<CONFIGURED_NAMESPACE>:<FILE_PATH>` and should be omitted unless you want to override vanilla, or other plugins' recipes. |
| `base`            | Yes      | Ingredient specifying an item to be upgraded. Can be a single item definition or tag, or list of item definitions or tags.       |
| `template`        | Yes      | Ingredient specifying an item to act as a template. Can be a single item definition or tag, or list of item definitions or tags. |
| `addition`        | Yes      | Ingredient specifying an item to be added. Can be a single item definition or tag, or list of item definitions or tags.          |
| `result`          | Yes      | Result item definition.                                                                                                          |
| `copy_components` | No       | Whether to copy the data components from the base item to the output. (Default: true)                                            |
| `discover`        | No       | Recipe discover trigger.                                                                                                         |

```json {filename="plugins/Recipes/recipes/diamond_pickaxe_from_smithing.json"}
{
    "type": "smithing",
    "base": { "type": "iron_pickaxe" },
    "template": { "type": "air" },
    "addition": { "type": "diamond" },
    "result": { "type": "diamond_pickaxe" },
    "discover": {
        "items": [
            { "type": "iron_pickaxe" }
        ]
    }
}
```

<br>
<br>

<!------  Stonecutting  ------->

<div class="ent">
  <h4>Stonecutting</h4>
  <div>
    {{< badge color="gray" content="Stonecutter" >}}
  </div>
</div>

Represents a recipe in a stonecutter.

| Property   | Required | Decsription |
| :--------- | :------- | :---------- |
| `key`      | No       | Identifier of the recipe. Fallbacks to `<CONFIGURED_NAMESPACE>:<FILE_PATH>` and should be omitted unless you want to override vanilla, or other plugins' recipes. |
| `input`    | Yes      | Input recipe choice. Can be a single item definition or tag, or list of item definitions or tags.       |
| `result`   | Yes      | Result item definition.                                                                                 |
| `discover` | No       | Recipe discover trigger.                                                                                |

```json {filename="plugins/Recipes/recipes/oak_stairs_from_stonecutting.json"}
{
    "type": "smelting",
    "input": { "type": "oak_log" },
    "result": {
        "type": "oak_stairs",
        "amount": 4
    },
    "discover": {
        "items": [
            { "type": "oak_log" }
        ]
    }
}
```