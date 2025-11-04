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

<!------  Display > Help  ------->

<h4 id="help" style="display:flex; justify-content:space-between;">
  <div style="float:left">Help</div>
  <div style="float:right">{{< badge content="Management">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Shows list of available commands.

<u>**Syntax**</u>  
`/display help [page]`

<u>**Permission**</u>  
`displayentities.command.display.help`

<br>
<br>

<!------  Display > Create  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Create</div>
  <div style="float:right">{{< badge content="Management">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Creates display of the specified type. Type can be **text**, **item**, **block**, **interaction** or **mannequin**. 

<u>**Syntax**</u>  
`/display create (type) (name)`

<u>**Permission**</u>  
`displayentities.command.display.create`

<br>
<br>

<!------  Display > Delete  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Delete</div>
  <div style="float:right">{{< badge content="Management">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Deletes specified entity from the world. This action is irreversible.

<u>**Syntax**</u>  
`/display delete (display)`

<u>**Permission**</u>  
`displayentities.command.display.delete`

<br>
<br>

<!------  Display > Clone  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Clone</div>
  <div style="float:right">{{< badge content="Management">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Clones specified display to a new one.

<u>**Syntax**</u>  
`/display clone (display) (name)`

<u>**Permission**</u>  
`displayentities.command.display.clone`

<br>
<br>

<!------  Display > Respawn  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Respawn</div>
  <div style="float:right">{{< badge content="Management">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Respawns specified display. Use it after adding placeholders or modifying placeholder refresh interval.

<u>**Syntax**</u>  
`/display respawn (display)`

<u>**Permission**</u>  
`displayentities.command.display.respawn`

<br>
<br>

<!------  Display > Teleport  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Teleport</div>
  <div style="float:right">{{< badge content="Management">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Teleports you to the specified display.

<u>**Syntax**</u>  
`/display teleport (display)`

<u>**Permission**</u>  
`displayentities.command.display.teleport`

<br>
<br>

<!------  Display > Export  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Export</div>
  <div style="float:right">{{< badge content="Management">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Exports specified display to a file.

<u>**Syntax**</u>  
`/display export (display)`

<u>**Permission**</u>  
`displayentities.command.display.export`

<br>
<br>

<!------  Display > Import  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Import</div>
  <div style="float:right">{{< badge content="Management">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Imports specified file to a new display.

<u>**Syntax**</u>  
`/display import (file) (name)`

<u>**Permission**</u>  
`displayentities.command.display.import`

<br>
<br>

<!------  Display > Edit > Scale  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Scale</div>
  <div style="float:right">{{< badge color="purple" content="Text">}} {{< badge color="blue" content="Item">}} {{< badge color="green" content="Block">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies scale of the specified display.

<u>**Syntax**</u>  
`/display edit (display) scale (x) (y) (z)`

<u>**Permission**</u>  
`displayentities.command.display.edit.scale`

<br>
<br>

<!------  Display > Edit > View Range  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; View Range</div>
  <div style="float:right">{{< badge color="purple" content="Text">}} {{< badge color="blue" content="Item">}} {{< badge color="green" content="Block">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies view range of the specified display. Range must be a value between **0.0** and **1.0**.

<u>**Syntax**</u>  
`/display edit (display) view_range (range)`

<u>**Permission**</u>  
`displayentities.command.display.edit.view_range`

<br>
<br>

<!------  Display > Edit > Billboard  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Billboard</div>
  <div style="float:right">{{< badge color="purple" content="Text Display">}} {{< badge color="blue" content="Item">}} {{< badge color="green" content="Block">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies billboard of the specified text display. Billboard can be **fixed**, **center**, **horizontal** or **vertical**.

<u>**Syntax**</u>  
`/display edit (display) billboard (billboard)` 

<u>**Permission**</u>  
`displayentities.command.display.edit.billboard`

<br>
<br>

<!------  Display > Edit > Brightness  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Brightness</div>
  <div style="float:right">{{< badge color="purple" content="Text">}} {{< badge color="blue" content="Item">}} {{< badge color="green" content="Block">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies brightness of the specified display. Brightness must be a value between 0 and 15.

<u>**Syntax**</u>  
`/display edit (display) brightness (block | sky) (brightness)`  

<u>**Permission**</u>  
`displayentities.command.display.edit.brightness`

<br>
<br>

<!------  Display > Edit > Rotate X  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Rotate X</div>
  <div style="float:right">{{< badge color="purple" content="Text">}} {{< badge color="blue" content="Item">}} {{< badge color="green" content="Block">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Rotates specified display for specified amount of degrees around X axis. Works only when billboard is fixed.

<u>**Syntax**</u>  
`/display edit (display) rotate_x (degrees)`  

<u>**Permission**</u>  
`displayentities.command.display.edit.rotate_x`

<br>
<br>

<!------  Display > Edit > Rotate Y  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Rotate Y</div>
  <div style="float:right">{{< badge color="purple" content="Text">}} {{< badge color="blue" content="Item">}} {{< badge color="green" content="Block">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Rotates specified display for specified amount of degrees around Y axis. Works only when billboard is fixed.

<u>**Syntax**</u>  
`/display edit (display) rotate_y (degrees)`  

<u>**Permission**</u>  
`displayentities.command.display.edit.rotate_y`

<br>
<br>

<!------  Display > Edit > Move To  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Move To</div>
  <div style="float:right">{{< badge color="purple" content="Text">}} {{< badge color="blue" content="Item">}} {{< badge color="green" content="Block">}} {{< badge color="yellow" content="Interaction">}} {{< badge color="red" content="Mannequin">}}</div> 
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Teleport specified display to the specified coordinates.  
Selector **~** points to corresponding coordinate of command sender.

<u>**Syntax**</u>  
`/display edit (display) move_to (x) (y) (z)`

<u>**Permission**</u>  
`displayentities.command.display.edit.move_to`

<u>**Example(s)**</u>  
Teleporting to your position can be done using selectors.  
`/display edit (display) move_to ~ ~ ~`

<br>
<br>

<!------  Display > Edit > Glow  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Glow</div>
  <div style="float:right">{{< badge color="purple" content="Text">}} {{< badge color="blue" content="Item">}} {{< badge color="green" content="Block">}} {{< badge color="red" content="Mannequin">}}</div> 
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies glow state and/or changes color of the specified display.  
Item and Block displays support named colors and hex colors.  
Mannequin entities do not support hex colors but only named colors. Colors names are different than for Item and Block displays due to how they're reprensented internally.

<u>**Syntax**</u>  
`/display edit (display) glow (color | @none)`

<u>**Permission**</u>  
`displayentities.command.display.edit.glow`

<u>**Example(s)**</u>  
Setting glow color to **#00FF00**. Mannequin entities do not support hex colors.
`/display edit (display) glow #00FF00`
Setting glow color to **light_blue**.
`/display edit (display) glow light_blue`

<br>
<br>

<!------  Display > Edit > Add Line  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Add Line</div>
  <div style="float:right">{{< badge color="purple" content="Text">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Adds new line to text contents of the specified text display.  
Supports [MiniMessage](https://docs.advntr.dev/minimessage/format.html#standard-tags) formatting and [PlaceholderAPI](https://modrinth.com/plugin/placeholderapi).

<u>**Syntax**</u>  
`/display edit (display) add_line (text)`

<u>**Permission**</u>  
`displayentities.command.display.edit.add_line`

<br>
<br>

<!------  Display > Edit > Remove Line  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Remove Line</div>
  <div style="float:right">{{< badge color="purple" content="Text">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Removes line at the specified position.

<u>**Syntax**</u>  
`/display edit (display) remove_line (line)`

<u>**Permission**</u>  
`displayentities.command.display.edit.remove_line`

<br>
<br>


<!------  Display > Edit > Set Line  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Set Line</div>
  <div style="float:right">{{< badge color="purple" content="Text">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Sets line at specified position to the specified text.  
Supports [MiniMessage](https://docs.advntr.dev/minimessage/format.html#standard-tags) formatting and [PlaceholderAPI](https://modrinth.com/plugin/placeholderapi).

<u>**Syntax**</u>  
`/display edit (display) set_line (line) (text)`

<u>**Permission**</u>  
`displayentities.command.display.edit.set_line`

<br>
<br>

<!------  Display > Edit > Insert Line  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Insert Line</div>
  <div style="float:right">{{< badge color="purple" content="Text">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Inserts new line **before** the specified position.  
Supports [MiniMessage](https://docs.advntr.dev/minimessage/format.html#standard-tags) formatting and [PlaceholderAPI](https://modrinth.com/plugin/placeholderapi).

<u>**Syntax**</u>  
`/display edit (display) insert_line (line) (text)`

<u>**Permission**</u>  
`displayentities.command.display.edit.insert_line`

<br>
<br>

<!------  Display > Edit > Refresh Interval  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Refresh Interval</div>
  <div style="float:right">{{< badge color="purple" content="Text">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies ticks interval at which specified text display will be refreshed to all viewers.  
Interval can be number of ticks, where 20 ticks is equal to 1 second.  
Interval can also be set to `default` which makes it use a value specified in configuration file.

<u>**Syntax**</u>  
`/display edit (display) refresh_interval (ticks) (text)`

<u>**Permission**</u>  
`displayentities.command.display.edit.refresh_interval`

<br>
<br>

<!------  Display > Edit > Alignment  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Alignment</div>
  <div style="float:right">{{< badge color="purple" content="Text">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies text alignment of the specified text display. Alignment can be **left**, **right** or **center**.

<u>**Syntax**</u>  
`/display edit (display) alignment (alignment)`

<u>**Permission**</u>  
`displayentities.command.display.edit.alignment`

<br>
<br>

<!------  Display > Edit > Background  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Background</div>
  <div style="float:right">{{< badge color="purple" content="Text">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies background color of the specified text display.  
Color can be either named (like **cyan**) or any hex value (like **#00FF00**).  
Opacity is specified in percentage, where **0%** is fully transparent, and **100%** is fully opaque.  
Opacity, if unspecified, defaults to fully opaque.

<u>**Syntax**</u>  
`/display edit (display) background (color) [opacity]`

<u>**Permission**</u>  
`displayentities.command.display.edit.background`

<u>**Example(s)**</u>  
`/display edit (display) background #00FF00`  
`/display edit (display) background #00FF00 75%`  
`/display edit (display) background cyan`  
`/display edit (display) background cyan 25%`

<br>
<br>

<!------  Display > Edit > Line Width  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Line Width</div>
  <div style="float:right">{{< badge color="purple" content="Text">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies line width of the specified text display.

<u>**Syntax**</u>  
`/display edit (display) line_width (width)`

<u>**Permission**</u>  
`displayentities.command.display.edit.line_width`

<br>
<br>

<!------  Display > Edit > See Through  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; See Through</div>
  <div style="float:right">{{< badge color="purple" content="Text">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies see through state of the specified text display.

<u>**Syntax**</u>  
`/display edit (display) see_through (true | false)`

<u>**Permission**</u>  
`displayentities.command.display.edit.see_through`

<br>
<br>

<!------  Display > Edit > Text Shadow  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Text Shadow</div>
  <div style="float:right">{{< badge color="purple" content="Text">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies text shadow state of the specified text display.

<u>**Syntax**</u>  
`/display edit (display) text_shadow (true | false)`

<u>**Permission**</u>  
`displayentities.command.display.edit.text_shadow`

<br>
<br>

<!------  Display > Edit > Text Opacity  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Text Opacity</div>
  <div style="float:right">{{< badge color="purple" content="Text">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies text opacity of the specified text display.  
Opacity is specified in percentage, where **0%** is fully transparent, and **100%** is fully opaque.

<u>**Syntax**</u>  
`/display edit (display) text_opacity (opacity)`

<u>**Permission**</u>  
`displayentities.command.display.edit.text_opacity`

<br>
<br>

<!------  Display > Edit > Block  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Block</div>
  <div style="float:right">{{< badge color="green" content="Block">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies the block that is represented by the specified block display. Block can be a predefined block type, or currently held block. Latter can be set with **@main_hand** or **@off_hand** selector.

<u>**Syntax**</u>  
`/display edit (display) block (@main_hand | @off_hand | type)`

<u>**Permission**</u>  
`displayentities.command.display.edit.block`

<br>
<br>

<!------  Display > Edit > Item  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Item</div>
  <div style="float:right">{{< badge color="blue" content="Item">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies the item that is represented by the specified item display. Item can be a predefined item type, or currently held item. Latter can be set with **@main_hand** or **@off_hand** selector.

<u>**Syntax**</u>  
`/display edit (display) item (@main_hand | @off_hand | type)`

<u>**Permission**</u>  
`displayentities.command.display.edit.item`

<br>
<br>

<!------  Display > Edit > Width  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Width</div>
  <div style="float:right">{{< badge color="yellow" content="Interaction">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies width of the specified interaction entity.

<u>**Syntax**</u>  
`/display edit (display) width (width)`

<u>**Permission**</u>  
`displayentities.command.display.edit.width`

<br>
<br>

<!------  Display > Edit > Height  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Height</div>
  <div style="float:right">{{< badge color="yellow" content="Interaction">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies height of the specified interaction entity.

<u>**Syntax**</u>  
`/display edit (display) height (width)`

<u>**Permission**</u>  
`displayentities.command.display.edit.height`

<br>
<br>

<!------  Display > Edit > Response  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Response</div>
  <div style="float:right">{{< badge color="yellow" content="Interaction">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies response state of the specified interaction entity.

<u>**Syntax**</u>  
`/display edit (display) response (true | false)`

<u>**Permission**</u>  
`displayentities.command.display.edit.response`

<br>
<br>

<!------  Display > Edit > Skin  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Skin</div>
  <div style="float:right">{{< badge color="red" content="Mannequin">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies skin of the specified mannequin entity.

<u>**Syntax**</u>  
`/display edit (display) skin (username | uuid)`

<u>**Permission**</u>  
`displayentities.command.display.edit.response`

<u>**Example(s)**</u>  
`/display edit (display) skin Grabsky`  
`/display edit (display) skin 6bd3cf88-7635-4531-8eb1-cfe527c858b8`

<br>
<br>

<!------  Display > Edit > Pose  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Skin</div>
  <div style="float:right">{{< badge color="red" content="Mannequin">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies pose of the specified mannequin entity. Pose can be **standing**, **sneaking**, **swimming**, **fall_flying**, **sleeping** or **sitting**.

<u>**Syntax**</u>  
`/display edit (display) pose (pose)`

<u>**Permission**</u>  
`displayentities.command.display.edit.pose`

<br>
<br>

<!------  Display > Edit > Custom Name  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Custom Name</div>
  <div style="float:right">{{< badge color="red" content="Mannequin">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies custom name of the specified mannequin entity. Custom name is what is displayed above mannequin's head.

<u>**Syntax**</u>  
`/display edit (display) custom_name (name | @hidden)`

<u>**Permission**</u>  
`displayentities.command.display.edit.custom_name`

<br>
<br>

<!------  Display > Edit > Description  ------->

<h4 style="display:flex; justify-content:space-between;">
  <div style="float:left">Edit &nbsp; ⟶ &nbsp; Description</div>
  <div style="float:right">{{< badge color="red" content="Mannequin">}}</div>
</h4>
<hr style="margin:12px 0 0 0; height:1px; color:gray;"> 

<u>**Description**</u>  
Modifies description of the specified mannequin entity. Description is what is displayed below mannequin's custom name.

<u>**Syntax**</u>  
`/display edit (display) description (description | @hidden)`

<u>**Permission**</u>  
`displayentities.command.display.edit.description`

<br>
<br>