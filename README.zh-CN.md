# isaac_ros2

Isaac Sim ROS 2 bridge -- OmniGraph 传感器发布链 (camera, LiDAR, IMU)
及输入端 topic 订阅 (cmd_vel)，用于 Isaac 仿真环境。

## 概述

从 [ycpss91255-lab/isaac](https://github.com/ycpss91255-lab/isaac)
([#309](https://github.com/ycpss91255-lab/isaac/issues/309))
抽取的 ROS 2 集成层。

负责构建 OmniGraph action graph，将传感器数据发布至 ROS 2 topic，
并订阅输入端命令。

## 当前状态

Seed code 阶段。尚无法独立运行。依赖 Isaac Sim 容器及 `isaac_devkit` 框架。

## 依赖

- Isaac Sim 6.x
- ROS 2 Humble
- `isaacsim.ros2.bridge` extension

## 来源

从
[ycpss91255-lab/isaac @ c068e3a](https://github.com/ycpss91255-lab/isaac/tree/c068e3a)
依据 [issue #309](https://github.com/ycpss91255-lab/isaac/issues/309) 抽取。

各文件来源对照表见 [SOURCE.md](SOURCE.md)。

## 许可证

[Apache-2.0](LICENSE)
