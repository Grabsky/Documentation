---
title: Getting Started
type: docs
weight: 1
---

**DisplayEntities** is an utility plugin adding commands for manipulation of server-side Display Entities, Interaction Entities and Mannequins (NPCs). Comes with [**PlaceholderAPI**](https://github.com/PlaceholderAPI/PlaceholderAPI) and [**MiniMessage**](https://docs.advntr.dev/minimessage/format.html)   support.


<br/>

### But what *are* Display Entities?
Display entities are lightweight hologram-like entities added in 1.19.4. They are capable of displaying text, items and blocks, and serve as an alternative to armor stands. You can read more [**here**](https://minecraft.wiki/w/Display).

### How does the plugin work?
Each entity created by the plugin will be *physically* kept in the world until manually removed. This can be done either by plugin-provided command or built-in, vanilla commands.

Since all entities are server-side, you can move / scale them freely with external tools such us [**Axiom**](https://modrinth.com/mod/axiom).

### How is that an *utility* plugin?
Plugin does not store anything on it's own except configuration file and necessary data attached to the PDC (Persistent Data Container) of each entity it interacts with. It leaves minimal footprint on the server.

To make the plugin a bit more useful, it comes with **MiniMessage** support and packet-level **PlaceholderAPI** hook. That should possibly make it as useful as any other holograms plugin you're already familiar with.

<br/>

## Features

- **Pure Simplicity**  
  Based on existing Bukkit and Paper APIs with no NMS access involved.

- **Minimal Footprint**  
  Basically a user-friendly wrapper around display entities. There's not much logic attached to it.

- **Compatibility**  
  Entities created by the plugin are real entities that can be modified with commands and other plugins.

- [**MiniMessage Support**](https://docs.advntr.dev/minimessage/format.html)  
  Text display entities are capable of parsing MiniMessage formatting.

- [**Folia Support**](https://github.com/PaperMC/Folia)  
  Designed to run on Paper and Folia servers. Folia Scheduler APIs are used when needed.

- [**PlaceholderAPI Support**](https://github.com/PlaceholderAPI/PlaceholderAPI)  
  Placeholders inside text displays are parsed and displayed per-player.  
  <sup>(Requires **[PlaceholderAPI](https://github.com/PlaceholderAPI/PlaceholderAPI)** and **[PacketEvents](https://github.com/retrooper/packetevents)**)</sup>

<br/>

## Requirements
Plugin runs only on **Paper** (or **Folia**) **1.21.4** and above, powered by **Java 21** or higher.
