<!-- markdownlint-disable MD033 MD041 -->
<p align="center">
  <img alt="LOGO" src="https://cdn.jsdelivr.net/gh/MaaAssistantArknights/design@main/logo/maa-logo_512x512.png" width="256" height="256" />
</p>

<div align="center">

# Touken Ranbu Automation Assistant

**An automated tool for Touken Ranbu game based on MaaFramework**

*Dear Yasumoto-san, thank you for bringing light to my journey*

</div>

This project is developed based on [MaaFramework](https://github.com/MaaXYZ/MaaFramework), specifically designed to provide automation features for the Touken Ranbu game, helping players reduce repetitive operations.

> **MaaFramework** is a next-generation automated black-box testing framework based on image recognition technology, utilizing the development experience of [MAA](https://github.com/MaaAssistantArknights/MaaAssistantArknights) with a complete rewrite for optimal performance.

## ✨ Features

### 🌸 1-1 Recovery

- Automatically selects the Memory of Restoration - Hakodate stage
- Uses Formation 1 for battle
- Automatically detects fatigue limit (100/100)
- Supports continuous farming until stamina depletion

### ⚔️ Practice Battle

- Automatically finds and initiates practice challenges
- Uses Formation 2 for practice battles
- Continuous practice until no more opponents available

### 📈 5-4 Level Up

- Automatically selects the Memory of Warriors - Atsugashiyama stage
- Uses Formation 3 for level grinding
- Intelligently avoids entering boss nodes
- Automatically detects severe injury status and stops
- Supports automatic return to citadel and restart

### 💪 Enhancement Activity Stage 1
- Automatically selects the first stage of Power Enhancement Plan
- Uses Formation 4 for battle
- Intelligently switches to sortie menu
- Automatically detects severe injury status and stops battle
- Supports continuous farming to increase combat power

## 🚀 Quick Start

### Requirements

- Android device or emulator
- Python 3.9+
- ADB debugging tools

### Installation Steps

1. **Clone the Project**

    ```bash
    git clone https://github.com/Severus-Yang0/MaaToukenRanbu.git
    ```

2. **Download MaaFramework**

    Download the latest version from [MaaFramework Releases](https://github.com/MaaXYZ/MaaFramework/releases) and extract to the `deps` folder.

3. **Configure OCR Model**

    ```bash
    git submodule update --init --recursive
    python ./configure.py
    ```

    If submodule download fails, you can manually download from [Mirror酱](https://mirrorchyan.com/zh/projects?rid=MaaCommonAssets&source=ghtempl-readme) and extract to the `assets/MaaCommonAssets` folder.

4. **Install Dependencies**

    ```bash
    python -m pip install MaaFW --upgrade
    ```

5. **Connect Device**

    Ensure your Android device has USB debugging enabled and is connected to your computer via ADB.

6. **Run in Debugger**

    ```bash
    python -m MaaDebugger
    ```

## ⚙️ Configuration

### Resolution Requirements

This tool is based on specific resolution coordinate configurations. Please ensure your device resolution matches the standard resolution. For other resolutions, you may need to adjust the ROI coordinates in `assets/resource/pipeline`.

### Formation Setup

- **Formation 1**: For flower farming tasks, recommend stable team composition
- **Formation 2**: For practice battle tasks
- **Formation 3**: For level grinding tasks, recommend characters that need leveling
- **Formation 4**: For power enhancement tasks (requires at least one clear), recommend team with appropriate combat power

## ⚠️ Important Notes

### Usage Risks

- This tool is for educational and communication purposes only
- Using automation tools carries certain risks, please use with caution
- Recommend testing on secondary accounts before using on main accounts
- Please read the game's terms of service carefully before use

### Disclaimer

- Users bear full responsibility for any consequences resulting from using this tool
- Developers are not responsible for account issues caused by using this tool
- Please comply with official game regulations and play responsibly

## 🔧 Troubleshooting

### Recognition Failures

1. Ensure the game interface is clear and unobstructed
2. Check if device resolution matches requirements
3. Confirm OCR model has been downloaded correctly
4. Review the `debug/maa.log` file for troubleshooting

### Inaccurate Click Positions

This may be caused by coordinate offset due to resolution mismatch. You need to adjust the coordinates in the configuration files according to your device.

### Program Unresponsive

1. Check if ADB connection is normal
2. Ensure device is not locked
3. Restart the program or reconnect the device

## 🤝 Contributing

We welcome Issues and Pull Requests to improve this project!

### Reporting Issues

- For game feature-related issues, please submit Issues in this project
- For MaaFramework framework issues, please visit [MaaFramework/issues](https://github.com/MaaXYZ/MaaFramework/issues)
- For usage questions, you can discuss in [MaaFramework Discussions](https://github.com/MaaXYZ/MaaFramework/discussions)

## 📄 License

This project adopts the same open source license as MaaFramework.

## 🙏 Acknowledgments

This project is powered by **[MaaFramework](https://github.com/MaaXYZ/MaaFramework)**!

Thanks to the MaaFramework team for providing an excellent automation framework.

---

**⭐ If this project helps you, please consider giving it a Star!**