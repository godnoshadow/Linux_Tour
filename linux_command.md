

：w ! sudo tee % vim强制保存

sudo ./BaiduPCS-Go 登录百度网盘下载软件（linux）

dpkg --info linux.deb查看安装的linux.deb放在哪里

service v2ray start

python(linux) 2.7.15+

python 3.7.4

查找...——find -name ...

一般来说著名的 Linux 系统基本上分两大类：

    RedHat 系列：Redhat、Centos、Fedora 等
    Debian 系列：Debian、Ubuntu 等

Dpkg (Debian系)：Ubuntu
RPM (Red Hat系)：CentOS、Fedora

RedHat 系列

    常见的安装包格式 rpm 包，安装rpm包的命令是“rpm -参数”
    包管理工具 yum
    支持 tar 包

Debian系列

    常见的安装包格式 deb 包，安装 deb 包的命令是“dpkg -参数”
    包管理工具 apt-get
    支持 tar 包

tar 只是一种压缩文件格式，所以，它只是把文件压缩打包而已。

rpm 相当于windows中的安装文件，它会自动处理软件包之间的依赖关系。优缺点来说，rpm一般都是预先编译好的文件，它可能已经绑定到某种CPU或者发行版上面了。

列出系统中已安装的所有套件：
```
dkpg -l

rpm -qa  

yum list installed
```





# 在Linux环境下编python脚本

1、首先定位到一个文件夹，然后使用vim编辑器：vim test.py 就创建了python脚本文件，并且进入编辑状态

2、编辑好之后按Esc切换到命令模式，然后输入：wq 回车就自动保存完成了，然后输入python  test.py运行程序（前提是linux环境装好python）          nohub  python test.py &     可以在后台运行。。不受shell退出影响

 

下面说下vim编辑器：

vim编辑器的工作模式有三种：命令模式，输入模式，末行模式。

（1）模式之间的切换：

当打开一个文件的时候默认是处于命令模式，在命令按i或者insert就可以进入输入模式，在输入模式下按Esc就可以切换回命令模式；在命令模式下，按shift+；，末行出现：，则进入末行模式，按q可以退出末行模式。

（2）进入文件编辑，保存退出文件

vim   filename 如果文件不存在就自动创建该名字的文件且进入，如果文件存在就直接进入该文件。

***vim常用命令：***

1. 键入i进入编辑模式
2. esc进入命令模式
3. a,进入编辑模式
4. b,光标移动到单词前，end,光标移动到行尾
5. home光标移动到行首
6. cc,删除当前行，并进入编辑模式
7. x 删除当前光标所在处的字符。
8. u，撤销，ctrl+r，反撤销
9. h,j,k,l,前下上后，光标移动
10. v,进入选择，y复制，p粘贴
11. 光标移动最后，yy复制当前行 。nyy复制当前n行。G，光标移动至尾行。gg光标移动至首行，nG,光标移动第n行。
11. ：set nu显示行号，：set nonu,取消行号
12. /user,查找user,/keyword,,n,向后N向前查看
13. /3$,查找以3结尾
14. :nohl，关闭高亮提示
15. ：q,退出，：q!,强制退出。
16. :wq,保存退出，：wq!，强制保存退出
17. ：w,写入。：w filename,将当前文件写入filename中
18. ：w>>filename，将当前文件追加到filename中
19. 2,4 w>>filename,将当前2到4行，追加到filename.
20. ：%s/usr/user/g,将所有（全文）usr替换为user，可以使用正则。。。不加g只替换一次，（当前行第一行）
21. ：%s/usr/user/g,将当前usr替换为user
    %全文，g，全部，i，不区分大小写、、\转义
22. ：!,临时执行命令





| 连接方式    | 功能                           |
| ----------- | ------------------------------ |
| 直接连接    | 所有访问都不是使用代理。       |
| 系统代理    | 访问网站与系统的默认代理有关。 |
| Shadowsocks | 所有访问都使用代理。           |
| 自动切换    | 所有访问都使用代理。           |





vi ...   打开文本文件

eog ...  /   xdg-open  ....    打开图片



### vim

:w -- write a file                                               写入文件

!sudo -- Call shell sudo command         调用shell sudo 命令

tee -- the output of write (vim :w) command redirected using tee. 

使用tee重定向的write命令的输出

% -- is nothing but current file name   只不过是当前文件名



proxychains 命令行代理

sudo apt-get install

rm XXX -rf 删除thing

ps -ef | grep v2ray 获取v2ray进程的相关信息

tmux

zsh 命令行补全

exit 退出终端命令