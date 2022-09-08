![](https://github.com/maHidaka/ros_face/workflows/PlatformIO%20CI/badge.svg)
![](https://github.com/maHidaka/ros_face/workflows/ROS1%20melodic/badge.svg)

# ROS-Face

ROS-Face is a project that aims to manipulate human facial muscles using the ros system.
You can control human facial expressions just as you would control a robot.

![ezgif-1-83660fbc68](https://user-images.githubusercontent.com/50083939/163762617-173b62d3-3896-47a3-9797-691d194df25e.gif)

Demo movie
https://www.youtube.com/watch?v=VLdtHsNA5pQ

# ATTENTION
maHidaka is not responsible for any accidents or damages caused by this project. Use of this code is at your own risk and is subject to the BSD2-Clause license.

## setup

### install rosserial

The ros environment must have been established in advance.
We have already confirmed that it works with melodic. Other versions may also work.

```
sudo apt install ros-melodic-rosserial-arduino
sudo apt install ros-melodic-rosserial
```


### Schematic
![97066d7b3dbf9945d558fdc4049416ad](https://user-images.githubusercontent.com/50083939/163585114-51e26d90-7f34-4871-91ee-c89b9eb7086b.png)


### Upload sketch to Arduino Uno

Main sketch is here "ROS_FACE/ros_face_Arduino/src/main.cpp".

Upload this sketch to arduino using platformio.
For more information about platformio and how to upload the sketch using ArduinoIDE, please refer to the instructions on another site.


## Example usage

1. ``` cd catkin_ws/src```
1. ```git clone https://github.com/maHidaka/ros_face.git```
1. ```catkin build```
2. ```roslaunch ros_face_apps face_control_joy.launch```
