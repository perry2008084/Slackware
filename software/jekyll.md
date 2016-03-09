安装及使用

Linux平台下安装笔记
* 安装ruby(版本号需大于2.0.0)
* 安装rubygems
 - 下载官网的压缩包或者github上的源码（推荐源码）
  * git clone https://github.com/jekyll/jekyll.git'
  * # ruby setup.rb
* 通过rubygems安装jekyll
 - 由于国外的源有问题，需修改镜像地址
  * gem sources -r https://rubygems.org/
  * gem sources -a https://ruby.taobao.org/
  * gem -u
 - # gem install jekyl
 
 * 参考
 - [jekyll安装-知乎回答](http://www.zhihu.com/question/30018945)
 