---
title: Overview
---
# Overview

Houdarcs (Houdini Architecture Assets) is a library of nodes for SideFX Houdini for performing simulation and analysis of buildings and urban areas. In some cases, the nodes link to existing simulation engines or libraries. The figure above shows the relationship between the plugins and the simulation engines or libraries.

{% include fig.html file="houdarcs.png" caption="Houdarcs, a library of plugins for Sidefx Houdini to support performance-based design." %}

# Simulation and Analysis Plugins

The plugins for simulation and analysis are grouped into six main areas:

- Daylight Simulation: Calculate illuminance or irradiance either at specific times during the day or over an entire year.
- EnergyPlus: Calculate heating and cooling loads based on building construction, schedules, and other data. (See Figure 8.)
- Structural Simulation: Calculate stress and strain using finite element methods for various types of structures.
- Network Analysis: Calculate various metrics for graphs, including shortest paths, centrality, connectivity, and so forth.
- Space Syntax: Generate axial line maps and calculate depth, integration, mean depth, and R2 correlation.
- Window Analyst: Calculate various metric for windows in urban environments, including the sky view factor, sky visibility factor, unobstructed view factor, solar factor, and privacy factor.

![Houdarcs](/assets/images/houdarcs.png)
*The interface for the EnergyPlus node allowing the user to specify various simulation settings.*

# Links

Various links:

## Developers

- Lead PI: [Patrick Janssen](http://patrick.janssen.name)

## Source Code Repository

- [Houdarcs Github Repository](https://github.com/phtj/houdarcs)

## Related Projects

- [Dexen](http://design-automation.net/dexen)
- [Eddex](http://design-automation.net/eddex)

## Papers

- Janssen, P., (2015). "Dexen: A scalable and extensible platform for experimenting with population-based design exploration algorithms". AI EDAM 29, 443–455. [Link](https://www.cambridge.org/core/journals/ai-edam/article/dexen-a-scalable-and-extensible-platform-for-experimenting-with-population-based-design-exploration-algorithms/B7AD943B220CB73A2C2538996B0280C0)

## See also

- [Sidefx Houdini](http://sidefx.com/)

