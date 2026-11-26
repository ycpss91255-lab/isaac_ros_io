# isaac_ros_io

ROS 2 I/O plugin for Isaac Sim. It owns all ROS 2 input and output of the
simulation: `/clock`, `/joint_states`, `/joint_command` (interpreted by
each joint's USD DriveAPI mode), and sensors (camera, LiDAR, IMU), built from
OmniGraph nodes of `isaacsim.ros2.bridge`. The isaac repo itself does not
touch ROS; it calls this plugin before play.

Not to be confused with NVIDIA Isaac ROS (`isaac_ros_*`).

## Current Status

Pre-release. The code under `seed/` is still the seed extracted from isaac
and is not runnable on its own. Targets and verification items:
[#3](https://github.com/ycpss91255-lab/isaac_ros_io/issues/3); plugin interface:
[#6](https://github.com/ycpss91255-lab/isaac_ros_io/issues/6).

## Dependencies

- Isaac Sim 6.x
- ROS 2 Humble
- `isaacsim.ros2.bridge` extension

## Origin

Extracted from
[ycpss91255-lab/isaac @ c068e3a](https://github.com/ycpss91255-lab/isaac/tree/c068e3a)
per [issue #309](https://github.com/ycpss91255-lab/isaac/issues/309).
Renamed from `isaac_ros2` to `isaac_ros_io` in
[#4](https://github.com/ycpss91255-lab/isaac_ros_io/issues/4).

See [SOURCE.md](SOURCE.md) for per-file provenance.

## License

[Apache-2.0](LICENSE)
