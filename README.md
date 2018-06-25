# Snake-Game
It is Graphical Snake Game on linux based machine. It is developed in C using OpenGL.
    
## Getting Started:
Here I will tell you about OpenGL and How to install and run the OpenGL project?

### OpenGL 
Open Graphics Library (OpenGL) is a cross-language, cross-platform application programming interface (API) for rendering 2D and 3D vector graphics. 


## About Project:
It is a Game where snake is moving on sceen. You have control to change the direction of snake. Real Game is that you have to increase our snake size and depending upon snake size score will be display. To increase snake size your snake have to eat food which will display randomly one by one on screen and if you eat your score will increase by one.You can also change the level from 1 to 9. Depending upon level snake speed will increase. Level 1 snake speed will be more than level 9 means 1 is highest level and 9 is lowest level

### Project Statistic
- **Description** : Snake game using OpenGL
- **Technology**  : C and OpenGL
- **Platform**    : Linux , Mac

### How we have done?
  We have use C language with OpenGl. We have use Double Circular link list to store (x,y) point of each cell of snake because we have no idea how much snake cell will be.

## To Run This Project (Game):
	
### You must have openGL install in your computer. 
Below are instructions to install openGL on Ubuntu based Operating System. Put the below command on Linux Terminal.

	sudo apt-get update
	sudo apt-get upgrade
	sudo apt-get install freeglut3
 	sudo apt-get install freeglut3-dev
	sudo apt-get install binutils-gold
 	sudo apt-get install g++ cmake
	sudo apt-get install libglew-dev
 	sudo apt-get install g++
 	sudo apt-get install mesa-common-dev
 	sudo apt-get install build-essential
 	sudo apt-get install libglew1.5-dev libglm-dev

### Command to execute this project 	 	
	
	g++ GameHeader.h
	g++ snake.c -lGL -lGLU -lGLEW -lglut -o startGame
	./startGame



## Function Used in Project:

### I] Header Function
	
1. `#include<stdio.h>`		: For Standard Input and output	( printf , scanf )

2. `#include <stdlib.h>`	: For Standard Libaray	( malloc  , rand , srand)

3. `#include <time.h>`		: For Time function	( nanosleep )

4. `#include <GL/gl.h>`		: Provides basic set of functions
	
5. `#include <GL/glu.h>`	: Provides high level functions

6. `#include <GL/glut.h>`	: Opening windows , managing menus and manging events

### II] Graphic Inbuilt Function We Have use?

1. `glutInit(&argc, argv);`  Initializes the grahics toolkit

2. `glutInitDisplayMode(GLUT_SINGLE|GLUT_RGB);` Single display buffer and RGB mode

3. `glutInitWindowSize(640,480);` Initial window size

4. `glutInitWindowPosition(800,300);` Initial position of windows left corner

5. `glutCreateWindow("Snake Game");` Opens a window with title

6. `glutDisplayFunc(mydisplay);` Registering the display function

7. `glutSpecialFunc(mySpecialKeyboard);` Registering the special keyboard  function ( like arrow key)

8. `glutKeyboardFunc(myKeyboard);` Registering the keyboard function

9. `glClearColor(0.127, 0.252, 0.0, 0.0);` Set the background color

10. `glClear(GL_COLOR_BUFFER_BIT);` Clear the entire window to background color

11. `glFlush();` The entire data is to be processed and sent for display

12. `glColor3f(0.0, 0.0, 0.0);` Set the drawing color to black;

13. `glRecti( x-5 ,  y-5 , x+5 , y+5 );`  Draw the rectangle on screen 

14. `glBegin(GL_TRIANGLES);` Specifies a set of points of triangle

15. `glVertex2i(x,y);` Giving the point with two integer arguments

16. `glutPostRedisplay();` Recall callback function
