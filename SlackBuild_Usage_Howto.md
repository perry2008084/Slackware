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
 >> ./chemtool
 >>  |-- README
 >>  |-- chemtool.info
 >>  |-- chemtool.SlackBuild
 >>  |-- chemtool.desktop
 >>  |-- chemtool.png
 >>  |-- slack-desc
 
 匿名的[ftp站点](ftp://ftp.slackbuilds.org)，如果这对于你更方便
 访问。
 
 下一步，从chemtool.info文件所列的地址下载应用程序的源代码，并且
 放置在上述列出chemtool文件夹中。在[仓库](https://slackbuilds.org)中
 的每个应用程序页面都有一个源码包的直接链接。
 
 --------------------------------------------------------------
 步骤2 - 如有需要编辑SlackBuild脚本
 
 如果你的chemtool版本比在SlackBuild脚本中所写的版本更高，你需要
 更改