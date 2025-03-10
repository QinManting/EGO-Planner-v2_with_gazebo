# EGO-Planner-v2_with_gazebo

适用于agc系统gazebo仿真的无人机单机规划

## Installation

Ubuntu 20.04安装ROS，参照官网（https://www.ros.org.）

## Build

```
git clone https://github.com/QinManting/EGO-Planner-v2_with_gazebo.git
cd EGO-Planner-v2_with_gazebo/main_ws
catkin_make
```

## Run

运行QGC，使无人机起飞

Terminal 1
```
cd path_to_your_ws/
source devel/setup.bash
roslaunch ego_planner rviz.launch
```

Terminal 2
```
cd path_to_your_ws/
source devel/setup.bash
roslaunch ego_planner single_drone_exploration.launch 
```

使用QGC切换到offboard模式，无人机即可开始按照规划路径飞行
