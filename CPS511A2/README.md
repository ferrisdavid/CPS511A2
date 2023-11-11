# CPS511 A2
This project implements all required functionality and requirements as outlined in the CPS511 A2 Requirements Document.

NOTE: The dark spots present in the mesh are a result of a strange lighting and shading issue that has been affecting the Mac users. The professor has stated that this should not effect marking.

In addition, due to an issue affecting macs usage of VAOs the VBO Mesh drawing has been implemented using only VBOs as per the assignment requirements.

## Compilation Note: 
This project was built and compiled on Mac OS, as such the associated makefile has only been tested on a Mac 
Machine (OS X) and I cannot guarantee its function on other platforms. The linked and imported libraries have also only been tested on Mac. If you are looking to compile and run this program (surfaceModeller.cpp) on another platform please adjust the imported libraries where necessary and compile using the method that works for your platform.

## Usage:
- Increase/Decrease Control Points: Up/Down Arrows in 2D Window
- Scale Mesh: In 3D Window, Right Click Drag-In to Shrink or Drag-Out to Expand (in z-direction)
- Camera Control: In 3D Window, Drag Mouse in horizontal direction to rotate camera around mesh around Y-axis, Shift Drag mouse up/down to control camera elevation angle