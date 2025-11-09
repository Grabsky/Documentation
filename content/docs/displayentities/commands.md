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

<div class="ent">
  <h4>Help</h4>
  <div>
    {{< badge content="Management">}}
  </div>
</div>

<u>**Description**</u>  
Shows list of available commands.

<u>**Syntax**</u>  
`/display help [page]`

<u>**Permission**</u>  
`displayentities.command.display.help`

<br>
<br>

<!------  Display > Create  ------->

<div class="ent">
  <h4>Create</h4>
  <div>
    {{< badge content="Management">}}
  </div>
</div>

<u>**Description**</u>  
Creates display of the specified type. Type can be **text**, **item**, **block**, **interaction** or **mannequin**. 

<u>**Syntax**</u>  
`/display create (type) (name)`

<u>**Permission**</u>  
`displayentities.command.display.create`

<br>
<br>

<!------  Display > Delete  ------->

<div class="ent">
  <h4>Delete</h4>
  <div>
    {{< badge content="Management">}}
  </div>
</div>

<u>**Description**</u>  
Deletes specified entity from the world. This action is irreversible.

<u>**Syntax**</u>  
`/display delete (display)`

<u>**Permission**</u>  
`displayentities.command.display.delete`

<br>
<br>

<!------  Display > Clone  ------->

<div class="ent">
  <h4>Clone</h4>
  <div>
    {{< badge content="Management">}}
  </div>
</div>

<u>**Description**</u>  
Clones specified display to a new one.

<u>**Syntax**</u>  
`/display clone (display) (name)`

<u>**Permission**</u>  
`displayentities.command.display.clone`

<br>
<br>

<!------  Display > Respawn  ------->

<div class="ent">
  <h4>Respawn</h4>
  <div>
    {{< badge content="Management">}}
  </div>
</div>

<u>**Description**</u>  
Respawns specified display. Use it after adding placeholders or modifying placeholder refresh interval.

<u>**Syntax**</u>  
`/display respawn (display)`

<u>**Permission**</u>  
`displayentities.command.display.respawn`

<br>
<br>

<!------  Display > Teleport  ------->

<div class="ent">
  <h4>Teleport</h4>
  <div>
    {{< badge content="Management">}}
  </div>
</div>

<u>**Description**</u>  
Teleports you to the specified display.

<u>**Syntax**</u>  
`/display teleport (display)`

<u>**Permission**</u>  
`displayentities.command.display.teleport`

<br>
<br>

<!------  Display > Export  ------->

<div class="ent">
  <h4>Export</h4>
  <div>
    {{< badge content="Management">}}
  </div>
</div>

<u>**Description**</u>  
Exports specified display to a file.

<u>**Syntax**</u>  
`/display export (display)`

<u>**Permission**</u>  
`displayentities.command.display.export`

<br>
<br>

<!------  Display > Import  ------->

<div class="ent">
  <h4>Import</h4>
  <div>
    {{< badge content="Management">}}
  </div>
</div>

<u>**Description**</u>  
Imports specified file to a new display.

<u>**Syntax**</u>  
`/display import (file) (name)`

<u>**Permission**</u>  
`displayentities.command.display.import`

<br>
<br>

<!------  Display > Edit > Scale  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Scale</h4>
  <div>
    {{< badge color="purple" content="Text">}}
    {{< badge color="blue" content="Item">}}
    {{< badge color="green" content="Block">}}
  </div>
</div>

<u>**Description**</u>  
Modifies scale of the specified display.

<u>**Syntax**</u>  
`/display edit (display) scale (x) (y) (z)`

<u>**Permission**</u>  
`displayentities.command.display.edit.scale`

<br>
<br>

<!------  Display > Edit > View Range  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; View Range</h4>
  <div>
    {{< badge color="purple" content="Text">}}
    {{< badge color="blue" content="Item">}}
    {{< badge color="green" content="Block">}}
  </div>
</div>

<u>**Description**</u>  
Modifies view range of the specified display. Range must be a value between **0.0** and **1.0**.

<u>**Syntax**</u>  
`/display edit (display) view_range (range)`

<u>**Permission**</u>  
`displayentities.command.display.edit.view_range`

<br>
<br>

<!------  Display > Edit > Billboard  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Billboard</h4>
  <div>
    {{< badge color="purple" content="Text">}}
    {{< badge color="blue" content="Item">}}
    {{< badge color="green" content="Block">}}
  </div>
</div>

<u>**Description**</u>  
Modifies billboard of the specified text display. Billboard can be **fixed**, **center**, **horizontal** or **vertical**.

