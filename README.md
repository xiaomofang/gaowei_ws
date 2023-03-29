# 编译
catkin_make
source devel/setup.bash

#１．首先运行gazebo仿真环境
```
roslaunch urdf02_gazebo demo03_env.launch 
```
#2.然后执行launch文件,自主移动的SLAM建图；
```
roslaunch nav_demo nav07_slam_auto.launch 
```
###3.运动方式－－键盘控制小车运动
```
rosrun teleop_twist_keyboard teleop_twist_keyboard.py 
```

###保存地图
```
 roslaunch nav_demo nav02_map.launch 
```
###启动地图服务
```
roslaunch nav_demo nav03_map_server.launch 
```





