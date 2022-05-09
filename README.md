# Tello-obstacle-avoidance

The code was created by Jaime Fernández. If any issues, contact me at fernandezelegidoj@gmail.com

The code created allows the drone to avoid an obstacle in its path, so that it can avoid it and avoid a collision. Once it has avoided it, the drone recovers the initial trajectory.

To achieve this, follow the steps below:

Execute the GET_TRACKBAR_VALUES code. Once this code is executed, a series of trackpads will be displayed on the screen to modify different parameters of the filters applied by the computational vision algorithm. These are really sensitive filters, so to achieve the correct identification of the obstacles these parameters must be changed every time the light conditions change. This values will be printed, get this values.


Run the TELLO_FLIGHT code. Modify in this code the values referring to the filters in the code by values previously obtained. 
Modify the following values:

values of the obstacl and security distance
obstacle_width = 50
obstacle_depth =100
sec_distance = 20
Filter values obtained from GET_TRACKBAR_VALUES

h_min = 33
h_max = 179
s_min = 0
s_max = 179
v_min = 89
v_max = 136
threshold1 = 20
threshold2 = 20

FOCAL ength of the camera
focal_length = 934.61
