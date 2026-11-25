# isaac_ros2

Isaac Sim ROS 2 bridge -- OmniGraph sensor publish chains (camera, LiDAR, IMU)
and inbound topic subscription (cmd_vel) for the Isaac simulation environment.

## Overview

ROS 2 integration layer extracted from
[ycpss91255-lab/isaac](https://github.com/ycpss91255-lab/isaac)
([#309](https://github.com/ycpss91255-lab/isaac/issues/309)).

Handles OmniGraph action graph construction for publishing sensor data to
ROS 2 topics and subscribing to inbound commands.

## Current Status

Seed code stage. Not independently runnable. Depends on the Isaac Sim
container and the `isaac_devkit` framework.

## Dependencies

- Isaac Sim 6.x
- ROS 2 Humble
- `isaacsim.ros2.bridge` extension

## Origin

Extracted from
[ycpss91255-lab/isaac @ c068e3a](https://github.com/ycpss91255-lab/isaac/tree/c068e3a)
per [issue #309](https://github.com/ycpss91255-lab/isaac/issues/309).

See [SOURCE.md](SOURCE.md) for per-file provenance.

## License

[Apache-2.0](LICENSE)
