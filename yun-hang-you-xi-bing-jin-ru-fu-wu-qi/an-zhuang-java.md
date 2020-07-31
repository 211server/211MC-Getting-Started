# 安装 Java

众所周知, Minecraft 使用 Java 语言编写. Java 是一种虚拟机语言, 所以为了运行它必须首先安装运行时\(Runtime\).

受限于游戏版本\(1.12.2\)和 Forge 版本\(1.12.2-14.23.5.2838\), 由于 Java9 及以上修改了 `UrlClassLoader` 的继承关系, 因此**不可用 Java8 以上的 Java 版本**. 请注意选择正确的 Java 版本!

## Windows

#### 命令行安装

如果已经安装有 Windows 包管理器, 例如 [choco](https://chocolatey.org) 请使用以下命令

```text
choco install javaruntime
```

[scoop](https://scoop.sh) 使用如下命令

```text
scoop bucket add java
scoop install openjdk
```

致命警告: 请注意下载的版本是否为 Java8.

#### 手动安装

使用浏览器打开以下网址 [https://www.java.com](https://www.java.com/)

![](../.gitbook/assets/image%20%284%29.png)

点击窗口中央的 "免费 Java 下载"

![](../.gitbook/assets/image%20%283%29.png)

此页面中央按钮下载得到的文件是在线安装器, 由于一些众所周知的原因, 国内网络在线安装比较困难, 请点击左侧的 "脱机安装程序" 链接获取离线安装包.

![](../.gitbook/assets/image%20%282%29.png)

由于 Windows 操作系统不额外强调 32位 与 [64位](https://zh.wikipedia.org/wiki/64%E4%BD%8D%E5%85%83) 软件, 因此**网页可能识别错误并给予 32位 Java 的离线下载地址**. 请再次点击左侧的 "所有 Java 下载" 并自行选择 Java 版本和 cpu 架构.

若中文页面的 “所有 Java 下载” 有错误, 请访问此英文页面 [https://www.java.com/en/download/manual.jsp](https://www.java.com/en/download/manual.jsp)

若有更多问题详见 [https://www.java.com/en/download/help/windows\_manual\_download.xml](https://www.java.com/en/download/help/windows_manual_download.xml)

轻微警告: 若下载缓慢请使用迅雷等工具下载.

严重警告: 若安装后没有自动添加 PATH 请手动添加, 详见 [https://www.java.com/en/download/help/path.xml](https://www.java.com/en/download/help/path.xml)

致命警告: 32位 Java 仅能使用至多 1GiB 的堆内存, 这远远达不到通常的 Minecraft 客户端所需, 因此你的计算机与操作系统以及 Java 运行时都必须为 amd64 或其兼容架构.

致命警告: 请注意下载的版本是否为 Java8.

## Linux

Debian/Ubuntu

```text
apt install openjdk-8-jre
```

轻微警告: 若系统中已安装其他版本 Java, 建议为 Java8 额外添加快捷方式, 例如

```text
ln -s /usr/lib/jvm/java-8-openjdk-amd64/bin/java /usr/bin/java8
```

致命警告: 启动器需要使用 [JavaFX](https://www.oracle.com/java/technologies/javase/javafx-overview.html) 库, 这在 openjdk 中是一个额外软件包, 请使用以下命令来安装

```text
apt install openjfx
```

此命令安装得到的 openjfx 可能对应 java 更高版本\(非 java8\), 请首先列出此软件包的全部版本

```text
apt list -a openjfx
```

命令执行结果例子:

```text
~$ apt list -a openjfx
正在列表... 完成
openjfx/bionic-updates,bionic-security 11.0.2+1-1~18.04.2 amd64
openjfx/bionic 8u161-b12-1ubuntu2 amd64
```

注意其中的 `8u161-b12-1ubuntu2` 版本, 接下去安装此版本.

```text
apt install openjfx=8u161-b12-1ubuntu2
```

`apt upgrade` 可能会自动将 openjfx 软件包更新至更高版本\(对应更高版本的 java\), 使用以下命令来锁定版本阻止自动升级

```text
apt-mark hold openjfx
```

其他发行版: 未测试

手动安装详见 [https://java.com/en/download/help/linux\_x64\_install.xml](https://java.com/en/download/help/linux_x64_install.xml)

## Mac

```text
brew cask install java
```

或详见 [https://www.java.com/en/download/help/mac\_install.xml](https://www.java.com/en/download/help/mac_install.xml)

