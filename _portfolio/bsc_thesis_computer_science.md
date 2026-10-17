---
title: "Bachelor's thesis: Procedural shoot 'em up"
excerpt: "Instar, a pixel shoot 'em up built in Unity in which enemies, waves and environments are generated entirely procedurally.<br/><img src='/images/bsc_thesis_computer_science.png'>"
collection: portfolio
date: 2025-02-01
---

Instar is a shoot 'em up developed in Unity and C# as my computer science thesis, supervised by Prof Ian Miguel. The game is based on extensive research of the history of the genre, with responsive controls, simple but strategic weapons and a scoring system that rewards defeating enemies without taking damage. Each run is entirely procedurally generated: levels, enemy sprites, enemy behaviour, wave patterns and the surrounding environment. This creates a new challenge with every run. 

The enemies are insects, assembled from procedurally generated parts defined by Bézier curves, including bodies, wings, legs and antennae. The generation aims to create varied, interesting, yet balanced attack and wave patterns. The environment is built from Voronoi cells. Points are placed with Poisson disc sampling, carved into irregular terrain by a layered Perlin noise curve, triangulated with the Bowyer-Watson algorithm, and converted into Voronoi cells that are rasterised dynamically.

The project was evaluated with five playtesters, who rated the visuals, interface and enemy design very highly overall. Delivering the project taught me about scoping a complete game, structuring a larger Unity codebase with scriptable objects and events, and balancing procedural variety against consistent quality.

Read the [report](/files/bsc_thesis_computer_science_report.pdf), [presentation](/files/bsc_thesis_computer_science_presentation.pdf), or [source code](https://github.com/eryngia/instar).

![Instar 1](/images/bsc_thesis_computer_science.png)

![Instar 2](/images/bsc_thesis_computer_science2.png)

![Instar 3](/images/bsc_thesis_computer_science3.png)