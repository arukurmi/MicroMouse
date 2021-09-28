### About_MicroMouse

The micromouse robot, as per the international micromouse competition regulations, should be completely autonomous, should traverse the maze by itself while discovering the walls and mapping them in the memory. At the time of placing the robot on the maze, only the starting position and the destination position with respect to the starting position is known by the robot. 


### Getting started with the algorithm

We represented the maze as a 2D array of size 16*16, initiated with zeros. We’ll call it the maze array.
While the robot is in the maze, it can moving while facing towards four directions (orientations). To represent this in the algorithm, we used a variable Orient to store one of the four values; 0,1,2,3. Every time the robot performs a turn, the orient variable is updated.

Next we assigned different numbers to different configurations of walls a square can have. There can be 16 different combinations of walls (including a square with all four walls, and with no walls at all).

The numbers given to different wall configurations
As the mouse traverses through the maze, it can detect if a walls present to the left, right or in front of it, with the use of it’s distance sensors. Next, depending on the availability of a wall to the left, right or front of the mouse, and the mouse’s orientation while in the cell, we updated the corresponding entry in the maze array by its wall configuration.
These 16 combinations were also categorized according to the presence of a wall to the left, right, up and down in a square.
