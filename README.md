# RushPilot 安装包发布处

这里只放 RushPilot 的安装包和版本说明，**不包含源码**。

## 自动更新

RushPilot 1.7.0 起会在启动时检查这里的最新版本。下载的安装包会核对签名、文件大小和指纹，全部通过才会安装；原片、导出文件和任务记录都不会被改动。

## 手动安装

1. 在右侧 **Releases** 里下载最新的 `RushPilot-x.y.z.zip`。
2. 解压后得到 `RushPilot AI Selects Preview.app`，改名为 `RushPilot.app`，放到“应用程序”文件夹（或你常用的位置）。
3. 第一次打开如果提示“无法验证开发者”，在访达里右键点应用，选“打开”。

需要：M 系列芯片 Mac、macOS 26 以上、Homebrew 安装的 ffmpeg。

## 核对安装包

每个版本附带 `latest.json`（版本信息）和 `latest.json.sig`（签名）。`latest.json` 里的 `sha256` 可以用下面的命令核对：

```bash
shasum -a 256 RushPilot-x.y.z.zip
```
