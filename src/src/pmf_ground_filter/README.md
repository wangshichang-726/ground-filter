# pmf_fit_ground_filter---渐近形态学滤波地面分割算法

This is a ROS package for 3D lidar recognition and segmentation of ground, such as velodyne (VLP16) and robosense(16 channels) sensor.

### Application package

You need clone the code.
```
$ mkdir -p catkin_ws/src
$ cd catkin_ws
$ catkin_make
$ cd src
$ git clone https://github.com/walterchenchn/pmf_fit_ground_filter.git
$ cd catkin_ws
$ catkin_make
```
When you application this package, you need to modify the `"pmf_ground_filter.launch"`, like `sensor_height` and so on.

```
$ source devel/setup.bash
$ roslaunch pmf_ground_filter pmf_ground_filter.launch
```
In a new terminal.
```
$ rviz
```
After you need set the frame to `velodyne`, and add two topic `filtered_points_no_ground` and `filtered_points_ground`.

### Example
![Screenshot 2019-06-21 09:54:30.png](https://i.loli.net/2019/06/21/5d0c391ee7a4e87595.png)
