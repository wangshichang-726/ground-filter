# ground_filter

1、这是一个用于3D激光雷达识别和地面分割的ROS包的介绍，支持接收激光雷达点云，并进行地面分割处理，发出地面点云和非地面点云;  

2、本项目用于收集所有常用地面分割算法，或者我喜欢的有趣的地面分割算法;  

3、本项目从头开始，不仅仅copy别人的想法，会添加自己的改进，并重新合规编程。<br>

### Application package

You need clone the code.
```
$ mkdir -p catkin_ws/src
$ cd catkin_ws
$ catkin_make
$ cd src
$ git clone https://gitlab.com/wsc_726/ground_filter.git
$ cd catkin_ws
$ catkin_make
```
When you application this package, you need to modify the `"plane_ground_filter.launch"`, like `sensor_height` and so on.

```
$ source devel/setup.bash
$ roslaunch plane_ground_filter plane_ground_filter.launch
```
新开启终端打开RVIZ.
```
$ rviz
```
After you need set the frame to `velodyne`, and add two topic `filtered_points_no_ground` and `filtered_points_ground`.

### Example
![Screenshot 2019-06-21 09:54:30.png](https://i.loli.net/2019/06/21/5d0c391ee7a4e87595.png)
