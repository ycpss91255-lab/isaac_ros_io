# isaac_ros_io

Isaac Sim 向けの ROS 2 I/O プラグイン。シミュレーションの ROS 2 入出力をすべて
担当する：`/clock`、`/joint_states`、`/joint_command`（各関節の USD DriveAPI の
モードに従って解釈）、およびセンサー（カメラ、LiDAR、IMU）。`isaacsim.ros2.bridge`
の OmniGraph ノードで構築する。isaac repo 自体は ROS を扱わず、play 前に本
プラグインを呼び出す。

NVIDIA Isaac ROS（`isaac_ros_*`）とは別物。

## 現在の状態

未リリース。`seed/` 以下は isaac から抽出したシードコードのままで、単独では
実行できない。目標と検証項目は [#3](https://github.com/ycpss91255-lab/isaac_ros_io/issues/3)、プラグイン
インターフェースは [#6](https://github.com/ycpss91255-lab/isaac_ros_io/issues/6) を参照。

## 依存関係

- Isaac Sim 6.x
- ROS 2 Humble
- `isaacsim.ros2.bridge` extension

## 出典

[ycpss91255-lab/isaac @ c068e3a](https://github.com/ycpss91255-lab/isaac/tree/c068e3a)
から [issue #309](https://github.com/ycpss91255-lab/isaac/issues/309) に基づいて抽出。
[#4](https://github.com/ycpss91255-lab/isaac_ros_io/issues/4) で `isaac_ros2` から `isaac_ros_io` に改名。

各ファイルの出典対照表は [SOURCE.md](SOURCE.md) を参照してください。

## ライセンス

[Apache-2.0](LICENSE)
