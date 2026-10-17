---
title: "Stippler"
excerpt: "A C++ implementation and analysis of four image stippling algorithms: rejection, CVT, AIS, and Wang tiles.<br/><img src='/images/stippler.png'>"
collection: portfolio
date: 2026-04-01
---

This C++ application converts images into stippled artwork, representing shading and detail through the placement of dots. It implements four algorithms: rejection sampling, weighted centroidal Voronoi tessellation (CVT), adaptive incremental stippling (AIS), and recursive Wang tile stippling. The application uses SDL and supports configurable dot sizes, colour inversion, and saving the generated images to file.

The project explores different approaches to generating visually pleasing dot distributions, balancing uniformity, natural appearance and computational efficiency. CVT uses iterative relaxation to produce evenly spaced dots, while AIS incrementally places dots according to local image density. Recursive Wang tile stippling uses precomputed blue-noise distributions to generate results quickly.

I evaluated the algorithms by comparing their output images, execution times and spectral properties. This included analysing power spectra, radial average power and anisotropy to investigate how closely each method approximates blue noise distributions. The results highlighted the trade-offs between the algorithms: CVT produces highly regular distributions but is computationally expensive, while Wang tiles are significantly faster. AIS offers a compromise between performance and visual characteristics. 

This project improved my knowledge of computational geometry, sampling algorithms and image processing, as well as methods for quantitative analysis of graphics techniques.

Read the [report](/files/stippler.pdf) or [source code](https://github.com/eryngia/stippler).

![Stippler 1](/images/stippler.png)

![Stippler 2](/images/stippler2.png)