# Tello-obstacle-avoidance



The code was created by Jaime Fernández. If any issues, contact me at fernandezelegidoj@gmail.com

The code created allows the drone to avoid an obstacle in its path, so that it can avoid it and avoid a collision. Once it has avoided it, the drone recovers the initial trajectory.

To achieve this, follow the steps below:

Execute the GET_TRACKBAR_VALUES code. Once this code is executed, a series of trackpads will be displayed on the screen to modify different parameters of the filters applied by the computational vision algorithm. These are really sensitive filters, so to achieve the correct identification of the obstacles these parameters must be changed every time the light conditions change. This values will be printed, get this values.
TUTORIAL: HOW TO KEEP WORKING IN THE PROJECT

In order to keep working with the project and improving it, here is a short tutorial of how to run the code and prepare everything:

Run the TELLO_FLIGHT code. Modify in this code the values referring to the filters in the code by values previously obtained. 
Modify the following values:
First, the obstacle that is going to be used needs to be measured. We will need its width and depth. Once this obstacle its measured we can run the first part of the code:

Run the file GET_TRACKBAR_VALUES , and automatically a new window will pop up, where you will be able to modify different parameters. Get the drone and make it face the obstacle you want to avoid. Modify this parameters until the different filters work correctly and the drone can identify the obstacle and other shapes in the route. 

Once the camera is correctly set up, we are ready to run the final code.

When you open the code, you will see this in the first lines:

values of the obstacl and security distance
obstacle_width = 50
@@ -29,3 +37,26 @@ threshold2 = 20

FOCAL ength of the camera
focal_length = 934.61

These are the parameters that should be modified to make the drone work correctly.
When this code is run, this is what we will see:

The trackbars, in the left part of the screen.

The following images:
Image 1: Image captured by the drone, no filters.
Image 2: Other filters applied to the image
Image 3: Image Blurried, grey scaled, canny edge detected and dilated. 
Image 4: Image 1, with the contours painted and other info included.

In case you are using a different drone than the one used here (RyzeTech Tello) the new focal length must be calculated.

To do so, load the GET_FOCAL_LENGTH file. You will need to stand at a measured distance in front of the drone, and take a picture. The algorithm will detect your face and calculate the focal length, however, you will have to modify the parameter measured_distance, and change it to the distance between your face and the drone when the picture was taken. Also, copy the path of your image here:

ref_image = cv2.imread("/YOUR_PATH")


Execute the GET_TRACKBAR_VALUES code. Once this code is executed, a series of trackpads will be displayed on the screen to modify different parameters of the filters applied by the computational vision algorithm. These are really sensitive filters, so to achieve the correct identification of the obstacles these parameters must be changed every time the light conditions change. This values will be printed, get this values.


Run the TELLO_FLIGHT code. Modify in this code the values referring to the filters in the code by values previously obtained. 
