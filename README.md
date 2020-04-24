# 搜狗输入法2.3.0.0109打包工程
```
这个工程弃坑了。
为什么弃坑呢？因为这个版本的搜狗输入法有很多问题，例如皮肤的问题、稳定性的问题……
而且，随着软件的更新，这个版本在最新的ArchLinux中似乎也没法使用了。
短暂的Qt5版本因为各种Bug，退回了Qt4。
至于这个版本的后续，我们也搞出来了。
在最近发布的Ubuntu Kylin 20.04 LTS中，里面的搜狗输入法变成了优麒麟的社区版。点开官网一看，这版本似乎是定制的版本。
于是我们打包出来，分享给大家。
哦，对了，这个版本不但会打包Arch Linux的版本，还会打包Ubuntu的版本。
因为最新的20.04删掉了Qt4，之前的版本没法用了。
地址：https://gitee.com/laomocode/fcitx-sogouimebs
```
![关于](http://yanxuan.nosdn.127.net/e902f7696f3141980390f4fb4435bc11.png)
# [码云下载](https://gitee.com/laomocode/fcitx-sogoupinyin/releases)
# [Github下载](https://github.com/laomocode/fcitx-sogoupinyin/releases)
## 如何使用？
### Arch Linux系
- 第一步，在下载页面里下载后缀为`.pkg.tar.xz`安装文件。
- 第二步，到你下载的文件夹打开终端，输入:`pacman -U fcitx-sogoupinyin-2.3.0.0109-6-x86_64.pkg.tar.xz`(注意大小写)。
- 第三步，重启。  
## Debian系
- 第一步，在下载页面里下载后缀为`.deb`的文件。
- 第二步，到你下载的文件夹打开终端，输入:`dpkg -i sogoupinyin.deb`(注意大小写)。
- 第三步，输入`sudo apt install -f`。  
- 第四步，重启。
## Ubuntu系
- 先按照Debian系的安装方法安装。
-  安装完成后，在命令行输入`sudo apt install libqt5widgets5 -y`，以解决无法使用问题。
这样，你就成功安装一个搜狗输入法2.3.0.0109的版本了。
## 有什么改进？
- 加入了五笔
- 从qt4框架迁移到qt5框架，可以解决ArchLinux\Manjaro因在他们的软件仓库删除了`fcitx-qt4`而无法使用搜狗输入法的问题
- 加入了符号大全
## 已知Bug：
- KDE桌面无法开启托盘菜单。
- 在多种输入法混合的情况下，皮肤会造成混乱。