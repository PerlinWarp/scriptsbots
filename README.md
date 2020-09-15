# SCRIPTBOTS
Author: Andrej Karpathy  
Contributors: Casey Link, Peter Walkington  
Licence: BSD  
  
Project website and attached forum:   
https://sites.google.com/site/scriptbotsevo/home  
  
------------------------------------------------------

## BUILDING:
To compile scriptbots you will need:

CMake >= 2.8 (http://www.cmake.org/cmake/resources/software.html)  
OpenGL and GLUT (http://www.opengl.org/resources/libraries/glut/)  
Linux: freeglut (http://freeglut.sourceforge.net/)  
It will use OpenMP to speed up everything, in case you have multicore cpu.  
  
If you are on Ubuntu (or debian) you can install all the dependencies with:  
```
$ sudo apt-get update
$ sudo apt-get install libglu1-mesa-dev freeglut3-dev mesa-common-dev
$ apt-get install cmake build-essential libopenmpi-dev libxi-dev libxmu-dev
```

### To build ScriptBots on Linux:
```
$ cd path/to/source
$ mkdir build
$ cd build
$ cmake ../ # this is the equiv of ./configure
$ make

To execute ScriptBots simply type the following in the build directory:
$ ./scriptbots
```

### For Windows:
Follow basically the same steps, but after running cmake open up the VS solution (.sln) file it generates and compile the project from VS.

## Controls:

* p = pause  
* d = toggle drawing (for faster computation)  
* f = toggle drawing food
* \+ = run faster
* \- = run slower
  
Move around the world by holding down the right mouse button and dragging.   
Zoom by holding down the middle mouse button and dragging the mouse up or down.   
Click on an agent to display its stats.   