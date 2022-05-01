<h1 align="center">
  <img src="https://cdn.jsdelivr.net/gh/RealLanta/lantawrt-k2p-a2/LantaWrt_Logo.png" alt="LantaWrt-CR6608" width="400">
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

LantaWrt非常的纯洁，只保留了最基本的功能

![](https://cdn.jsdelivr.net/gh/RealLanta/lantawrt-cr6608/doc/2022-04-30_13-30.png)

## 轻量

LantaWrt的资源占用非常低，默认情况下开启V2ray(WS+TLS)内存占用仅120M

![](https://cdn.jsdelivr.net/gh/RealLanta/lantawrt-cr6608/doc/2022-04-30_13-26.png)

## 美观

默认使用[Argon](https://github.com/jerrykuku/luci-theme-argon)主题，高雅而美观

![](https://cdn.jsdelivr.net/gh/RealLanta/lantawrt-cr6608/doc/2022-04-30_13-27.png)

## 更改

- 增加了[Hello World](https://github.com/jerrykuku/luci-app-vssr)（默认开启SSR、SS、V2ray、VLESS、Trojan的支持）
- 增加了Adbyby Plus+
- 增加了网络唤醒
- 增加了动态DNS
- 增加了KMS服务器
- 增加了htop（方便查看系统占用）
- 默认开启iPv6Helper

# 刷机方法

在Breed刷入`openwrt-ramips-mt7621-phicomm_k2p-initramfs-kernel.bin`即可

# 自编译

LantaWrt的源编译文件是开放的，你可以Clone仓库直接开始编译

[查看编译文档](https://github.com/RealLanta/lantawrt-cr6608/blob/master/compile.md)

