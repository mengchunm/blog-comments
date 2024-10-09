---
title: 刷机资源整合
cover: https://article.biliimg.com/bfs/article/2b6527995a849d783d480907bdbff0e964587936.jpg
---

由于近来刷机方式越来越复杂，刷机所需要的资源也越来越多  

找起来比较麻烦，干脆写个整合
<!-- more --><!-- more -->

## Android 调试桥 (adb)

[//]: # (![img]&#40;https://s2.loli.net/2022/04/16/N9WavxViTQGKuMh.png&#41;)

如果您是 Android 开发者，则应从 Android Studio 的 [SDK 管理器](https://developer.android.google.cn/studio/intro/update?hl=zh-cn#sdk-manager)或通过 [`sdkmanager`](https://developer.android.google.cn/studio/command-line/sdkmanager?hl=zh-cn) 命令行工具获取最新的 SDK Platform-Tools。这样可确保这些工具能够与其他 Android SDK 工具一起保存到正确的位置，并可轻松地进行更新。

但是，如果您只想使用这些命令行工具，请访问以下链接：

- [下载适用于 Windows 的 SDK Platform-Tools](https://dl.google.com/android/repository/platform-tools_r33.0.1-windows.zip?hl=zh-cn)
- [下载适用于 Mac 的 SDK Platform-Tools](https://dl.google.com/android/repository/platform-tools_r33.0.1-darwin.zip?hl=zh-cn)
- [下载适用于 Linux 的 SDK Platform-Tools](https://dl.google.com/android/repository/platform-tools_r33.0.1-linux.zip?hl=zh-cn)

## Magisk

[//]: # (![img]&#40;https://s2.loli.net/2022/04/15/i18qOxctKpVNDrE.png&#41;)

[magisk](https://github.com/topjohnwu/Magisk/releases)下载并安装

#### 获取BOOT.img文件

下载ROM（刷机包）文件

小米:<https://xiaomirom.com>

一加:<https://www.oneplus.com/cn/support/softwareupgrade>

##### 线刷包

通过解压，在解压文件里找

##### 卡刷包

同样解压后,通过[payload dumper](https://github.com/ssut/payload-dumper-go/releases)工具解包

将payload.bin文件解压出来，和payload_dumper.exe,ROM(刷机包)放在一个文件夹下，双击payload_dumper.exe解包

#### 处理BOOT.img文件

1. 打开magisk软件，选择magisk旁的安装
2. 选择并修补一个文件
3. 选择BOOT.img
4. 将magisk生成的magisk_patched.img文件上传至电脑
5. 在adb文件夹内，点击上方文件路径输入并打开cmd运行

{% copy fastboot flash boot D:\magisk_patched.img（该文件所在地址）%}

恭喜你已经成功给你的手机输入了magisk框架

但刷入了错误或不适配的文件可能会导致你的手机无法正常开机/成砖

所以我建议你刷入第三方rec并安装mm管理器(Magisk Manager for Recovery Mode)模块

### 第三方Rec

[//]: # (![img]&#40;https://s2.loli.net/2022/04/16/gEM6NXAjbiTDSH5.png&#41;)
  进入Rec

|      | 电源键 | 音量- | 音量+ |  其他   |
| :--: | :----: | :---: | :---: | :-----: |
| 小米 |   ●    |       |   ●   |         |
| oppo |   ●    |   ●   |       |         |
| 一加 |   ●    |   ●   |       |         |
| 索尼 |   ●    |       |   ●   |         |
| 三星 |   ●    |       |   ●   | bixby键 |

  [TWRP(Team Win Recovery Project)](https://twrp.me/Devices/)

{% copy fastboot flash recovery D:\TWRP.img（该文件所在地址） %}

### [mm管理器](https://www.droidmirror.com/download/mm-201904040-zip)

在mm管理器中下载并刷入

使用方法：在REC主界面选择 高级——>终端命令——>在终端中输入 sh /sdcard/mm或/data/media/mm 即可进入

建议使用mm管理器中文版<https://www.lanzoui.com/b00ncqwod>密码：yezi

### 其他工具

[搞机助手](https://lsdy.top/gjzs)

[残芯定制rec](http://119.3.10.7)(要付费，但功能全一点点， 安卓11以下rec自动解锁，安卓十二以上无锁屏密码自动解锁)

### 成砖修复

小米可以试试[miflash](https://miuiver.com/miflash/)(配合<https://xiaomirom.com>)

可以试试保留数据刷机，不行再全部删除刷机

