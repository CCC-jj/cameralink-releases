# 光栈 CameraLink · Android 内测发布

本仓库用于发布 CameraLink 安装包、更新说明和应用内更新清单。开发源码及签名私钥不存放在这里。

## 下载与安装

前往 [Releases](https://github.com/CCC-jj/cameralink-releases/releases) 下载所需版本的 `CameraLink-版本号.apk`。

- Android 8 及以上。
- 首次使用应用内更新，需要手动安装 0.8.0 或之后包含更新模块的版本。
- 安装后进入「设置 → 检查更新」。默认更新来源为 `CCC-jj/cameralink-releases`。
- 下载完成后，App 校验安装包的长度、SHA-256、包名、版本和签名，再调起 Android 系统安装。
- 首次可能需要允许 CameraLink 安装未知应用；允许后返回更新页继续安装。
- 更新安装前，请完成照片传输并断开相机连接。相机热点通常不能联网，可稍后使用可用网络下载。

## Release 附件

每个正式发布的 Release 包含 APK、`update.json` 和 `SHA256SUMS.txt`。App 读取最新非草稿、非预发布 Release；后续版本必须递增 Android versionCode 并使用兼容签名。

当前为开发签名内测渠道。真机与相机兼容性仍需实测；每个版本的验证范围见对应 Release 说明。更新失败不会要求先卸载旧版本，请保留应用内照片。
