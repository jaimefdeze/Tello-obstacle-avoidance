# Tello-obstacle-avoidance

The code was created by Jaime Fernández. If any issues, contact me at fernandezelegidoj@gmail.com

The code created allows the drone to avoid an obstacle in its path, so that it can avoid it and avoid a collision. Once it has avoided it, the drone recovers the initial trajectory.

To achieve this, follow the steps below:

Execute the GET_TRACKBAR_VALUES code. Once this code is executed, a series of trackpads will be displayed on the screen to modify different parameters of the filters applied by the computational vision algorithm. These are really sensitive filters, so to achieve the correct identification of the obstacles these parameters must be changed every time the light conditions change.

Run the TELLO_FLIGHT code. Modify in this code the values concerning the filters in the code by ovals obtained previously. 
Modify the value real_width with the width of the obstacle to avoid.
