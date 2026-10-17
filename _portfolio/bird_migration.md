---
title: "Bird migration visualisation"
excerpt: "A Spark and Scala pipeline that turns millions of eBird sightings into interactive migration maps, with machine learning to group migration routes and forecast shifts in range.<br/><img src='/images/bird_migration.png'>"
collection: portfolio
date: 2026-07-01
---

This project analyses how bird populations move across North America over the year and how their ranges shift over time, using large-scale citizen science observations from the eBird dataset. The data comes as records of species, counts, dates and coordinates, with inconsistent formatting and many entries that cannot be used. I wrote a Scala and Apache Spark pipeline that keeps only approved observations, parses counts and dates into typed fields, and discards records with missing or invalid coordinates. The cleaned data is held as a typed Spark Dataset and queried through a lightweight HTTP service, so a Python notebook can request any species on demand without reloading the data.

The service exposes three analyses per species: seasonal migration phases, range of latitude and longitude travelled, and yearly density surface of sightings. These feed a set of Plotly maps with interactive controls. I also clustered these trajectories with k-means to separate migration behaviours, such as long-distance northbound movers, short-range altitudinal movers and resident species. This grouping matched known flyways without any such labels being given to the model. To forecast movement, I trained a gradient boosting regressor on weekly centroids, the phase of the year and recent range trends. It was evaluated on later years held out from training. It predicted the position of the population more accurately than a baseline using the average seasonal path, and it highlighted a gradual northward drift in the range of several species over the period.

The project required handling data that was large, uneven in quality and heavily biased by observer behaviour, as sightings cluster around cities and popular birding times. It also gave me experience designing a data service around Spark, and building analysis tools that let non-specialists explore the results directly.

![Bird migration 1](/images/bird_migration.png)

![Bird migration 2](/images/bird_migration2.png)

![Bird migration 3](/images/bird_migration3.png)