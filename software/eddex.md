---
title: Overview
---
# Overview

Eddex (Evo-Devo Design Explorer) enables designers to run evolutionary optimization jobs on Dexen without writing code.

{% include fig.html file="eddex.png" caption="The Eddex architecture." %}

With Eddex, the designer defines the development and evaluation procedure using a parametric modelling environment such as Sidefx Houdini. (We have not yet implemented a link to McNeel Grasshopper, but this can also be done.) Eddex uses an automated task generator to create development and evaluation scripts that wrap the parametric models, as well as a number of other required scripts, so that they can be executed on Dexen.

Once the scripts have been generated, the designer can run the evolutionary job using the graphical interface provided by the Eddex web application. Running the job will generate a number of graphs and charts that give information on how it is progressing. The web application also enables the designer to download data associated with specific design variants, including the 3D models and simulation results.

For the design development model, the modelling commands within the parametric modelling environment are typically sufficient. For the evaluation model, however, a number of more advanced simulations are often needed in order to calculate performance metrics. For this, the parametric modelling environment requires a library of plugins that link to existing simulation engines. [Houdarcs](/software/houdarcs) is such a library, developed for SideFx Houdini. The Design Automation Lab uses Houdini rather than Grasshopper due to its ability to handle greater complexity and better scalability. 

Recently, the Design Automation Lab has developed a parametric modelling tool in the browser, called [Möbius Modeller](/software/mobius). A link between Eddex and Möbius is also planned for the future. 

# Links

- Lead PI: [Patrick Janssen](http://patrick.janssen.name)

## Source Code Repository

- [Eddex Github Repository](https://github.com/phtj/eddex)

## Related Projects

- [Dexen](http://design-automation.net/dexen)
- [Houdarcs](http://design-automation.net/houdarcs)

## Papers

- Janssen, P., (2015). "Dexen: A scalable and extensible platform for experimenting with population-based design exploration algorithms". AI EDAM 29, 443–455. [Link](https://www.cambridge.org/core/journals/ai-edam/article/dexen-a-scalable-and-extensible-platform-for-experimenting-with-population-based-design-exploration-algorithms/B7AD943B220CB73A2C2538996B0280C0)

## See also

- [Sidefx Houdini](http://sidefx.com/)

## Install


- [Eddex Install](eddex_install.html)