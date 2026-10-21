# OOMWOO ROS 2 Simulation

## 📌 專案介紹

本專案使用 OOMWOO 官方提供的 ROS 2 模擬環境，
透過 Docker 建立開發環境，並使用 Gazebo 與 RViz
進行機器人模擬、SLAM 建圖及 Nav2 自動導航測試。

目前主要使用官方提供的 ROS 2 套件與 Launch 檔案，
尚未另外開發自訂 ROS 2 套件。

## 🛠️ 開發環境

| 項目 | 使用環境 |
|---|---|
| 作業系統 | Windows 11 |
| 容器平台 | Docker Desktop |
| Docker Image | `makerspet/oomwoo:jazzy-dev` |
| ROS 版本 | ROS 2 Jazzy |
| 模擬器 | Gazebo |
| 視覺化工具 | RViz |
| 建圖功能 | SLAM |
| 導航功能 | Nav2 |
## 📡 主要 ROS 2 Topic

| Topic | 功能 |
|---|---|
| `/cmd_vel` | 機器人速度控制 |
| `/odom` | 里程計資訊 |
| `/scan` | LiDAR 雷射掃描資料 |
| `/camera/image` | 攝影機影像 |
| `/imu` | 慣性測量資料 |
| `/map` | SLAM 建立的地圖 |
| `/tf` | 座標轉換資訊 |

## 📂 專案架構

本 Repository 主要包含 OOMWOO 官方 ROS 2
模擬端相關原始碼與設定檔。

主要套件包括：

- `oomwoo_gazebo`：Gazebo 模擬場景與啟動設定
- `oomwoo_bringup`：機器人系統啟動、SLAM 與導航設定
- `oomwoo_one`：OOMWOO One 機器人相關套件
- `kaiaai_teleop`：機器人遙控相關功能

## 🔗 官方專案來源

本專案基於 OOMWOO 官方開源專案。

官方 GitHub：

https://github.com/makerspet/oomwoo-install

本 Repository 主要用於整理模擬端原始碼、
記錄開發進度，以及方便團隊成員了解系統架構。

原始程式碼之著作權與授權條款以原作者公告為準。
