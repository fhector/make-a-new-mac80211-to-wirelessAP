make-a-new-mac80211-to-wirelessAP
=================================

在新内核中copy一个mac80211模块作为可选模块并使用该模块实现无线AP。

首先下载一个新的内核。

然后copy net/mac80211 net/mac80211ext

修改相关Kconfig和makefile

修改.c中相关声明

之后，make Kconfig，选择mac80211ext编译为内核模块

make内核

重启使用新内核

查看mac80211ext是否可以工作

按照step1，重新配置无线网卡为无线AP。
