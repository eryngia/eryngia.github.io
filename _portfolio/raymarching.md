---
title: "Raymarching in URP"
excerpt: "A real-time raymarching renderer for Unity's Universal Render Pipeline, with blended distance-field shapes and an animated Mandelbulb fractal, including lighting and shadows.<br/><img src='/images/raymarching.png'>"
collection: portfolio
date: 2026-01-01
---

This Unity project explores raymarching, a technique that renders scenes by tracing rays through mathematical distance fields instead of drawing meshes. It is built for the Universal Render Pipeline using custom render features and passes, so the effect integrates with the engine's normal rendering and runs in real time.

The shapes renderer draws spheres and cubes defined by signed distance functions. Overlapping shapes are combined with a smooth minimum, which merges them into organic, liquid forms, and their colours are blended through HSV space so that transitions between hues look natural. The shader also supports tiling to repeat shapes through space, soft shadows cast by the scene's directional light, and ambient lighting. Surface normals are estimated directly from the distance field.

The fractal renderer implements a distance estimator for the Mandelbulb, a three-dimensional relative of the Mandelbrot set. Its fractal power is animated while the project runs, so that the shape continuously changes and reveals new structures. Colour comes from the lighting and from how many iterations the estimator takes at each point, which highlights the detail in the folds of the surface, and an occlusion term based on the number of ray steps gives the crevices depth.

The project gave me practical experience with GPU rendering: writing HLSL shaders, integrating custom passes into URP, and designing the interface between the C# scene code and the shader so that the effects remain interactive and easy to modify.

View the [source code](https://github.com/eryngia/raymarching).

![Raymarching 1](/images/raymarching.png)

![Raymarching 2](/images/raymarching2.png)

![Raymarching 3](/images/raymarching3.png)