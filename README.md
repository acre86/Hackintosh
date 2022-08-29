# 国光的黑苹果安装教程：手把手教你配置 OpenCore

##  且行且珍惜

写这篇文章的时间是 2021 年 09 月 15 日，今天的苹果发布会暂时还没有下一代 Mac 的消息，如果下一代 Mac 不配备 intel CPU 的话，那么黑苹果这个技术会随着时间的流逝逐渐成功历史，为了证明自己来过，所以写了这个系列的黑苹果从 0 开始的教程。

实际上 [OpenCore 官方文档](https://dortania.github.io/OpenCore-Install-Guide/)写的已经很不错了，本教程的大部分内容也会搬运自 OpenCore 官方文档。

本 Gitbook 系列的原版文件开源项目地址为：https://github.com/sqlsec/Hackintosh

由于精力有限，本教程不维护了，如果还有人愿意维护这个教程可以 fork 上面的这个项目，Gitbook 搭建的，跑起来不难的。



## 配套视频教程

本系列教程也在 B 站开了系列，感兴趣的网友可以自行去观看：

![](https://image.3001.net/images/20220202/16438093107511.png) 

 视频教程链接传送门：https://www.bilibili.com/video/BV1yq4y1o7cT

## 配套的 QQ 群

建群的初衷不是请一帮伸手党大哥的，还是希望可以营造一个黑苹果技术讨论的地方，提问前自己先谷歌或者百度一下，别人也没有义务去帮你，虚心请教还是大家或多或少都会帮助的。

- 国光的黑苹果正经交流：708385833 （已满）

目前在我的督促下，目前群里绝大多数网友都可以自己配置 EFI 安装黑苹果了，所以别人可以的话，为什么你不可以呢？要相信自己。

更新一下，因为我不搞黑苹果了，所以也没有新的群了，这个群已经满了，所以没有人退出的话也就没有新的人可以进去，这样马很好的，因为随着时间的流逝，群里的绝大多数人应该都自己会配置 EFI 了。

## 为什么造轮子?

为什么要重复造轮子呢？国光我不是一个喜欢重复造轮子的人，而且这个工作量本身也很大，平时的工作任务本身就很有挑战性了，还得抽出时间写这个系列，这不是自讨苦吃吗。所以我想分享一下，写这个系列的 Gitbook 的几个原因：

1. OpenCore 官方文档对小白不是很友好，也不符合国内的阅读习惯，阅读需要一定的门槛
2. OpenCore 黑苹果这块一直没有一个系统的教程，写这个系列日后还可以配合视频讲解在 B 站出一个教程系列
3. 授人以鱼不如授人以渔，与其等待大佬们的 EFI，不如自己动手自己配置一个自己的 EFI

## 关于 Hackintosh

凡是存在即合理，黑苹果的英文 Hackintosh，里面出现了 Hack，说到 Hack 就不得不提 Hacker 的几个基本的精神：热爱、叛逆、共享、开源、免费......

所以黑苹果本身也继承了这些特点，试想一下，如果著名的黑苹果 kexts 驱动：Liu、WhateverGreen、AppleALC 不开源的话，黑苹果技术还会和我们有关系吗？我们本质上就是一些 kexts 的搬运工，本身并没有创造什么，只是一些基本的排列组合。这也是国光我也坚持开源 EFI 的原因，毕竟喝水不忘挖井人。

好了，说了一堆乱七八糟的了，下面黑苹果教程正式开始。


## 参考资料

- [Dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/) 
- [[指南] hackintosh之SSDT/DSDT · Mac OS之程序员 · 看云](https://www.kancloud.cn/chandler/mac_os/482278#SSDTDSDT_9) 
- [DSDT - ArchWiki](https://wiki.archlinux.org/title/DSDT) 
- [黑果小兵的部落阁](https://blog.daliansky.net/)
- [黑苹果星球-分享Mac的精彩世界](https://heipg.cn/) 

