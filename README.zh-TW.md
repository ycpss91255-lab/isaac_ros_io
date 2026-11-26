# isaac_ros_io

Isaac Sim 的 ROS 2 I/O 插件。負責模擬的全部 ROS 2 輸入與輸出：`/clock`、
`/joint_states`、`/joint_command`（依各關節 USD DriveAPI 的模式解讀），以及
感測器（相機、LiDAR、IMU），以 `isaacsim.ros2.bridge` 的 OmniGraph 節點建構。
isaac repo 本身不碰 ROS，在 play 前呼叫本插件。

請勿與 NVIDIA Isaac ROS（`isaac_ros_*`）混淆。

## 目前狀態

尚未發佈。`seed/` 下仍是從 isaac 抽出的種子程式碼，無法獨立執行。目標與驗證
項目見 [#3](https://github.com/ycpss91255-lab/isaac_ros_io/issues/3)；插件介面見
[#6](https://github.com/ycpss91255-lab/isaac_ros_io/issues/6)。

## 相依套件

- Isaac Sim 6.x
- ROS 2 Humble
- `isaacsim.ros2.bridge` extension

## 來源

從
[ycpss91255-lab/isaac @ c068e3a](https://github.com/ycpss91255-lab/isaac/tree/c068e3a)
依據 [issue #309](https://github.com/ycpss91255-lab/isaac/issues/309) 抽出。
於 [#4](https://github.com/ycpss91255-lab/isaac_ros_io/issues/4) 由 `isaac_ros2` 改名為 `isaac_ros_io`。

各檔案來源對照表見 [SOURCE.md](SOURCE.md)。

## 授權

[Apache-2.0](LICENSE)
