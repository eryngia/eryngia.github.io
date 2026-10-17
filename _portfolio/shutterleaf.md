---
title: "Shutterleaf"
excerpt: "A wildlife photography game with an open forest in which predators and prey interact in an autonomous ecosystem using decision trees and pathfinding.<br/><img src='/images/shutterleaf.png'>"
collection: portfolio
date: 2024-11-01
---

Shutterleaf is a relaxed simulation game in which the player observes a randomly generated forest from above and photographs the animals that live in it. Wolves hunt deer, foxes stalk rabbits, and the prey flee, look for food and visit ponds to drink. The player cannot control the animals directly but can place bait to lure them into good positions, and photos are scored on how many interesting animals and features are captured in the frame. It is written in Java with Processing, using my own game engine.

The main technical work was a library of AI behaviours built as reusable components for the engine. These cover steering behaviours, including seek, flee, pursue with target prediction and wander, as well as separation, cohesion and velocity matching, which combine to produce flocking. Obstacle avoidance and boundary control keep movement natural, and a grid-based A* pathfinder lets characters navigate around obstacles, following their path by looking ahead rather than tracing it exactly. Behaviours are force-based, so they can be layered on top of each other and the physics system. The animals are driven by decision trees that reflect their priorities. A predator wanders until it becomes hungry and then searches for and chases prey, whereas prey animals put escaping nearby predators first and only then look for bait or water.

I also extended the engine to support new functionality, including a multiple cameras that can be moved and zoomed, a layered renderer for drawing operations so sprites appear in the correct order, and grid-based procedural generation. The result is a small ecosystem in which the interactions between the animals are interesting to watch.

Read the [report](/files/shutterleaf.pdf).

![Shutterleaf](/images/shutterleaf.png)