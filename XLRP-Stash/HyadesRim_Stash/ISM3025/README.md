# ISM3025_data

Data for ISM3025, this data was exported by Morphyum out of his project [InnerSphereMap](https://github.com/Morphyum/InnerSphereMap). The goals for the ISM3025 project are:

* All systems from BattleTech lore in the year 3025 as accessible by Inner Sphere powers
* Complete independance of any other mod, while trying to be as compatiable as possible
* Proper rendering of borders and map data
* Relative configurablility for the DLL/Assembly

## What's Been Done

The initial data had all systems, including ones owned by factions that the Inner Sphere powers did not have contact with in 3025. A quick rectangular cutout was made, boxing in the systems owned by the Inner Sphere powers. Systems from the initial data that had owners other then those factions in vanilla were simply removed (this should be revisited!). Abandoned systems were then assigned to closest faction to make cohesive borders and any faction data other than that of vanilla factions was removed. The shop data that was in the initial data was removed (as all systems had the same shop setup). 

## What Needs to Be Done (!!)

### NEEDS CONTRIBUTORS!

* Many, many systems do not have descriptions and have generated biomes/tags
  * Ideally, volunteers would claim some amount of systems
  * Research system (Sarna!), fill system description out and check existing tags/biomes
* Probably many systems need to be removed (to match the goals of above)
* Jump distance needs to be set to be able to reach all systems

### Likely Covered

* Contract targets/givers aren't really correct
  * Givers only contain Locals/Owner
  * Targets are literally everyone
  * DLL-based solution seems plausible
* A system for preventing the borders from going to the edge of the map
  * Currently border systems that have no owner constrain it to the most part
  * Could have "fake systems" that are injected by dll into border rendering shader?

## DLL/Assembly

The included assembly is out of [this repository](https://github.com/mpstark/ism3025) but may not be 100% up-to-date. It provides:

* Configurable map dimensions/zoom levels
* Custom camera clamping/smooth zooming
* Working borders and map border-line
* Configurable faction colors and faction logos
* Shop generation by system tags
