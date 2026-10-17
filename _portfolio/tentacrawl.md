---
title: "Tentacrawl"
excerpt: "A turn-based roguelike in which an octopus explores procedurally generated dungeons built with a layered algorithm for structure, themed rooms and item and enemy placement.<br/><img src='/images/tentacrawl.png'>"
collection: portfolio
date: 2024-12-01
---

Tentacrawl is a tactical dungeon crawler in which the player controls an octopus exploring a series of procedurally generated levels. Each level has to be explored to find the keys that unlock the exit, along with items that strengthen the player, while a variety of enemies defend the rooms. Combat is turn-based, and every action by the player triggers a response from nearby enemies. Attacks are charged and released in patterns that become larger and more complex as the difficulty increases, so players must plan ahead and anticipate their opponents. It is written in Java with Processing, using my own entity-component game engine.

The main focus of the project was the level generator, which works in layers. A structure generator divides the map into zones through binary space partitioning, places rooms in each zone and connects them with corridors. The partition tree guarantees that the whole level is connected. An interior generator groups neighbouring rooms into themed areas, such as underground or residential, and then assigns each room a specific type such as a library, dining room or mineshaft. This produces levels that feel coherent. Decorations are placed according to the density and weights of each room type. Finally, the entrance, exit and keys are spread across the level to force players to explore, and the map is populated with enemy groups that become stronger as the difficulty increases.

The game engine was also extended with new functionality such as an improved input system and more complex time-sequencing. Together, these systems produce a complete, replayable game loop from a small set of generators and data.

Read the [report](/files/tentacrawl.pdf).

![Tentacrawl](/images/tentacrawl.png)