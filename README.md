# Turtlebot-Mechanical-Update

This repository contains the 3D model of a modified Turtlebot Burger used by the SwarmUS project.

## Requirements
- Solidworks 2021

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
├── pioneer2DX.SLDASM
└── README.md
```

#### Turtlebot_modified.SLDASM

Main assembly of the modified Turtlebot. It's composed of a Turtlebot Burger with additionnal components that are external to the robot (*external*) and of components that are internal to the robot (*internal*). These components wrre mostly added to support mechanically and electrically the HiveBoard and its BeeBoards.

### Turtlebot

This folder contains all the components of the Turtlebot and it contains the Turtlebot's assembly itself. All the components and the assembly were exported from the Robotis Model on [OnShape](https://cad.onshape.com/documents/2586c4659ef3e7078e91168b/w/14abf4cb615429a14a2732cc/e/9ae9841864e78c02c4966c5e) and was converted to a SolidWorks assembly afterwards.

### external

Contains the 3D models of the external components and their supports.


### internal

Contains the 3D models of the internal components added to the Turtlebot.

- **REG_313080006.SLDPRT**: 313080006 5V regulator for powering the Hiveboard and its BeeBoards.

### Outputs

- STL files of the custom made part in order to 3D print them.
- DXF files of the custom 2D plate. A .swg and a .pdf was generated for each .dxf files with 0.001" paths with the colorRGB(255, 0, 0) . This can be used with a laser cutting machine.

