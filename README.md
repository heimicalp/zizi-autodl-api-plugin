# 黑米CaC AutoDL-API插件

字字动画的视频生成插件，通过 CodeWithGPU/AutoDL 托管工作流 API 生成视频。

## 下载与更新

在 [Releases](https://github.com/heimicalp/zizi-autodl-api-plugin/releases) 下载最新的 `autodl-shot-bridge-*.zip`。退出字字动画，解压安装包后，在 PowerShell 中运行：

固定的更新元数据位于 [`latest.json`](latest.json)，包含版本号、下载地址和 ZIP 的 SHA256；后续版本发布时会同步更新。

```powershell
.\Install.ps1 -AppRoot '你的字字动画安装目录' -Upgrade
```

首次安装时去掉 `-Upgrade`。安装器会检查文件摘要，并在升级前备份旧代码；用户配置、令牌和任务记录不包含在发行包中。安装后重启字字动画。

当前版本属于发布候选版。真实宿主付费生成、画质和第二台机器验收尚未完成，请参见安装包中的 `RELEASE_CHECKLIST.md`。
