---
title: Loopback 小工具：让 UWP 应用也可以走代理
date: 2022/10/03 13:01:00
description: 为 UWP 应用启用代理功能
---
适用于 Windows 8/8.1/10/11 各系列用户，Linux/MacOS/安卓/苹果/Windows 8以下等系统用户无需参考。

UWP APP 运行在沙箱里面，而这个沙箱限制了本机代理和 UWP APP 的往来，而有些时候因为网络太卡需要代理加速，这时 APP 轻则不走代理（如 MC 基岩版），重则直接报错、卡死、闪退（如 LyricEase）。因而，本站整合了全网各种方法与工具，一站式处理这个问题。

## AppContainer Loopback Exemption Utility（适用于有针对性用户）

这是网络抓包工具 Fiddler 出品的一款简洁小工具。软件傻瓜操作，只需要先在需要解除限制的软件前打勾，然后点击上面的 Save Changes，就可以解除限制了。

![AppContainer Loopback Exemption Utility 截图][1]

{% grid  下载地址 %}
官方地址：[亚马逊 S3](https://telerik-fiddler.s3.amazonaws.com/fiddler/addons/enableloopbackutility.exe)
MD5：f292bb20622d374f5e0832aa1d3813c0
{% endgrid %}

## UWPLoopback（国产，适合电脑小白）

这是作者对于软件的[介绍][2]，直接一站式解除所有限制，无需多次操作。

{% grid  下载地址 %}
官方地址：[Github](https://github.com/Dispnt/UWPLoopback/releases/download/1.0.0/Loopback.exe)
备用镜像：[FastGit](https://hub.fastgit.org/Dispnt/UWPLoopback/releases/download/1.0.0/Loopback.exe)
{% endgrid %}


## 注册表 + 命令行（适合不想安装软件的用户，难度相对较大）

打开注册表，进入 `计算机\HKEY_CURRENT_USER\Software\Classes\Local Settings\Software\Microsoft\Windows\CurrentVersion\AppContainer\Mappings`。
在 Mappings 中找到需要的软件（右边的 DisplayName 就是需要的软件名）后，复制文件夹的名字（如`S-1-15-2-xxx`），关闭注册表。

管理员模式打开命令行，输入`CheckNetIsolation.exe loopbackexempt -a -p=那个文件夹的名字`。

{% note color:yellow 即使显示了完成，也不一定代表真的OK，因为即使输错文件夹名字系统也不会报错！ %}



  [1]: https://s1.328888.xyz/2022/08/22/bhGyR.png
  [2]: https://www.dispnt.com/index.php/archives/23/