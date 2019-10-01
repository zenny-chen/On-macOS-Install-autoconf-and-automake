# On-macOS-Install-autoconf-and-automake
macOS下安装autoconf与automake以及其相关的库

<br />

我们首先要安装M4库，可以在此链接中获取：http://mirrors.kernel.org/gnu/m4/ 。我们选择最新发布的库进行下载，如何挑选当前是最新的呢？各位主要看中间一栏的发布日期，这个是最准的。这里大家还要注意的是，发布日期是有些乱序的，因此需要注意观察。如果下载的库太老，那么会影响后续库的编译，所以各位应该要选择较新的库才行。然后我们要下载的文件应该以 **.tar.gz** 结尾。
下载完毕后，我们打开命令行，进入到该文件所在的目录，再使用`tar -xzvf  <文件名>`进行解压，然后进入到解压后的文件夹。然后使用以下命令进行安装：
```makefile
./configure --prefix=/usr/local
make
sudo make install
```

然后下载autoconf库，链接为：http://mirrors.kernel.org/gnu/autoconf/ ，同样选择最新的发布版本，跟上面操作一样进行解压安装。autoconf库安装好之后我们可以先关掉控制台，然后再重新打开它，确保autoconf已经完全起作用了。

接着，我们下载automake库，链接为：http://mirrors.kernel.org/gnu/automake/ ，同样选择最新的发布版本，跟上面操作一样进行解压安装。

最后，我们下载libtool工具库，链接为：http://mirrors.kernel.org/gnu/libtool/ ，同样选择最新的发布版本，跟上面操作一样进行解压安装。

这样就把这些基本的需要编译很多开源软件的库都安装好了。

