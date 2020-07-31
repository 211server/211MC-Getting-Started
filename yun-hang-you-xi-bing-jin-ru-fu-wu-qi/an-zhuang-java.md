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
严重警告: 以上操作方法可能会导致JavaFX缺失，并且**不能**通过以下方式解决
```text
sudo apt install openjfx
```
正确的安装方式-使用[sdkman](https://sdkman.io/install)安装

使用以下三个命令，能够在Ubuntu 20.04上安装带有JavaFX的openjdk 8：

`curl -s "https://get.sdkman.io" | bash`

`source "$HOME/.sdkman/bin/sdkman-init.sh"`

`sdk install java 8.0.262.fx-zulu`


## Mac

```text
brew cask install java
```

或详见 [https://www.java.com/zh\_CN/download/help/mac\_install.xml](https://www.java.com/zh_CN/download/help/mac_install.xml)

