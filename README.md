# meshing
An interactive application for sculpting in 3D. 

Distance functions defining the surface of a shape can be added additively and subtractively to form complex shapes.
Functions are added to an octree which causes affected areas to be re-evaluated.
Function evaluation consists of iterating over a hierarchical grid to find distances smaller than some threshold.
Zero-crossing points are collected and uploaded to an openGL vertex buffer, then drawn.

__[Video](https://www.youtube.com/watch?v=L7l1_QjAOaE)__

__Controls:__
* mouse movement: look around
* left click: apply brush additively
* right click: apply brush subtractively
* 1 key: toggle between sphere and cube brushes
* Up Arrow, Down Arrow: increase or decrease brush size
* 3 and 4 keys: increase and decrease brush fidelity
* WS: forward and backward
* AD: left and right
* left shift, space: down and up

__Dependencies:__
* OpenGL 4.3
* glew
* glfw3
* glm
* c++11 compiler
* cmake
  
__Building:__
* mkdir build
* cd build
* cmake .. -G <your platform>
* cd ..
* cmake --build build --config Release

__Running:__
* cd bin
* ./main <width> <height> 


![alt tag](http://i.imgur.com/fyDl3kW.png)
