# Arch系搜狗输入法2.3.0.0109打包工程
![关于](http://yanxuan.nosdn.127.net/e902f7696f3141980390f4fb4435bc11.png)
# [点击下载](https://gitee.com/laomocode/fcitx-sogoupinyin/releases)
## 如何使用？
- 第一步，在发行版里下载安装文件。
- 第二步，到你下载的文件夹打开终端，输入:`pacman -U fcitx-sogoupinyin-2.3.0.0109-6-x86_64.pkg.tar.xz`(注意大小写)。
- 第三步，重启。  
这样，你就可以得到一个搜狗输入法2.3.0.0109的版本了。
## 有什么改进？
- 加入了五笔
- 从qt4框架迁移到qt5框架，可以解决ArchLinux\Manjaro因在他们的软件仓库删除了`fcitx-qt4`而无法使用搜狗输入法的问题
- 加入了符号大全
## 已知Bug：
- KDE桌面无法开启托盘菜单。
- 在多种输入法混合的情况下，皮肤会造成混乱。