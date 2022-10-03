---
title: LyricEase：简洁的第三方网易云音乐客户端【补档】
date: 2022/10/03 13:01:00
description: LyricEase，简洁的第三方网易云音乐客户端
---

LyricEase 是一款第三方网易云音乐 UWP 客户端，曾在 Github 上开源（已下架）、Microsoft Store 上供用户免费使用（已下架）。

![软件截图][1]

我们同时提供了[视频](https://www.bilibili.com/video/BV19a4y1f7Mq)版本。

## 补档原因

由于“非法侵权网易云音乐有版权音乐”与“非法攫取网易云音乐用户与流量”，被网易公司警告，在全平台下架。2022年8月15日，LyricEase 开发者将软件分发至微软另一平台（APP Center），但无法确定此次平台分发能够持续多久，故本站下载保存了程序安装包并上传补档，以备不时之需。

## 软件明细

| 属性     | 值                                                       |
| -------- | -------------------------------------------------------- |
| 适用平台 | Windows（需要支持 UWP，大约为 Windows 10 或 Windows 11） |
| 语言     | 多语言（含简体中文）                                     |
| 发行格式 | Msix Bundle、证书与安装脚本                              |

## 安装说明

1. 由于未在微软商店上架，需要开启开发者模式以安装应用。
   Win11：设置（APP）-隐私和安全性-开发者选项-开发人员模式（设置为开启）
   Win10：设置（APP）-更新和安全-开发者选项-使用开发人员功能（设置为“开发人员模式”）
2. 下载压缩包并 **完全解压**，**不要在压缩软件内直接打开！**
3. 双击运行 "install.ps1"，期间系统的安全提示全部选择允许 / 同意。

## 下载地址

- 官方（APP Center）【最新版本】[下载地址](https://install.appcenter.ms/users/brandonw3612/apps/lyricease/distribution_groups/public)，进入后稍等加载，然后点击蓝色按钮 **DOWNLOAD** 下载
- 好物荟萃镜像【v0.11.125 (20220815)】[下载地址](https://imymuyang-my.sharepoint.com/:u:/g/personal/i_xn--ouw410g_ml/EWGk-TfVEcRGniW8i9WlSpABwtmeBPtSKzxtrhQtQhVdRg?e=PPsYid)，密码为 **xn--5us.gq**，输入密码后可在线查看压缩包，电脑版左上角第三个按钮有中文“下载”字样

MD5：a2737e03df62097d6dc60d48a157feb4

## 安装问题解答

### x86 和 arm 平台没法安装

目前由于维护困难，开发者仅仅提供了 x64 与 arm64 的安装包，不提供 x86 和 arm 的支持。

### 选择用 Powershell 打开，出现一下蓝窗口就闪退消失

先在开始菜单用管理员身份打开 Powershell，然后再输入 install.ps1 的 **全地址**。

### 提示“无法加载文件 xxx.ps1，因为在此系统上禁止运行脚本。”

先在开始菜单用管理员身份打开 Powershell，然后输入 `set-executionpolicy remotesigned`，然后输入 `A`，按下 Enter 键。

### 软件使用时出现弹窗错误，内容为“An error occurred while sending the request.”

关闭电脑中的全局代理，或者查看[这篇文章][2]。


  [1]: https://i.imgtg.com/2022/10/03/mfTND.png
  [2]: https://www.xn--5us.gq/archives/loopback