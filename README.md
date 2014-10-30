Layered-3D-Display-Case
=======================

CAD files for a handheld layered 3D-display based on three transparent OLED-displays.

Introduction
============

This project contains all CAD files needed to build the layered 3D-display prototype described in [1] and [2]. All files are in the Autodesk Inventor file format. For easy 3d printing, STL files for all parts exported from Inventor are supplied in the STL directory.
The main case consists of six layers which are printed separately. An explosion drawing of the display is provided here: https://raw.githubusercontent.com/patrigg/Layered-3D-Display-Case/master/pictures/explosion_rendering.png
It consists of the following parts (from front to bottom):
- TouchTop
- DisplayTop
- DisplayMid1
- DisplayMid2
- DisplayBottom
- TouchBottom
The middle display layer is split into two parts DisplayMid1 and DisplayMid2 to allow the actual display to be placed in the middle of the layer. Both parts are exportet from the same DisplayMid.ipt file using the split plane in the Inventor file.

Additionally model files to build a plug are also provided: PlugFront and PlugMiddle. 

Getting Started
===============

Prerequisites:
 - 2 Nintendo DSL Digitizers (http://www.exp-tech.de/Displays/Touch-screen-Nintendo-DSL-digitizer.html)
 - 2 breakout boards for the digitizers (http://www.exp-tech.de/Shields/Touch-screen-breakout-board-0-5mm-FPC.html)
 - 3 µTOLED_20_G2 from 4D Systems (http://www.4dsystems.com.au/product/uTOLED_20_G2/ discontinued product :( )
 - some male and female headers
 - some cable
 - soldering iron
 - glue
 
To build the prototype, first print all the 3d models provided in the STL directory. Attach the displays to the according layers. Then, desolder the headers from the display controller boards and replace them with wires. Beware: This will void warranty! Route the wires along the notches, cut them to the required length and add one row of female headers and push them into the printed frame.The result is shown in the following picture:
https://raw.githubusercontent.com/patrigg/Layered-3D-Display-Case/master/pictures/partially_assempled.jpg
Next, attach the breakout boards for the digitizers to the DisplayTop and DisplayBottom Layers. Solder wires to the breakout boards and also route them along the notches. Like before add female headers.
Now the display can be assembled: First press the digitizers into the frame. Connect the breakout boards by aligning the top and bottom display layer to the touch layers. This part is a bit tricky since the cables of the digitizers are quite short.
Now put the remaining layers together in the order shown in the explosion drawing above. The TouchTop layer can be clipped into the TouchBottom layer.

To assemble the plug, print the respective parts. Afterwards glue some male headers into the hollows and solder wires onto them.

If everything worked out, your prototype should look something like the one shown here:
https://raw.githubusercontent.com/patrigg/Layered-3D-Display-Case/master/pictures/prototype.jpg

[1] P. Bader, S. Schneegass, N. Henze, V. Schwind, and K. Wolf, “A Mobile See-through 3D Display with Front- and Back-touch,” in Proceedings of the 8th Nordic Conference on Human-Computer Interaction: Fun, Fast, Foundational, New York, NY, USA, 2014, pp. 1063–1066. http://doi.acm.org/10.1145/2639189.2670276

[2] P. Bader, V. Schwind, N. Henze, S. Schneegass, N. Broy, and A. Schmidt, “Design and Evaluation of a Layered Handheld 3D Display with Touch-sensitive Front and Back,” in Proceedings of the 8th Nordic Conference on Human-Computer Interaction: Fun, Fast, Foundational, New York, NY, USA, 2014, pp. 315–318. http://doi.acm.org/10.1145/2639189.2639257
