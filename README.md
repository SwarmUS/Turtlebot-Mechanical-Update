# Turtlebot-Mechanical-Update

This repository contains the 3D model of a modified Turtlebot Burger used by the SwarmUS project.

## Requirements
- Solidworks 2021

## Getting started

This repository contains submodule of 3D model parts. Right after cloning the project and prior to opening any assembly, run the following command:

```
git submodule update --init --recursive
```

### Repository structure

------

```
Turtlebot-Mechanical-Update
├── outputs
│   ├── dxf
|   ├── pdf
│   └── STL
|   	├── external
│   	└── internal
├── external
├── internal
├── TurtleBot
├── Turtlebot_modified.SLDASM
└── README.md
```

#### Turtlebot_modified.SLDASM

Main assembly of the modified Turtlebot. It's composed of a Turtlebot Burger with additionnal components that are external to the robot (*external*) and of components that are internal to the robot (*internal*). These components wrre mostly added to support mechanically and electrically the HiveBoard and its BeeBoards.

### Turtlebot

This folder contains all the components of the Turtlebot and it contains the Turtlebot's assembly itself. All the components and the assembly were exported from the Robotis Model on [OnShape](https://cad.onshape.com/documents/2586c4659ef3e7078e91168b/w/14abf4cb615429a14a2732cc/e/9ae9841864e78c02c4966c5e) and was converted to a SolidWorks assembly afterwards.

### external

Contains the 3D models of the external components and their supports. Significant assemblies and parts are described below:

- **qr_plate.SLDPRT**: Plate on which a QR code is glued on. Can be directly screwed on the Turtlebot top layer.
- **qr_plate_support.SLDPRT**: Supports of the qr_plate. The part has two [configurations](http://help.solidworks.com/2021/English/SolidWorks/sldworks/c_Configurations_Overview.htm), one for the port side and one for the starboard side.
- [HiveBoard-BeeBoard-Mechanical](https://github.com/SwarmUS/HiveBoard-BeeBoard-Mechanical): Submodule that contains the 3D models of the BeeBoard and the HiveBoard and their cases. 


### internal

Contains the 3D models of the internal components added to the Turtlebot. Significant assemblies and parts are described below:

- **REG_313080006.SLDPRT**: 313080006 5V regulator for powering the Hiveboard and its BeeBoards.
- **assembled_interloc_system.SLDASM**: Assembly of the HiveBoard, 3x BeeBoards, the voltage regulator (REG_313080006), a plate with the bolt pattern of all the components and some standoff for the assembly with the Turtlebot. The BeeBoards are placed in a specific pattern for interlocalisation.

### Outputs

- STL files of the custom made part in order to 3D print them.
- DXF files of the custom 2D plate. A .swg and a .pdf was generated for each .dxf files with 0.001" paths with the colorRGB(255, 0, 0) . This can be used with a laser cutting machine.

