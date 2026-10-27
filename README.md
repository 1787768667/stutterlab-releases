# 卡顿诊断（StutterLab）安装包

找出 Windows 电脑卡顿、掉帧、死机的真正原因。这个仓库只用来发布安装包和自动更新，不含源代码。

## 下载

到 [Releases](../../releases/latest) 下载最新的 `StutterLab-<版本>-portable.zip`，解压后双击 `StutterLab.exe`。
适用于 Windows 10 / 11（64 位），不需要安装 .NET。详细说明见压缩包里的"使用说明.txt"。

## 自动更新

0.4.0 及以后的版本会自动检查这里的新版本，发现后询问是否更新。
`update.json` 带有发布者的数字签名，安装包的 SHA-256 也写在里面；签名或指纹对不上时软件不会安装。
检查更新时只下载 `update.json`，不发送任何电脑或个人信息，可以在"设置 → 更新"里关闭。

## 第三方组件

安装包里包含 Intel PresentMon（MIT）、PawnIO 安装程序（GPL-2.0，未修改，源码 https://github.com/namazso/PawnIO）、
LibreHardwareMonitorLib（MPL-2.0）、.NET 运行时（MIT）和 PCI ID 数据库摘录（BSD-3）。
许可全文见压缩包里的"第三方组件许可.txt"和 `third_party` 文件夹。

---

# StutterLab releases

Finds the real causes of stutter, frame drops and freezes on Windows PCs. This repository only hosts release packages and auto-update data; it contains no source code.

Download the latest `StutterLab-<version>-portable.zip` from [Releases](../../releases/latest), extract it and run `StutterLab.exe` (Windows 10/11, 64-bit).
Version 0.4.0 and later check here for updates. `update.json` is signed by the publisher and includes the package's SHA-256; the app refuses to install anything that doesn't match.
