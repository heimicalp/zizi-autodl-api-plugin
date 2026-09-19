# 黑米CaC AutoDL-API插件

字字动画的视频生成插件，通过 CodeWithGPU/AutoDL 托管工作流 API 生成视频。

## 下载与更新

在 [Releases](https://github.com/heimicalp/zizi-autodl-api-plugin/releases) 下载最新的 `autodl-shot-bridge-*.zip`。

固定的更新元数据位于 [`latest.json`](latest.json)，包含版本号、下载地址和 ZIP 的 SHA256；后续版本发布时会同步更新。

RC22 起，在插件内点击“检查更新”与“下载并安装”；插件会在运行中校验并安装，确认“已安装”后自行退出、重开字字动画即可。生成任务运行期间会拒绝安装。RC20/RC21 的旧后台安装机制可能在软件退出时一起结束，导致只下载却没安装；仍停留在这些版本的用户需要用以下命令过渡升级一次。安装前先结束生成任务，并关闭字字动画：

```powershell
.\Install.ps1 -AppRoot '你的字字动画安装目录' -Upgrade
```

首次安装时去掉 `-Upgrade`。安装器会检查文件摘要，并在升级前备份旧代码；用户配置、令牌和任务记录不包含在发行包中。安装后重启字字动画。

当前版本属于发布候选版。真实宿主付费生成、画质和第二台机器验收尚未完成，请参见安装包中的 `RELEASE_CHECKLIST.md`。
