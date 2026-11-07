# ShadeMap Studio

ShadeMap Studio is a Mac app for making SVG maps that Splunk Dashboard Studio's **Choropleth SVG**
visualization can shade: world and country maps, floor plans, network diagrams and tile maps. Every area is
written as a `<path>` with its own id and a plain fill, it checks each map against what Splunk needs, and it
writes the visualization, data source and whole dashboard JSON from the map's own colour rules. It replaces
Vectory Studio.

This repository holds the **releases** and **issue reports**. The source code is kept privately.

## Install

1. Download the latest `ShadeMap-Studio-<version>.dmg` from [Releases](../../releases/latest).
2. Open it and drag **ShadeMap Studio** into **Applications**.
3. Open ShadeMap Studio. It needs macOS 27 or later.

Every release is signed with a Developer ID and notarized by Apple. The `.sha256` file beside each disk
image holds its checksum.

## Updates

ShadeMap Studio doesn't check for updates itself yet. Watch this repository (**Watch › Custom ›
Releases**) to hear about new versions, then install the new disk image over the old app.

## Moving from Vectory Studio

Vectory Studio saved plain SVG files, and ShadeMap Studio opens them as they are (**File › Open…**).
Open the **Splunk Check** tab afterwards: Vectory wrote rectangles, circles and polygons as drawn, and
the check offers to turn them into paths.

## Reporting a problem

[Open an issue](../../issues/new) with what you were doing, what you expected and what happened. Include
the version from **ShadeMap Studio › About ShadeMap Studio**. If a map doesn't shade in your Splunk, say
which Splunk version you use and attach the SVG if you can. Please don't attach maps, dashboards or data
that show real hosts, sites or other details of your environment.

The starter maps are made from [Natural Earth](https://www.naturalearthdata.com) data, which is in the
public domain.

© 2026 Aaron Stone. All rights reserved.
