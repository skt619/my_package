Download the package in ~/ros_ws/src
colcon build
source install/local_setup.bash
ros2 launch my_package robot_launch.py

For the outdoor world, daytime is:
Viewpoint -> TexturedBackgroundLight
set value to 1
night is:
Viewpoint -> TexturedBackgroundLight
set value to 0
