# VidRestore - AI 智能视频增强工具

**macOS 专用的本地 AI 视频画质提升软件**

VidRestore 是一款完全离线运行的 macOS 应用，基于先进 AI 模型自动检测并高质量修复视频中的低清晰度、模糊或损坏区域。支持批量处理，并针对 Apple Silicon 芯片进行了深度优化。

## ✨ 主要特性

- 简洁现代的 macOS 原生风格界面
- 支持 28 种常见视频格式（mp4、mkv、mov、ts、m2ts、wmv、flv、webm 等）
- **智能动态分段 + 多进程并行处理**，根据设备内存和视频分辨率自动调整分段长度
- 自动修复视频元数据、时长、帧率等问题
- 输出高质量 HEVC（hvc1）编码视频，体积更小、兼容性更好
- 实时日志、进度追踪、待处理/已完成列表管理
- **完全离线运行**，无需联网，数据不离开本地设备
- 针对不同硬件配置（从 16GB 到 128GB+ 内存）进行内存优化

## 📥 下载与安装

**下载最新版本**

[⬇️ 下载 VidRestore（最新版）](https://github.com/Poeticphysicist/vidrestore/releases/latest/download/VidRestore.dmg)

**安装步骤**：
1. 下载 `VidRestore.dmg`
2. 双击打开，将 `VidRestore.app` 拖拽到「应用程序」文件夹
3. 在 Launchpad 或 `/Applications` 中打开应用
4. **首次打开**可能需要右键点击 →「打开」（绕过 macOS 安全提示）

## 🚀 使用方法

1. 打开 VidRestore
2. 点击「📁 选择视频文件」添加需要处理的视频（支持多选）
3. 点击「🚀 开始处理」
4. 处理完成后，视频将自动保存为 `原文件名-U.mkv`，并出现在右侧「已完成」列表中

**支持功能**：
- 批量处理多个视频
- 点击已完成列表中的路径可在 Finder 中快速定位文件
- 处理过程中可随时停止任务

## 系统要求

- macOS 12.0 或更高版本
- Apple Silicon 芯片（M1/M2/M3/M4 系列）
- 推荐内存：32GB 及以上（16GB 可正常运行，处理时会自动采用更保守策略）

## 技术特点

- 采用 Supervisor 架构管理后台进程，提升稳定性和资源回收能力
- 根据设备内存和视频分辨率动态调整分段时长与处理参数
- 完善的错误处理机制，失败任务不会影响整体流程
- 完全本地 AI 处理，无任何网络请求

## 致谢

感谢以下开源项目为本软件提供的技术支持：

- Real-ESRGAN
- FFmpeg
- PyInstaller
- CustomTkinter

## 联系我们

如有问题或建议，欢迎邮件联系：**support@vidrestore.app**
