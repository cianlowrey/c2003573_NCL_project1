Portfolio 1
===========

This package is build as a part of the CSC1034: Portfolio-1.

The premise of the project is to create a 3D Panda that has optional additions to make the scene interactable.

Without any changes, the default environment shows a camera rotating around a walking panda, situated in a forest/jungle. This panda is scaled to the forest proportionally, and the camera consistently circulates around the panda. 

walking_panda.py takes the cli() function from cli.py to play the code. The cli.py itself takes the class WalkingPanda from panda.py, creating another dependency. cli.py takes all the argparse arguments for how to change the animation accordingly. panda.py holds the class for the WalkingPanda and takes on all the variables to create the actual scene in of itself.

spinCameraTask() takes on the argument of "--no-rotate" which if returns False, the camera rotates as normal. If it returns True, the camera remains at its original position.

scaleUp() and scaleDown() work in the same way. If given the argument of "--scale-up", it doubles the size of all 3 dimensions of the panda, with "--scale-down" halving the dimensions.

setScaleUp() and setScaleDown() also work in a proportionally same way. With the arguements of "--set-scale-up" and "--set-scale-down" doubling or halving the size of the background screen accordingly.
