these are the modified turtlebot4 files for Alan Federmens gopher2,

as expalined in the mockBot documents:

It consists of these modified files.

turtlebot_bringup.sh

-----
ros2 launch turtlebot4_bringup mock.launch.py &
ros2 launch ldlidar_stl_ros2 ld19.launch.py &
ros2 launch laser_filters footprint_filter_example.launch.py &
------

The lidar files are buit in ros2_ws using colcon, the laser filters from
sudo apt install.

mock.launch.py is modified from the turtlebot4 bringup lite.launch.py


The ros2_ws/src/turtlebot4/turtlebot4_description is included as a tar.gz files
and has added meshes and modified urdf'sncluding for my odd shaped table and the ld19 lidar.

Finally, the oakd_lite.yaml file in bringup/config has frame rate and picture size reduced for slower networks. 
