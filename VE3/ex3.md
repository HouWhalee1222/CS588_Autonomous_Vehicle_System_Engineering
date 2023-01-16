# Name
Jingyu Li

# Group Members
Jingyu Li
Shujing Yang
Siwei Zhang
Yutao Zhou
Yu Zhang

# Description
Either use an existing visual slam package or an existing visual odometry package to recover a representation of vehicle movement in the back lot.

# Usage
We used the hector slam package. You can install it with:
```
git clone https://github.com/tu-darmstadt-ros-pkg/hector_slam.git
```
Then compile it with `catkin_make`.<br>
<br>

Open the 1st terminal, launch hector slam.
```
source devel/setup.bash
roslaunch hector_slam_launch tutorial.launch
```
Open the 2nd terminal, play the prerecorded rosbag. (We used the data bag provided by TA, you can download it [here](https://uofi.app.box.com/s/gw38m6rz45c90qd5qikpccl55c6lk6z8))
```
source devel/setup.bash
rosbag play SampleRun_2022-10-31.bag /lidar1/scan:=/scan --clock -r 1.8
```

# Video Link
https://youtu.be/0PY2XPh1fyc
