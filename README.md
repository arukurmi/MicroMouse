# About_MicroMouse

The micromouse robot, as per the international micromouse competition regulations, should be completely autonomous, should traverse the maze by itself while discovering the walls and mapping them in the memory. At the time of placing the robot on the maze, only the starting position and the destination position with respect to the starting position is known by the robot. 


## Getting started with the algorithm

We represented the maze as a 2D array of size 16*16, initiated with zeros. We’ll call it the maze array.
While the robot is in the maze, it can moving while facing towards four directions (orientations). To represent this in the algorithm, we used a variable Orient to store one of the four values; 0,1,2,3. Every time the robot performs a turn, the orient variable is updated.

