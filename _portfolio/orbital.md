---
title: "Orbital"
excerpt: "A physics puzzle game built on a custom 2D engine with forces, collisions and constraints, where randomised abilities make every attempt a new problem.<br/><img src='/images/orbital.png'>"
collection: portfolio
date: 2024-10-01
---

Orbital is a light-hearted physics puzzle game, developed in Java with the Processing framework. It was built to demonstrate a game engine and physics system that I wrote from scratch. The player controls an alien who has to get through each level using the environment, including crates, springs and hanging balls, together with a set of abilities such as spawning blocks, freezing objects and teleporting. The levels are not designed with a single solution. The abilities on offer are randomised each time a level is attempted, so the player has to improvise and adapt, and the same level can be solved in different ways. This was inspired by physics puzzle games such as Mosa Lina.

The engine is modular and component-based. Every element of the game is a game object assembled from reusable components, arranged in a scene hierarchy where children follow their parents. The engine runs the core game loop, an event system for input and collisions, and a deferred clean-up step that keeps the object hierarchy safe from changes during updates. On top of this sits a physics engine based on a point-mass model. Forces come from pluggable generators, including gravity, drag, springs and buoyancy, which can be combined freely. Collisions are resolved with impulses and restitution, with correction of interpenetration and handling of resting contact to avoid jitter. Rod and cable constraints give fixed or maximum distances between objects, which enables nechanics like pendulums and hanging objects.

Developing both the engine and a game within taught me a lot about the trade-offs when designing a developer framework regarding generality, performance, and ease of use.

Read the [report](/files/orbital.pdf).

![Orbital](/images/orbital.png)