# JNUSSR - ROBOCON 2026 🤖

欢迎来到暨南大学 SSR 战队 2026 赛季 ROBOCON 官方工程仓库。
本仓库用于集中管理机器人的下位机控制代码、上位机视觉算法、硬件电路设计以及相关技术文档。

## 📂 目录结构 (Directory Structure)

本仓库采用软硬件协同的模块化管理，主要包含以下子系统：

* **`Docs/` - 项目文档与规范**
	* 存放协议定义。
	* 存放算法推导与规范文档。
	* 团队协作指南与会议记录。

* **`Firmware/` - 下位机控制工程 (STM32)**
  

* **`Hardware/` - 硬件与电路设计**
	-  存放主控板、电源管理及各传感器接口的电路原理图（Schematics）与 PCB Layout 工程。
 

* **`Vision/` - 上位机视觉**
	- 运行于上位机的视觉识别算法

## 🤝 协作与提交规范 (Contribution Guidelines)

为了保证代码库的整洁与稳定，请团队成员严格遵守以下规范：

1. **分支管理 (Branching)：**
   * `main` 分支仅用于存放经过实车测试、稳定可靠的版本。**严禁直接 Push 到 main 分支。**
   * 日常开发请在各自的功能分支上进行，例如：`feature/chassis-ctrl` 或 `feature/vision-yolo`。
   * 开发完成后，提交 Pull Request (PR) 合并到主开发分支或 `main`。

2. **忽略文件 (.gitignore)：**
   * 提交代码前，请确保本地配置了正确的 `.gitignore`。
   * **绝对不要**提交编译产生的中间文件（如 `.o`, `.d`, `.hex`, `.bin`）以及 IDE 的本地用户配置（如 `.uvoptx` 的用户数据，或 EDA 软件的自动备份日志）。
