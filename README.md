# ros_object_detector

This package uses Tensorflow to power an object detection and localization algoriithm (built by the user) located in the "include/obj_detector" folder. 
The main script that does the heavy lifting, "src/tf_object_detector.py", looks for a /camera1/cam1/image_raw node to subscribe to, performs detection and localization, and republishes the image with bounding boxes.

This is an alpha, "it works on my laptop" release.

#TODO

- Publish all the data returned by tensorflow (classifications, probabilities, box coordinates, etc)
- Make python file available through rosrun
- Make python file not dependent on being executed in its directory
- Add msg files for the different node publications
- Make parameters (model location, buffer size, camera node, etc.) configurable at runtime instead of hard-coded 
- Make parameters definable in a parameter file
- Edit roslaunch to execute all relevant objects, not just the camera

Any feedback is welcome. Submit code to github, and contact me directly at dbrown@byu.net

