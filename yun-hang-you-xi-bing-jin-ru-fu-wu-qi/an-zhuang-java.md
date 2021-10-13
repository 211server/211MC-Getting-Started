# 安装 Java

如果不使用官方启动器, 可能需要额外安装 Java 运行时. **官方启动器用户请跳过此帮助**.

## Windows

#### 命令行安装

如果已经安装有 Windows 包管理器, 例如 [choco](https://chocolatey.org) 请使用以下命令

```
choco install javaruntime
```

[scoop](https://scoop.sh) 使用如下命令

```
scoop bucket add java
scoop install openjdk
```

#### 手动安装

使用浏览器打开以下网址 [https://www.java.com](https://www.java.com)

![](<../.gitbook/assets/image (1).png>)

点击窗口中央的 "免费 Java 下载"

![](<../.gitbook/assets/image (2).png>)

此页面中央按钮下载得到的文件是在线安装器, 由于一些众所周知的原因, 国内网络在线安装比较困难, 请点击左侧的 "脱机安装程序" 链接获取离线安装包.

![](<../.gitbook/assets/image (3).png>)

由于 Windows 操作系统不额外强调 32位 与 [64位](https://zh.wikipedia.org/wiki/64%E4%BD%8D%E5%85%83) 软件, 因此**网页可能识别错误并给予 32位 Java 的离线下载地址**. 请再次点击左侧的 "所有 Java 下载" 并自行选择 Java 版本和 cpu 架构.

若中文页面的 “所有 Java 下载” 有错误, 请访问此英文页面 [https://www.java.com/en/download/manual.jsp](https://www.java.com/en/download/manual.jsp)

若有更多问题详见 [https://www.java.com/en/download/help/windows_manual_download.xml](https://www.java.com/en/download/help/windows_manual_download.xml)

轻微警告: 若下载缓慢请使用迅雷等工具下载.

严重警告: 若安装后没有自动添加 PATH 请手动添加, 详见 [https://www.java.com/en/download/help/path.xml](https://www.java.com/en/download/help/path.xml)

致命警告: 32位 Java 仅能使用至多 1GiB 的堆内存, 这远远达不到通常的 Minecraft 客户端所需, 因此你的计算机与操作系统以及 Java 运行时都必须为 amd64 或其兼容架构.

## Linux

Debian/Ubuntu

```
apt install default-jre
```

致命警告: 部分启动器需要使用 [JavaFX](https://www.oracle.com/java/technologies/javase/javafx-overview.html) 库, 这在 openjdk 中是一个额外软件包, 请使用以下命令来安装

```
apt install openjfx
```

其他发行版: 未测试

手动安装详见 [https://java.com/en/download/help/linux_x64\_install.xml](https://java.com/en/download/help/linux_x64\_install.xml)

## Mac

```
brew cask install java
```

详见 [https://www.java.com/en/download/help/mac_install.xml](https://www.java.com/en/download/help/mac_install.xml)
