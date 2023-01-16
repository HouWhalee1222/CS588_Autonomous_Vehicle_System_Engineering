# Name
Jingyu Li

# Group Members
Jingyu Li
Shujing Yang
Siwei Zhang
Yutao Zhou
Yu Zhang

# Description
Use the codebase for GPS and waypoints which Hang Cui has kindly let us use ( gzipped tarfile) and your skill and judgement to cause the vehicle to follow a figure 8 path on the outdoor track.

# Steps
## Step 1: Record the figure 8 path
Open the 1st terminal, launch the joystick controller.
```
source devel/setup.bash
roslaunch basic_launch gem_dbw_joystick.launch
```

Open the 2nd terminal, launch the basic sensors.
```
source devel/setup.bash
roslaunch basic_launch gem_sensor_init.launch
```

Open the 3rd terminal and let the safty driver drive the vechicle in a figure 8 path.
```
source devel/setup.bash
rosrun gem_waypoint_pid follow_waypoints.py
```

## Step 2: Control the vechicle to follow the figure 8 path automatically
Open the 1st terminal, launch the joystick controller.
```
source devel/setup.bash
roslaunch basic_launch gem_dbw_joystick.launch
```

Open the 2nd terminal, launch the basic sensors.
```
source devel/setup.bash
roslaunch basic_launch gem_sensor_init.launch
```

Open the 3rd terminal and and let the computer controls the vechicle.
Make sure you use the `fig8.csv` as the waypoints source.
```
source devel/setup.bash
rosrun gem_waypoint_pid follow_waypoints.py
```

# Video Link
https://youtu.be/pZCcuCtHEs8
