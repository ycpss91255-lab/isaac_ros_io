# isaac_ros2

Isaac Sim ROS 2 bridge -- OmniGraph センサーパブリッシュチェーン (camera, LiDAR, IMU)
およびインバウンド topic サブスクリプション (cmd_vel)。Isaac シミュレーション環境向け。

## 概要

[ycpss91255-lab/isaac](https://github.com/ycpss91255-lab/isaac)
([#309](https://github.com/ycpss91255-lab/isaac/issues/309))
から抽出した ROS 2 統合レイヤー。

OmniGraph アクショングラフを構築し、センサーデータを ROS 2 topic へパブリッシュし、
インバウンドコマンドをサブスクライブします。

## 現在の状態

Seed code 段階。単独では実行不可。Isaac Sim コンテナおよび `isaac_devkit`
フレームワークに依存しています。

## 依存関係

- Isaac Sim 6.x
- ROS 2 Humble
- `isaacsim.ros2.bridge` extension

## 出典

[ycpss91255-lab/isaac @ c068e3a](https://github.com/ycpss91255-lab/isaac/tree/c068e3a)
から [issue #309](https://github.com/ycpss91255-lab/isaac/issues/309)
に基づいて抽出。

各ファイルの出典対照表は [SOURCE.md](SOURCE.md) を参照してください。

## ライセンス

[Apache-2.0](LICENSE)
