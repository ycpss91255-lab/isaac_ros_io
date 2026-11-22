# Source

Seed code extracted from ycpss91255-lab/isaac @ c068e3a.

| Seed file | Origin |
|-----------|--------|
| seed/ros_io.py | framework/isaac_devkit/ros_io.py (full file, 395 lines) |
| seed/sensors_omnigraph.py | framework/isaac_devkit/sensors.py (full file, 756 lines; layer (b)+(c) OmniGraph + ROS 2 publish chains) |
| seed/driver.py | framework/isaac_devkit/driver.py (full file, 379 lines; contains rclpy init) |
| seed/config/fastdds.xml | config/ros2/fastdds.xml |
| seed/example/ | example/ros2/ (ROS 2 app packages: camera_subscriber, cmd_vel_publisher) |
| seed/test/test_ros_io.py | test/unit/pytest/test_ros_io.py |
| seed/test/test_sensor_setup.py | test/unit/pytest/test_sensor_setup.py |

This is seed code for the split described in ycpss91255-lab/isaac#309.
The code is NOT independently runnable yet -- it still depends on
isaac_devkit imports and Isaac Sim container. Refactoring to make it
standalone is the next step.
