记录Slackware下安装Node.js的方法：

* 下载 Node.js源码

[Node.js](https://github.com/nodejs/node/archive/v4.2.4.tar.gz)

* 下载Slackbuild

本路径下的[nodejs.tar.gz](https://github.com/perry2008084/Slackware/blob/master/software/nodejs/nodejs.tar.gz)

* 解压Slackbuild

命令如下：
`cd /tmp
 mkdir nodejs
 cd ./nodejs
 tar -zxvf nodejs.tar.gz
`

* 拷贝Node.js源码到Slackbuild解压路径中

`
cp v4.2.4.tar.gz ./nodejs
`

* 编译

`
su
./nodejs.SlackBuild
`

* 将编译生成的文件进行安装即可。

`
installpkg xxxx.tgz
`
