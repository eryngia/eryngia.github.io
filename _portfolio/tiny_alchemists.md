---
title: "Tiny Alchemists"
excerpt: "A cooperative, physics-based multiplayer party game built in Unity with experimental potion crafting and networked gameplay.<br/><img src='/images/tiny_alchemists.png'>"
collection: portfolio
date: 2025-09-01
---

Tiny Alchemists is a cooperative multiplayer party game built in Unity, in which players control tiny homunculi in a magical greenhouse. Players collect ingredients, experiment with potion combinations and use their effects to overcome environmental obstacles before a spreading miasma consumes the map. The game combines physics-based interactions, sandbox experimentation and cooperative problem-solving, with multiple ways to approach each challenge.

As lead game designer, I helped define the game's core mechanics, wrote the game design document and translated the team's ideas into implementable systems. 

As lead programmer, one of the main challenges was the miasma system, a spreading environmental hazard that uses a voxel grid with a dynamically generated mesh and probabilistic growth for organic and performant puddle formation. Another difficulty was synchronizing objects across multiplayer clients using Unity Netcode for GameObjects. The codebase also had to be designed to be easy to maintain and extend, so I introduced ScriptableObjects for configurable properties, and polymorphic effect behaviours for dynamic potions combinations.

The project combined game design with practical software engineering challenges. It taught me how to turn a creative concept into a coherent set of game systems while balancing design ambitions, implementation complexity and the constraints of a collaborative development process.

View the [website](https://shuangyuzhu04.github.io/tiny-alchemists-web/), [GDD](/files/tiny_alchemists.pdf), or [my blog](https://eryngia.notion.site/Tiny-Alchemists-Game-Dev-Blog-0347b6366964824586b181a65ee1a7e9).

![Tiny Alchemists 1](/images/tiny_alchemists.png)

![Tiny Alchemists 2](/images/tiny_alchemists2.png)

![Tiny Alchemists 3](/images/tiny_alchemists3.png)

![Tiny Alchemists 4](/images/tiny_alchemists4.png)