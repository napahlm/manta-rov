# Manta
"Manta" is the name of the ROV given by Vortex NTNU at the time of construction in 2017.
It has competed in ROV and AUV competitions internationally, and is now mainly used and maintained as a ROV.

# The ROV Control System
This repo contains the necessary ROS packages for controlling the underwater drone physically.

## Launch files
Launch files are called with the `roslaunch` command and contains a specific set of packages meant to do a specific task. Usually differentiated between physical operation and simulator operation.


**Usage:**

`roslaunch   package_name launch  _file.launch`

**Files:**

simulator.launch

&nbsp;&nbsp;&nbsp;&nbsp; *Launches the barebone control structure necessary for simulator control of Manta.*
  
manta.launch

&nbsp;&nbsp;&nbsp;&nbsp; *Launches all the necessary packages for normal physical operation of Manta.*

## Packages
The function of the packages are designed as a traditional closed loop feedback system.

The measured states are the depth and orientation of the ROV determined by the setpoint given by the a joystick.

*Add the feedback loop image*.