<u>**Syntax**</u>  
`/display edit (display) billboard (billboard)` 

<u>**Permission**</u>  
`displayentities.command.display.edit.billboard`

<br>
<br>

<!------  Display > Edit > Brightness  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Brightness</h4>
  <div>
    {{< badge color="purple" content="Text">}}
    {{< badge color="blue" content="Item">}}
    {{< badge color="green" content="Block">}}
  </div>
</div>

<u>**Description**</u>  
Modifies brightness of the specified display. Brightness must be a value between 0 and 15.

<u>**Syntax**</u>  
`/display edit (display) brightness (block | sky) (brightness)`  

<u>**Permission**</u>  
`displayentities.command.display.edit.brightness`

<br>
<br>

<!------  Display > Edit > Rotate X  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Rotate X</h4>
  <div>
    {{< badge color="purple" content="Text">}}
    {{< badge color="blue" content="Item">}}
    {{< badge color="green" content="Block">}}
  </div>
</div>

<u>**Description**</u>  
Rotates specified display for specified amount of degrees around X axis. Works only when billboard is fixed.

<u>**Syntax**</u>  
`/display edit (display) rotate_x (degrees)`  

<u>**Permission**</u>  
`displayentities.command.display.edit.rotate_x`

<br>
<br>

<!------  Display > Edit > Rotate Y  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Rotate Y</h4>
  <div>
    {{< badge color="purple" content="Text">}}
    {{< badge color="blue" content="Item">}}
    {{< badge color="green" content="Block">}}
  </div>
</div>

<u>**Description**</u>  
Rotates specified display for specified amount of degrees around Y axis. Works only when billboard is fixed.

<u>**Syntax**</u>  
`/display edit (display) rotate_y (degrees)`  

<u>**Permission**</u>  
`displayentities.command.display.edit.rotate_y`

<br>
<br>

<!------  Display > Edit > Move To  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Move To</h4>
  <div>
    {{< badge color="purple" content="Text">}}
    {{< badge color="blue" content="Item">}}
    {{< badge color="green" content="Block">}}
    {{< badge color="yellow" content="Interaction">}}
    {{< badge color="red" content="Mannequin">}}
  </div>
</div>

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

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Glow</h4>
  <div>
    {{< badge color="purple" content="Text">}}
    {{< badge color="blue" content="Item">}}
    {{< badge color="green" content="Block">}}
    {{< badge color="red" content="Mannequin">}}
  </div>
</div>

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

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Add Line</h4>
  <div>
    {{< badge color="purple" content="Text">}}
  </div>
</div>

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

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Remove Line</h4>
  <div>
    {{< badge color="purple" content="Text">}}
  </div>
</div>

<u>**Description**</u>  
Removes line at the specified position.

<u>**Syntax**</u>  
`/display edit (display) remove_line (line)`

<u>**Permission**</u>  
`displayentities.command.display.edit.remove_line`

<br>
<br>


<!------  Display > Edit > Set Line  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Set Line</h4>
  <div>
    {{< badge color="purple" content="Text">}}
  </div>
</div>

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

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Insert Line</h4>
  <div>
    {{< badge color="purple" content="Text">}}
  </div>
</div>

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

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Refresh Interval</h4>
  <div>
    {{< badge color="purple" content="Text">}}
  </div>
</div>

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

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Alignment</h4>
  <div>
    {{< badge color="purple" content="Text">}}
  </div>
</div>

<u>**Description**</u>  
Modifies text alignment of the specified text display. Alignment can be **left**, **right** or **center**.

<u>**Syntax**</u>  
`/display edit (display) alignment (alignment)`

<u>**Permission**</u>  
`displayentities.command.display.edit.alignment`

<br>
<br>

<!------  Display > Edit > Background  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Background</h4>
  <div>
    {{< badge color="purple" content="Text">}}
  </div>
</div>

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

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Line Width</h4>
  <div>
    {{< badge color="purple" content="Text">}}
  </div>
</div>

<u>**Description**</u>  
Modifies line width of the specified text display.

<u>**Syntax**</u>  
`/display edit (display) line_width (width)`

<u>**Permission**</u>  
`displayentities.command.display.edit.line_width`

<br>
<br>

<!------  Display > Edit > See Through  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; See Through</h4>
  <div>
    {{< badge color="purple" content="Text">}}
  </div>
</div>

<u>**Description**</u>  
Modifies see through state of the specified text display.

