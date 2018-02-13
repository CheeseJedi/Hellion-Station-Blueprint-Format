# Hellion-Station-Blueprint-Format
A community proposal for a JSON based file format for the interchange of Hellion station blueprints.

This proposal aims to set out a minimal JSON data format to describe the docking hierarchy of ships and modules
within the game HELLION by Zero Gravity Games.

The format describes a list of objects, each representing an in-game module (or ship), each with it's own list of
DockingPorts. Each module in the list has a unique StructureID; a docking port that is in use (docked) will list
the StructureID of the 'other' module as well as its PortName, describing the docking relationship in a 
bi-directional manner.

Note this is **not a data export format** for HELLION Dedicated Server .save files as it does not describe the
condition, inventory or other state of any of the modules.

Contributors: CheeseJedi, GLotsapot, Yozheek
