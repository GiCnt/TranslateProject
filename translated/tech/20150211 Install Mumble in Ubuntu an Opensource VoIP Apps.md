Ubuntu上的一个开源VoIP应用——Mumble
================================================================================
Mumble是一个免费开源的VoIP应用，遵守New BSD License，主要面向的用户群体是玩家。运行起来类似于TeamSpeak和Ventrilo，用户通过连接到同一个服务器来实现相互通讯。

Mumble提供了如下的一些特性:

- 低延迟，这点对游戏相当重要
- 提供游戏中的可视插件，通过它你可以知道是谁正在和你通话并定位他们的位置
- 交谈内容经过加密的，能够保护你的隐私和安全
- 界面简单易于上手
- 稳定高效的使用你的服务器资源

### 安装 Mumble ###

[Mumble][1]已经流行开来，进入了许多linux主流发行版的软件仓库，这使它安装起来更加的方便。若你使用的是Ubuntu那么使用apt-get就能安装，详细命令如下：

    $ sudo apt-get install mumble-server

![mumble install](http://blog.linoxide.com/wp-content/uploads/2015/01/mumble-install.jpg)

这条命令将会在你的服务器上安装服务端（亦称Murmur）。

### 配置 Mumble ###

运行以下命令启动Mumble：

    $ sudo dpkg-reconfigure mumble-server

会弹出以下一些问题：

![mumble q1](http://blog.linoxide.com/wp-content/uploads/2015/01/mumble-q1.jpg)

选择“是”开机自动启动mumble，接着它会询问你是否运行高性能模式以保持低延迟，为了让它保持最佳性能这是个不错的主意。

![mumble q2](http://blog.linoxide.com/wp-content/uploads/2015/01/mumble-q2.jpg)

接着为你刚安装好的mumble服务端设置最高权限用户的密码，记住密码它会在登录时用到。

![mumble q3](http://blog.linoxide.com/wp-content/uploads/2015/01/mumble-q3.jpg)

### 安装 Mumble 客户端 ###

客户端可以安装到许多的主流操作系统中，例如windows，mac和linux。我们将教你在Ubuntu linux上安装和配置，你可以使用软件中心也可以用命令安装客户端：

    $ sudo apt-get install mumble

第一次运行mumble时，导向将会帮助你配置音频的输入输出，使其能在客户端上保持最好的效果。第一次同样也会询问你要使用的是什么声音设备和麦克风：

![mumble client 1](http://blog.linoxide.com/wp-content/uploads/2015/01/mumble-client-1.jpg)

然后它将帮你校准设备：

![mumble client 2](http://blog.linoxide.com/wp-content/uploads/2015/01/mumble-client-2.jpg)

因为mumble帮你加密所有的通讯内容所以它会征询你创建证书：

![mumble client 3](http://blog.linoxide.com/wp-content/uploads/2015/01/mumble-client-3.jpg)

完成导向后你就能添加第一个服务器，连接对话框如下图所示：

![mumble add server](http://blog.linoxide.com/wp-content/uploads/2015/01/mumble-add-server.jpg)

首先输入一个标签，名字任意因为那只不过是为了记住服务器的，然后输入服务器的地址和端口，最后使用“SuperUser”作为用户名而密码则是你配置mumble服务器端时输入的密码。

现在你可以连接到服务器了，在联网玩游戏或与你好友、队友聊天开黑时享受这些功能给你带来的乐趣吧！

--------------------------------------------------------------------------------

via: http://linoxide.com/ubuntu-how-to/install-mumble-ubuntu/

作者：[Adrian Dinu][a]
译者：[译者ID](https://github.com/译者ID)
校对：[校对者ID](https://github.com/校对者ID)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创翻译，[Linux中国](http://linux.cn/) 荣誉推出

[a]:http://linoxide.com/author/adriand/
[1]:http://wiki.mumble.info/wiki/Main_Page