<u>**Syntax**</u>  
`/display edit (display) see_through (true | false)`

<u>**Permission**</u>  
`displayentities.command.display.edit.see_through`

<br>
<br>

<!------  Display > Edit > Text Shadow  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Text Shadow</h4>
  <div>
    {{< badge color="purple" content="Text">}}
  </div>
</div>

<u>**Description**</u>  
Modifies text shadow state of the specified text display.

<u>**Syntax**</u>  
`/display edit (display) text_shadow (true | false)`

<u>**Permission**</u>  
`displayentities.command.display.edit.text_shadow`

<br>
<br>

<!------  Display > Edit > Text Opacity  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Text Opacity</h4>
  <div>
    {{< badge color="purple" content="Text">}}
  </div>
</div>

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

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Block</h4>
  <div>
    {{< badge color="green" content="Block">}}
  </div>
</div>

<u>**Description**</u>  
Modifies the block that is represented by the specified block display. Block can be a predefined block type, or currently held block. Latter can be set with **@main_hand** or **@off_hand** selector.

<u>**Syntax**</u>  
`/display edit (display) block (@main_hand | @off_hand | type)`

<u>**Permission**</u>  
`displayentities.command.display.edit.block`

<br>
<br>

<!------  Display > Edit > Item  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Item</h4>
  <div>
    {{< badge color="blue" content="Item">}}
  </div>
</div>

<u>**Description**</u>  
Modifies the item that is represented by the specified item display. Item can be a predefined item type, or currently held item. Latter can be set with **@main_hand** or **@off_hand** selector.

<u>**Syntax**</u>  
`/display edit (display) item (@main_hand | @off_hand | type)`

<u>**Permission**</u>  
`displayentities.command.display.edit.item`

<br>
<br>

<!------  Display > Edit > Width  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Width</h4>
  <div>
    {{< badge color="yellow" content="Interaction">}}
  </div>
</div>

<u>**Description**</u>  
Modifies width of the specified interaction entity.

<u>**Syntax**</u>  
`/display edit (display) width (width)`

<u>**Permission**</u>  
`displayentities.command.display.edit.width`

<br>
<br>

<!------  Display > Edit > Height  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Height</h4>
  <div>
    {{< badge color="yellow" content="Interaction">}}
  </div>
</div>

<u>**Description**</u>  
Modifies height of the specified interaction entity.

<u>**Syntax**</u>  
`/display edit (display) height (width)`

<u>**Permission**</u>  
`displayentities.command.display.edit.height`

<br>
<br>

<!------  Display > Edit > Response  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Response</h4>
  <div>
    {{< badge color="yellow" content="Interaction">}}
  </div>
</div>

<u>**Description**</u>  
Modifies response state of the specified interaction entity.

<u>**Syntax**</u>  
`/display edit (display) response (true | false)`

<u>**Permission**</u>  
`displayentities.command.display.edit.response`

<br>
<br>

<!------  Display > Edit > Skin  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Skin</h4>
  <div>
    {{< badge color="red" content="Mannequin">}}
  </div>
</div>

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

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Pose</h4>
  <div>
    {{< badge color="red" content="Mannequin">}}
  </div>
</div>


<u>**Description**</u>  
Modifies pose of the specified mannequin entity. Pose can be **standing**, **sneaking**, **swimming**, **fall_flying**, **sleeping** or **sitting**.

<u>**Syntax**</u>  
`/display edit (display) pose (pose)`

<u>**Permission**</u>  
`displayentities.command.display.edit.pose`

<br>
<br>

<!------  Display > Edit > Custom Name  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Custom Name</h4>
  <div>
    {{< badge color="red" content="Mannequin">}}
  </div>
</div>


<u>**Description**</u>  
Modifies custom name of the specified mannequin entity. Custom name is what is displayed above mannequin's head.

<u>**Syntax**</u>  
`/display edit (display) custom_name (name | @hidden)`

<u>**Permission**</u>  
`displayentities.command.display.edit.custom_name`

<br>
<br>

<!------  Display > Edit > Description  ------->

<div class="ent">
  <h4>Edit &nbsp; ⟶ &nbsp; Description</h4>
  <div>
    {{< badge color="red" content="Mannequin">}}
  </div>
</div>


<u>**Description**</u>  
Modifies description of the specified mannequin entity. Description is what is displayed below mannequin's custom name.

<u>**Syntax**</u>  
`/display edit (display) description (description | @hidden)`

<u>**Permission**</u>  
`displayentities.command.display.edit.description`

<br>
<br>