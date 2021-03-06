---
title: kicadPanelizer
description: KiCAD PCB panelization helper
author: C. Riehl
tags: KiCAD, PCB, EDA, electronics
created:  2015.10.09
modified: 2015.10.09

---

kicadPanelizer
=======
## Introduction

kicadPanelizer is a program for fast automatic PCB panelization proces. That's what people have been doing so far manually, sometimes wasting a lot of time, using the "Join plate" option, it is now achievable by a few clicks.

## The basic features of the software:
- script based

- step repeat on both dimensions

- Rotation

- adds common panel elements from separate file to ease panel composition (for stuff that cannot be repeated, like tooling frame, fiducials, etc...)

- substitutes the text "##PCBNUMBER##" anywhere on the PCB with an incremental number (so the board number can be located even after separation if necessary)

- works with complex board shapes, rotations, v-scoring or routing.

- demo project included with v-score, routing, tooling frame example


Some output from the included demo project:

![output](https://github.com/f4eru/kicadPanelizer/tree/master/demo_files/output/demo_layout-panelized-layerstack_Front.pdf)

This one program is designed as a maximum to facilitate as much as possible.

## Installation & configuration
Unpack newest release to prefered dir.

Unix based OS user can set execute privileges to execute as any other shell script:
> chmod +x generate_panelized_pcb.py

## Running initially testing script.
From command line in dir with script:
> ./generate_panelized_pcb.py

or simply double click on the file to execute it

To run it it's nessesary to install:
- [Python interpreter] in version 2 (On today newests is 2.7.8). Don't miss with version 3 (On today newests is 3.4.1).
- [KiCAD] compiled with allowed python scripting. Minimum BZR version is 5161.
- [GTK Libraries].
[Python interpreter]: https://www.python.org/downloads/
[KiCAD]: http://kicad-pcb.org/
[GTK Libraries]: http://www.gtk.org/download/


TO DO:
- readapt to GUI as original project did
