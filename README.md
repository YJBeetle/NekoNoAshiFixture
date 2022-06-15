# Neko Paw Shaped Test Point
This repository contains a "Neko Paw" Shaped Test Point design files, include KiCad Footprint and FreeCad test point clip design file.

![footprint](https://user-images.githubusercontent.com/8038511/173807471-f3634d36-5d1a-4202-bad3-2db55b7f6b24.png)

## KiCad Footprint
In the `Local.pretty` folder, there are two type of KiCad footprint. 

 * If you don't need vias, you can use `meow.kicad_mod`. This is the one-side footprint without vias,
 * If you need double side connection or multiple layers of board, `meow_hole.kicad_mod` contains vias on the "claw tips" of neko paw, it can make your "neko paw" more beautiful with vias.

All footprints contains dowel pin on Edge Cuts. The footprint without dowel pin is on the way.

## Connector
Of course, this repository contains connector for neko paw test point. Both of them need pogo pin to assemble.

We high recommend to use 1.0mm needle bar diameter with 0.74mm tip diameter pogo pin with round tip, such as PAL75-J, if you use sharp tip, it may harm your PCB tin layer.

There are two type of connector.

### Test Needle Connector
Test Needle connector is a handheld connector. This type of connector is good for programming a lot of chips.

You can find PCB design files in the `TestNeedle` folder.

### Clip connector
Clip connector is a good way to persistent connection to the PCB, such as debug your chip, `Clip` folder contains a FreeCAD design file `Fixture.FCStd`, you can 3D print this file with PETG or other sturdy print material. And the supplementary PCB design is also provided in the `Clip` folder.

![Clip](https://user-images.githubusercontent.com/8038511/173806358-feefa180-b81d-44e4-99a9-08597d6d76a1.png)
