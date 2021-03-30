# Rover Iteration 2 Features

## Controller
Covers everything outside of autonomous control.

!!! Canbus-Layer
    Create an abstract Layer to improve canbus messaging between systems and modularity as well as documentation as code for handover purposes.

!!! Command-GUI
    Improved command GUI with integrated sensory information, arm and drive control capabilities and autonomous controls. Debug and console values should also be sent here.

!!! PID-Interface
    Help with the construction of a PID interface that all motors can use, help with integration to interface with arm and drive motor controllers.

## Autonomous

!!! Odometry-Localisation-and-Navigation
    Fuse all Odometry information and perform ekf localisation and navigation. Localise against a coordinate grid.

!!! Landmark-Localisation
    Perform AR Tag Detection on Realsense to determine distance. Localise against a coordinate grid, account for error in Odometry information.

!!! Obstacle-Detection-and-Avoidance
    Use LIDAR and Depth Camera to detect and avoid obstacles

!!! Slope-Detection
    Use Odom and Realsense to determine slopes the rover can attempt to climb.

## Jetson and Code Cleanliness

!!! Build-and-Deploy-Objects
    On Git push, code will be tested and deployed to the jetson via jenkins jobs. This would allow us to minify and optimise builds as well as keep hard drive size minimal. Would require: AWS Cloud services and JFrog Artifactory.

