# 悬浮便签更新源

这个公开仓库只存放悬浮便签的 Windows 自动更新与 macOS 半自动更新资源，不包含源码或本地用户数据。

每个正式 Release 包含：

- Windows：`latest.yml`、Setup 安装包和对应 blockmap
- macOS：`latest-mac.yml`、DMG 安装镜像和对应 blockmap

应用通过 `https://github.com/LawrenceChiu95/floating-sticky-notes-updates/releases/latest/download` 读取更新。Windows 可以在应用内完成下载、退出和安装；macOS 会下载并校验 DMG、打开安装镜像并退出，用户仍需手动拖到 Applications 并确认替换。

发布规则：先创建 Draft Release 并上传安装包，完成 Windows 与 Apple Silicon Mac 基础真机验证后再发布，并明确标记为 latest。`latest.yml` 和 `latest-mac.yml` 最后上传；这两个元数据文件分别是 Windows 和 macOS 的更新开关。
