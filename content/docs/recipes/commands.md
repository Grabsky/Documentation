---
title: Commands
type: docs
weight: 2

toc: false
---

List of all available commands with descriptions, permissions and a couple of examples.

<br>
<br>
<br>

<!------  Recipes > Reload  ------->

<h4 id="help" style="display:flex; justify-content:space-between;">
  <div style="float:left">Reload</div>
  <div style="float:right">{{< badge content="Management">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Reloads recipes, items and the configuration file.

<u>**Syntax**</u>  
`/recipes reload`

<u>**Permission**</u>  
`recipes.command.reload`

<br>
<br>

<!------  Recipes > List Recipes  ------->

<h4 id="help" style="display:flex; justify-content:space-between;">
  <div style="float:left">List Recipes</div>
  <div style="float:right">{{< badge content="Management">}} {{< badge content="Recipes" color="green">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Lists all recipes added, or overridden by this plugin.

<u>**Syntax**</u>  
`/recipes list_recipes`

<u>**Permission**</u>  
`recipes.command.list_recipes`

<br>
<br>

<!------  Recipes > List Items  ------->

<h4 id="help" style="display:flex; justify-content:space-between;">
  <div style="float:left">List Items</div>
  <div style="float:right">{{< badge content="Management">}} {{< badge content="Custom Items" color="yellow">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Lists all registered custom items.

<u>**Syntax**</u>  
`/recipes list_items`

<u>**Permission**</u>  
`recipes.command.list_items`

<br>
<br>

<!------  Recipes > Register Item  ------->

<h4 id="help" style="display:flex; justify-content:space-between;">
  <div style="float:left">Register Item</div>
  <div style="float:right">{{< badge content="Management">}} {{< badge content="Custom Items" color="yellow">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Registers item currently held in the main hand as a custom item.  
Registered items can be referenced in recipes via `registered_item` property.

<u>**Syntax**</u>  
`/recipes register_item (identifier)`

<u>**Permission**</u>  
`recipes.command.register_item`

<br>
<br>

<!------  Recipes > Unregister Item  ------->

<h4 id="help" style="display:flex; justify-content:space-between;">
  <div style="float:left">Unregister Item</div>
  <div style="float:right">{{< badge content="Management">}} {{< badge content="Custom Items" color="yellow">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Unregisters custom item with given identifier.

<u>**Syntax**</u>  
`/recipes unregister_item (identifier)`

<u>**Permission**</u>  
`recipes.command.unregister_item`

<br>
<br>

<!------  Recipes > Give Item  ------->

<h4 id="help" style="display:flex; justify-content:space-between;">
  <div style="float:left">Give Item</div>
  <div style="float:right">{{< badge content="Management">}} {{< badge content="Custom Items" color="yellow">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Gives specified custom item to the target.

<u>**Syntax**</u>  
`/recipes give_item (target) (identifier) [amount]`

<u>**Permission**</u>  
`recipes.command.give_item`

<br>
<br>

