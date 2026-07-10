# 悬浮便签更新源

这个公开仓库只存放悬浮便签的 Windows 自动更新资源，不包含源码或本地用户数据。

每个正式 Release 包含：

- `latest.yml`
- Windows Setup 安装包
- 对应 blockmap

应用通过 `https://github.com/LawrenceChiu95/floating-sticky-notes-updates/releases/latest/download` 读取更新。

发布规则：先创建 draft Release 并上传全部资源，完成 Windows 真机验证后再发布。把 draft 切换为 published 是唯一上线开关。