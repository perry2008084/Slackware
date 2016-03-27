SlackBuild 使用说明

警告

slackbuilds.org上所有的编译脚本都是为Slackware最新的稳定发行版
所使用，如果你需要将这些脚本使用在旧版本的Slackware发行版，请
查看[FAQ](https://slackbuilds.org/faq/)中的
[说明页面](https://slackbuilds.org/howto/versions/)。

--------------------------------------------------------------
步骤1 - 下载

下载应用的SlackBuild压缩包，并且解压到你的编译路径下。例如，在
你解压chemtool.tar.gz压缩包后，你应该有以下的文件夹树：

```
 ./chemtool
  |-- README
  |-- chemtool.info
  |-- chemtool.SlackBuild
  |-- chemtool.desktop
  |-- chemtool.png
  |-- slack-desc
```

 匿名的[ftp站点](ftp://ftp.slackbuilds.org)，如果这对于你更方便
 访问。
 
 下一步，从chemtool.info文件所列的地址下载应用程序的源代码，并且
 放置在上述列出chemtool文件夹中。在[仓库](https://slackbuilds.org)中
 的每个应用程序页面都有一个源码包的直接链接。
 
 --------------------------------------------------------------
 步骤2 - 如有需要编辑SlackBuild脚本
 
 如果你的chemtool版本比在SlackBuild脚本中所写的版本更高，你需要
根据相应版本修改脚本。使用你最喜欢的编辑器，打开chemtool.SlackBuild
脚本，并且找到以VERSION开头的行。
>  VERSION=1.6.7

改变这一行来反映chemtool源码的当前版本。

* 如果有哪些新版本应用程序的靠修改VERSION字符串不能正确编译，请通过
提交报告让我们知道，提交到[SlackBuild Bugs](https://slackbuilds.org/bugs/)。

----------------------------------------------------------------
步骤3 - 执行SlackBuild脚本(使用root)

如果有需要通过chmod让脚本可执行：
> chmod +x chemtool.SlackBuild

接着允许脚本：
> ./chemtool.SlackBuild

注意，对于多数的编译，你需要一个真正登录shell来确保拥有一个正确的
通用环境。在其他事情中，/usr/share/texmf/bin将不会在你的环境变量PATH
中，如果你只是简单的用“su”--因此，你需要使用“su -l”当切换到root时，或者
做了“su”操作后更新(source)/etc/profile脚本，或者可能要修改/root/.bashrc来
包含必须的PATH元素。

-----------------------------------------------------------------
步骤4 - 安装软件包

假设所有的事情都根据计划进行（编译过程未报错），生成的软件包应该生成在
脚本中声明为“OUTPUT”的目录下（默认为/tmp目录）。使用installpkg来安装，
安装后你可能想要移动到其他位置来保存。

-----------------------------------------------------------------
其他资源

对于其他关于使用、编辑和创建SlackBuild脚本的信息，参考以下说明:
* [SlackWiki.com](SlackWiki.com)
* [SlackBuild Scripts Usage HOWTO](http://www.slackwiki.com/SlackBuild_Scripts)
* [SlackBuild Scripts Writing HOWTO](http://www.slackwiki.com/Writing_A_SlackBuild_Script)
