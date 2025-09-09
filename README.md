<!-- markdownlint-disable MD033 MD041 -->
<p align="center">
  <img alt="LOGO" src="https://cdn.jsdelivr.net/gh/MaaAssistantArknights/design@main/logo/maa-logo_512x512.png" width="256" height="256" />
</p>

<div align="center">

# 刀剑乱舞自动化助手

**基于 MaaFramework 的刀剑乱舞游戏自动化工具**
*献给热爱刀剑乱舞的审神者们，以及那些在开发路上给予支持的重要之人*
</div>

本项目基于 [MaaFramework](https://github.com/MaaXYZ/MaaFramework) 开发，专为刀剑乱舞游戏提供自动化功能，帮助玩家减少重复性操作。

> **MaaFramework** 是基于图像识别技术、运用 [MAA](https://github.com/MaaAssistantArknights/MaaAssistantArknights) 开发经验去芜存菁、完全重写的新一代自动化黑盒测试框架。

## ✨ 功能特色

### 🌸 维新刷花（函馆关卡）

- 自动选择维新的记忆-函馆关卡
- 使用部队一进行战斗
- 自动检测疲劳度上限（100/100）
- 支持循环刷取直至体力耗尽

### ⚔️ 一键演练

- 自动寻找并发起演练挑战
- 使用部队二进行演练
- 循环进行演练直至无可挑战对象

### 📈 5-4练级（阿津贺志山之战）

- 自动选择武家的记忆-阿津贺志山关卡
- 使用部队三进行练级
- 智能避免进入王点
- 自动检测重伤状态并停止
- 支持自动返回本丸重新开始

### 💪 战力扩充关卡1
- 自动选择战力扩充计划第一关卡
- 使用部队四进行战斗
- 智能切换到出阵菜单
- 自动检测重伤状态并停止战斗
- 支持循环刷取提升战力
  
## 🚀 快速开始

### 环境要求

- Android 设备或模拟器
- Python 3.9+
- ADB 调试工具

### 安装步骤

1. **克隆项目**

    ```bash
    git clone https://github.com/Severus-Yang0/MaaToukenRanbu.git
    ```

2. **下载 MaaFramework**

    从 [MaaFramework Releases](https://github.com/MaaXYZ/MaaFramework/releases) 下载最新版本，解压到 `deps` 文件夹中。

3. **配置 OCR 模型**

    ```bash
    git submodule update --init --recursive
    python ./configure.py
    ```

    如果子模块下载失败，可从 [Mirror酱](https://mirrorchyan.com/zh/projects?rid=MaaCommonAssets&source=ghtempl-readme) 手动下载并解压到 `assets/MaaCommonAssets` 文件夹。

4. **安装依赖**

    ```bash
    python -m pip install MaaFW --upgrade
    ```

5. **连接设备**

    确保 Android 设备已开启 USB 调试，并通过 ADB 连接到电脑。

6. **在debugger中运行**

    ```bash
    python -m MaaDebugger
    ```

## ⚙️ 配置说明

### 分辨率要求

本工具基于特定分辨率的坐标配置，请确保您的设备分辨率为标准分辨率。如需适配其他分辨率，可能需要调整 `assets/resource/pipeline` 中的 ROI 坐标。

### 部队配置

- **部队一**：用于刷花任务，建议配置稳定的队伍
- **部队二**：用于演练任务
- **部队三**：用于练级任务，建议配置需要练级的角色
- **部队四**：用于战力扩充任务（需要已经通关至少一次），建议配置战力合适的队伍

## ⚠️ 注意事项

### 使用风险

- 本工具仅供学习交流使用
- 使用自动化工具存在一定风险，请谨慎使用
- 建议在小号上测试后再在主号使用
- 使用前请仔细阅读游戏服务条款

### 免责声明

- 使用本工具产生的任何后果由用户自行承担
- 开发者不对因使用本工具导致的账号问题负责
- 请遵守游戏官方规定，理性游戏

## 🔧 常见问题

### 识别失败怎么办？

1. 确认游戏界面清晰，无遮挡
2. 检查设备分辨率是否匹配
3. 确认 OCR 模型已正确下载
4. 查看 `debug/maa.log` 日志文件排查问题

### 点击位置不准确

可能是分辨率不匹配导致的坐标偏移，需要根据您的设备调整配置文件中的坐标。

### 程序无响应

1. 检查 ADB 连接是否正常
2. 确认设备未锁屏
3. 重启程序或重新连接设备

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request 来完善本项目！

### 反馈问题

- 游戏功能相关问题请在本项目提 Issue
- MaaFramework 框架问题请前往 [MaaFramework/issues](https://github.com/MaaXYZ/MaaFramework/issues)
- 使用疑问可在 [MaaFramework 讨论区](https://github.com/MaaXYZ/MaaFramework/discussions) 交流

## 📄 开源协议

本项目采用与 MaaFramework 相同的开源协议。

## 🙏 鸣谢

本项目由 **[MaaFramework](https://github.com/MaaXYZ/MaaFramework)** 强力驱动！

感谢 MaaFramework 团队提供的优秀自动化框架。

---

**⭐ 如果这个项目对您有帮助，请考虑给个 Star！**
