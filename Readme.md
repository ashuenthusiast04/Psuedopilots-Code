# *SETUP OF THE ENVIRONMENT*

We will be having a mobile camera(in this case we are using the open-source DroidCam Client connected through common wifi network between mobile device and laptop) mounted on the top of the arena (here on the stair of a ladder) which will be taking live feed of the dynamic environment of the arena and feed each frames to the path algorithm code. In each frames, we will be having some obstacles in the arena and two arucos, one representing the robot and the other representing the stack.

# *WORKING OF ARUCO MARKER*

Two Aruco markers of known ids were generated and printed from an online resource. Then, using the opencv-contrib-python library which has the cv2.aruco library, programming it for the ORIGINAL_ARUCO markers, we are able to identify the markers in the frame received and are able to write code to get the coordinates of the corners, centers of the markers and the orientation or the polar angle of the markers in degrees. Using all of this data we have written the code such that aruco on the robot makes the robot chase the aruco on the stacks in the same frame. Hence, making the movement of the robot autonomous.
