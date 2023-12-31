---
title: XTC 任意版本 root 方法
author: xrz
---

# XTC 任意版本 root 方法

## 刷前提示

**刷机有风险，玩机需谨慎。如果变砖作者概不负责。**

## 新版

刷入修改后的 aboot，再刷 sboot 就行了。

## 旧版

**请先有 root 和安装软件的必要和前提再来。  
本教程适用于有救砖能力的想在小天才新版本 root 的玩家，小白请绕道。**  
[XTC 文件库](/blog/XTC-Files)(失效文件链接请到这里面找)  
还找不到？有一个好东西叫[百度](https://www.baidu.com)

## 条件

聪明的脑子、灵活的双手、会用 QFIL[下载](https://www.mediafire.com/file/220h5xaxi1gd55m/QPST_2.7.496.zip/file) [教程](https://www.baidu.com/s?ie=utf-8&f=8&rsv_bp=1&tn=baidu&wd=QFIL%E6%95%99%E7%A8%8B)、刷过 sboot[下载](https://xrzyun-generic.pkg.coding.net/xrz-video/xtc/XTC-SBoot-RV1.5.zip)。

## 提取固件（已有固件可忽略）

1. 移除 root，升级至最新固件
2. 连接电脑，打开 QFIL，9008 模式提取 system 分区[提取方法](https://www.baidu.com/s?ie=utf-8&f=8&rsv_bp=1&tn=baidu&wd=QFIL%E6%8F%90%E5%8F%96%E5%88%86%E5%8C%BA)和 userdata 分区(刷入后可能导致绑定号出错，部分小天才功能不能使用)。 Tips：QFIL 默认把提取的文件存至`C:\Users\l\AppData\Roaming\Qualcomm\QFIL\`下的一个目录。

## 正式开工

3. 进 9008，回到**可以刷 sboot 的版本**，刷入 sboot(boot 分区)和 recovery.img(recovery 分区)[下载][不会刷看教程]（和备份的 userdata.bin）。
4. _(可选)回到系统，输入 `adb reboot recovery` 确认能进入 rec_
5. 9008 刷之前提取的 system.bin。
6. 开机查看：新系统和 magisk 都有了。

## 其它

[可能出现的意外及解决方法](./xtcuproot-Q&A)  
Tips：作者 z5q 测试成功，其他机型请自测。（图有空再补）

# LICENSE 版权声明

本博客所有文章除特别声明外，均采用[BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/)许可协议。转载请注明出处！
