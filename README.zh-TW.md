# isaac_ros2

Isaac Sim ROS 2 bridge -- OmniGraph 感測器發布鏈 (camera, LiDAR, IMU)
及輸入端 topic 訂閱 (cmd_vel)，用於 Isaac 模擬環境。

## 概述

從 [ycpss91255-lab/isaac](https://github.com/ycpss91255-lab/isaac)
([#309](https://github.com/ycpss91255-lab/isaac/issues/309))
抽出的 ROS 2 整合層。

負責建構 OmniGraph action graph，將感測器資料發布至 ROS 2 topic，
並訂閱輸入端指令。

## 目前狀態

Seed code 階段。尚無法獨立執行。依賴 Isaac Sim 容器及 `isaac_devkit` 框架。

## 相依套件

- Isaac Sim 6.x
- ROS 2 Humble
- `isaacsim.ros2.bridge` extension

## 來源

從
[ycpss91255-lab/isaac @ c068e3a](https://github.com/ycpss91255-lab/isaac/tree/c068e3a)
依據 [issue #309](https://github.com/ycpss91255-lab/isaac/issues/309) 抽出。

各檔案來源對照表見 [SOURCE.md](SOURCE.md)。

## 授權

[Apache-2.0](LICENSE)
