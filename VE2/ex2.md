# Name
Jingyu Li

# Group Members
Jingyu Li
Shujing Yang
Siwei Zhang
Yutao Zhou
Yu Zhang

# Description
Cause the vehicle to brake after detecting a person (answers in teams of no more than five.
We have used python cv2 human detector for detection purpose. The detector will access every frame from the vehicle camera and detects whether pedestrians exist. When the detector cannot find person at first, the vehicle will move forward with an acceleration of 0.3. If there are pedestrians, the vehicle will brake and stop moving.

# Steps
## Step 1
Open the 1st terminal, launch the joystick controller
```
source devel/setup.bash
roslaunch basic_launch gem_dbw_joystick.launch
```
# Step 2

Open the 2nd terminal, launch the basic sensors
```
source devel/setup.bash
roslaunch basic_launch gem_sensor_init.launch
```

# Step 3
```
source devel/setup.bash
rosrun [PackageName] brake.py
```

# Video Link
https://youtu.be/Au7jVN3jaJU
