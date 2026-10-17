---
title: "Sultan's Archive"
excerpt: "A statically generated game wiki generated from source files from *Sultan's Game*.<br/><img src='/images/sultans_archive.png'>"
collection: portfolio
date: 2025-10-01
---

Sultan's Archive is a statically generated website documenting the content of the video game *Sultan's Game*, presenting the underlying data files as a searchable, interconnected reference. Written in JavaScript, it parses complex original data and generates tens of thousands of pages covering game content such as cards, recipes, tags, and decks.

The main challenge was turning raw, undocumented game data written in poorly structured syntax into a consistent and readable format. Automated page generation handles the large volume of content, with layered regex parsing rules to turn formulas into a standardised format and then into HTML. Related content is linked automatically, allowing users to navigate between elements. The website also includes search functionality and support for all game languages.

A key learning from this project was how to structure a maintainable content-generation pipeline. By separating data parsing, content formatting and page presentation, the website can be regenerated as the underlying game files change and easily extended.


View the [website](http://eryngia.github.io/sultans-archive/).

![Sultan's Archive](/images/sultans_archive.png)