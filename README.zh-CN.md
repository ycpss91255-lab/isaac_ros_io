# isaac_ros_io

Isaac Sim 的 ROS 2 I/O 插件。负责仿真的全部 ROS 2 输入与输出：`/clock`、
`/joint_states`、`/joint_command`（按各关节 USD DriveAPI 的模式解读），以及
传感器（相机、LiDAR、IMU），以 `isaacsim.ros2.bridge` 的 OmniGraph 节点构建。
isaac repo 本身不涉及 ROS，在 play 前调用本插件。

请勿与 NVIDIA Isaac ROS（`isaac_ros_*`）混淆。

## 当前状态

尚未发布。`seed/` 下仍是从 isaac 抽出的种子代码，无法独立运行。目标与验证
项目见 [#3](https://github.com/ycpss91255-lab/isaac_ros_io/issues/3)；插件接口见
[#6](https://github.com/ycpss91255-lab/isaac_ros_io/issues/6)。

## 依赖

- Isaac Sim 6.x
- ROS 2 Humble
- `isaacsim.ros2.bridge` extension

## 来源

从
[ycpss91255-lab/isaac @ c068e3a](https://github.com/ycpss91255-lab/isaac/tree/c068e3a)
根据 [issue #309](https://github.com/ycpss91255-lab/isaac/issues/309) 抽出。
于 [#4](https://github.com/ycpss91255-lab/isaac_ros_io/issues/4) 由 `isaac_ros2` 更名为 `isaac_ros_io`。

各文件来源对照表见 [SOURCE.md](SOURCE.md)。

## 许可证

[Apache-2.0](LICENSE)
