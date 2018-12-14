# Google Fuchsia:美国国家安全局了解到的消息

​	前段时间，谷歌公布了Fuchsia并非Linux内核的消息，谁也不知道它以后是否能取代Android。美国国家安全局(NSA)在内的一些组织也在调查Fuchisa的进展 ，并将调查结果在加拿大温哥华的北美Linux安全峰会上进行公布。

### Fuchsia是一个模块化的操作系统。

​	詹姆斯·卡特和斯蒂芬·斯莫利对美国国家安全局透露了一些Fushsia的消息。他们将目光聚集在Fushsia的安全和Zircon的底层微核问题上。 

​	Zircon最开始是Android的引导程序的一个小内核，现在已经被修改成了一个微内核操作系统。它现在包括一小部分用户空间服务、驱动程序和库，被用做引导系统、与硬件对话、加载用户空间进程。Fuchsia 通过系统调用直接访问C++类来管理着几种不同的对象类型。

​	Zircon是一款不仅能在PC运行，在低功耗、最低资源的设备上也能使用的模块化操作系统。Zircon只需添加对象模块即可获得更多功能。

### Fuchsia与Unix/Linux的相似之处

​	Fuchsia还支持便携式操作系统接口(POSIX)协议。

​	这意味着从开发人员的角度来看，Fuchsia和Unix/Linux有些相像。Fuchsia 使用谷歌的Flutter框架作为软件开发工具包(SDK)。通过Flutter，开发人员可以构建Chrome OS和Android应用程序。同时，Fuchsia也支持苹果的Swift语言。

### Fuchsia面临的安全问题

​	斯莫利和卡特的任务是调查操作系统和软件在国家安全工作中的潜在隐患，美国国家安全局不希望政府使用脆弱的系统。

​	卡特还帮助美国国家安全局创造了运行最安全的Linux系统——SELinux。在测试Zircon和Fuchsia时，他们分享了关于操作系统的一些体会。

​	首先，他们发现Zircon是Fuchsia唯一以管理模式运行的部分，而其他的驱动程序、文件系统、网络等都是在用户模式下运行的。这意味着在Fuchsia上运行的程序所采取的方法与大多数操作系统上运行的程序有所不同。

​	随着研究的深入，他们也发现了许多安全问题。例如，如果在工程项目中任意获取句柄，会造成句柄的泄漏。这将对系统安全造成致命的危害。

### Fuchsia还有许多工作要做

​	Fuchsia的问题很大，到今年夏天，它还远远没有准备好生产。正如卡特所解释的，Fuchsia在很大程度上是一个尚未成型的系统，在 Fuchsia足够安全之前需要做很多工作。

​	与Linux相比，Fuchsia仍然不成熟，安全也远远不够。

​	卡特说，虽然许多工作需要做，但它会变得更安全，他鼓励开发人员在Fuchsia的安全上更多的投入。

​	不管成熟与否，Fuchsia可能很快就会用在谷歌的Home Hub上

### Fuchsia是否会应用在谷歌的Home Hub上？

​	Home Hub是一种新型的物联网设备。它是一个7英寸触摸屏，包括一个全距离扬声器，一个光传感器，和两个远场麦克风，不包括摄像机。在底层上，它使用的是Amlogic S905D2的CPU而不是高通SD624 SoC。

​ 一些人在*9to5Google*中疯狂钻研Fuchsia，并且不断挖掘GoogleHome Hub的源代码。他们在源码中发现了Fuchsia的踪迹。这意味着Home Hub可能会在圣诞时就会运行着Fuchsia！

​	国安局发现Fuchsia仍存在很多问题。但是如果你想体验Fuchsia，新的Home Hub是值得期待的。



****

本文作者为社区成员：VicZ，题图及内容翻译自

https://www.zdnet.com/article/google-fuchsia-heres-what-the-nsa-knows-about-it/
