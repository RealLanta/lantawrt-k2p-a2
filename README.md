<h1 align="center">
  <img src="https://cdn.jsdelivr.net/gh/RealLanta/lantawrt-k2p-a2/LantaWrt_Logo.png" alt="LantaWrt-K2P(A2)" width="400">
  <br>LantaWrt-K2P(A2)<br>

</h1>

  <p align="center">
    <a target="_blank" href="https://github.com/coolsnowwolf/lede">
    <img src="https://img.shields.io/badge/OpenWrt(LEDE) Kernel-r4491--d5622e353-blue">
  </a>
  <a target="_blank" href="https://github.com/RealLanta/lantawrt-k2p-a2/tree/0.1">
    <img src="https://img.shields.io/badge/source code-v0.1--beta-green.svg">
  </a>
  <a target="_blank" href="https://github.com/RealLanta/lantawrt-k2p-a2/releases">
    <img src="https://img.shields.io/badge/New Release-v0.1--beta-orange.svg">
  </a>
  </p>



<p align="center">
纯洁·轻量·美观
</p>
<p align="center">
本固件基于<a href="https://github.com/coolsnowwolf/lede">LEDE</a>编译、修改
</p>

已经编译好的固件请直接前往[Releases](https://github.com/jerrykuku/luci-app-vssr/releases)下载

默认登陆IP 192.168.87.1 密码 password

# 功能介绍

## 纯洁

LantaWrt-K2P(A2)非常的纯洁，提供了最基础的OpenWrt环境，极限压缩了EROM占用，给用户留了足够的空间安装额外插件

## 轻量

LantaWrt-K2P(A2)的资源占用非常低，默认情况下待机内存占用仅70M

![](https://cdn.jsdelivr.net/gh/RealLanta/lantawrt-k2p-a2/doc/2022-05-02_03-12.png)

## 美观

默认使用[Argon](https://github.com/jerrykuku/luci-theme-argon)主题，高雅而美观

![](https://cdn.jsdelivr.net/gh/RealLanta/lantawrt-k2p-a2/doc/2022-05-02_03-10.png)

![](https://cdn.jsdelivr.net/gh/RealLanta/lantawrt-k2p-a2/doc/2022-05-02_03-11.png)

## 更改

- 默认开启iPv6Helper
- 默认使用Argon作为主题

# 刷机方法

首先在Breed刷入`openwrt-ramips-mt7621-phicomm_k2p-initramfs-kernel.bin`

![](https://cdn.jsdelivr.net/gh/RealLanta/lantawrt-k2p-a2/doc/firmware.png)

进入系统后进入菜单`系统->备份/升级`

![](https://cdn.jsdelivr.net/gh/RealLanta/lantawrt-k2p-a2/doc/2022-05-02_03-15.png)

在下面的`刷写新的固件`**去掉**“保留配置”的勾选，并选择`openwrt-ramips-mt7621-phicomm_k2p-squashfs-sysupgrade.bin`刷入

![](https://cdn.jsdelivr.net/gh/RealLanta/lantawrt-k2p-a2/doc/2022-05-02_03-16.png)

![](https://cdn.jsdelivr.net/gh/RealLanta/lantawrt-k2p-a2/doc/2022-05-02_03-17.png)

# 自编译

LantaWrt的源编译文件是开放的，你可以Clone仓库直接开始编译

[查看编译文档](https://github.com/RealLanta/lantawrt-cr6608/blob/master/compile.md)

# 疑难解答

## 为什么我保存数据重启后就没有了？

这个是因为`openwrt-ramips-mt7621-phicomm_k2p-squashfs-sysupgrade.bin`没有刷入成功，通常升级一下Breed版本就可以了

前往[Breed下载站](https://breed.hackpascal.net/)寻找K2P

然后在你原本的Breed中把新版Breed拖到"Bootloader"选项

![](https://cdn.jsdelivr.net/gh/RealLanta/lantawrt-k2p-a2/doc/bootloader.png)

并刷入后即可升级Breed版本

升级好Breed之后重新刷入固件一般来说就能正常使用了
