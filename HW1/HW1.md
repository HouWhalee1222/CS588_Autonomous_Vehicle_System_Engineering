# Name
Jingyu Li

# Group Members
Jingyu Li
Shujing Yang
Siwei Zhang
Yutao Zhou
Yu Zhang

# Description
In this HW, we implemented PID controller to follow waypoints along a path on the simulator. The codes file we modified include `pid.py` and `follow_waypoints.py`. We have filled the "TODO" parts. Main tasks done: 
- transforming the goal point into the vehicle coordinate frame in function `start_drive`
- define feedback value for PID control in function `start_drive`
- Set own sets of weights for P, I, D terms in `__init__`.

Running results are shown in the provided movie.

# Steps
## Step 1. Launch track 1 environment in the simulator
```
source devel/setup.bash
roslaunch gem_launch gem_init.launch world_name:="track1.world" x:=0 y:=-2
```

## Step 2. Run follow_waypoints file to let the car move in the middle of the road
```
source devel/setup.bash
rosrun gem_waypoint_pid follow_waypoints.py
```

# Video Link
https://youtu.be/GPDPIF34peI
