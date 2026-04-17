# VidRestore - AI 智能视频增强工具

**macOS 专用的本地 AI 视频画质提升软件**

VidRestore 是一款完全离线运行的 macOS 应用，利用先进的 AI 模型自动检测并高质量修复视频中的低清晰度、马赛克或模糊区域，支持批量处理和 Apple Silicon 硬件加速。

## ✨ 主要特性

- 简洁现代的 macOS 原生风格 GUI 界面
- 支持 28 种常见视频格式（mp4、mkv、mov、ts、m2ts、wmv、flv、webm 等）
- 自动视频分段 + 多进程并行处理，充分发挥 M 系列芯片性能
- 智能修复元数据、时长、帧率等问题
- 输出高质量 HEVC（hvc1）视频，体积更小、兼容性更好
- 实时日志、进度条、待处理/已完成列表
- **完全离线运行**，无需联网、无需额外依赖

## 📥 下载与安装

**最新版本：v1.0.0**

[⬇️ 下载 VidRestore v1.0.0](https://github.com/Poeticphysicist/vidrestore/releases/latest/download/VidRestore.dmg)

**安装步骤**：
1. 下载 `VidRestore.dmg`
2. 双击打开 dmg 文件，将 `VidRestore.app` 拖拽到「应用程序」文件夹
3. 在 Launchpad 或 `/Applications` 中打开 VidRestore

> **注意**：首次打开时可能需要右键点击 →「打开」（macOS 安全策略）

## 🚀 使用方法

1. 打开 VidRestore
2. 点击「📁 选择视频文件」，添加需要处理的视频
3. 点击「🚀 开始处理」
4. 处理完成后，视频会自动保存为 `原文件名-U.mkv`，并出现在右侧「已完成」列表

**批量处理**：可一次性选择多个视频  
**快速定位**：点击已完成列表中的路径可在 Finder 中高亮显示文件

## 系统要求

- macOS 12.0 或更高版本
- Apple Silicon 芯片（M1/M2/M3/M4）
- 推荐内存 32GB 以上（16GB 可正常运行）

## 技术栈

- **界面**：CustomTkinter（现代 macOS 风格）
- **核心**：先进 AI 视频修复引擎 + Real-ESRGAN 模型 + FFmpeg + mkvmerge
- **打包**：PyInstaller（单文件 .app + .dmg）

## 致谢

感谢以下开源项目为本软件提供的强大支持：
- Real-ESRGAN（BSD-3-Clause）
- FFmpeg
- PyInstaller
- CustomTkinter

## 联系我们

有任何问题或建议，欢迎邮件联系：support@vidrestore.app
