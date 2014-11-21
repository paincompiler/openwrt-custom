##综合课程设计小组 working source code

这里有鸟叔和川川还有我，加油。

请相关人员把 rsa public key 发给我

在终端运行命令：

```
#ssh-keygen
```

依照步骤最终生成 RSA key （一路回车就行了）

在用户文件夹下（类unix系统在 ~/.ssh/ 中，Windows 在用户文件夹/.ssh/ ）找到 rsa_key.pub 文件，发给我


###使用指南

1.将代码 clone 到本地：

```
#git clone git@github.com:paincompiler/openwrt-custom.git
```

2.切换到自己的工作分支（以鸟叔为例）：

```
#git checkout dev-btboy
```

3.改改改！更改后的文件存储更改：

```
#git add xxxx.h
```

4.确认更改完毕后（尽量做了一次更改就提交一次），提交 commit ：

```
#git commit -m 'xxxx.h modified'

ps: -m 参数后面跟更改说明
```

5.同步到远端代码库：

```
#git push origin dev-btboy
```

###注意事项

1.切勿切换到别人的分支和 master 分支进行修改，只在自己的分支工作

2.及时保存和提交自己的更改

3.有任何阶段性的成果，一起确认没有问题可以工作后，请在仓库页面提交 pull request 申请合并到 master 分支


<hr>

This is the buildsystem for the OpenWrt Linux distribution.

Please use "make menuconfig" to configure your appreciated
configuration for the toolchain and firmware.

You need to have installed gcc, binutils, bzip2, flex, python, perl, make,
find, grep, diff, unzip, gawk, getopt, subversion, libz-dev and libc headers.

Run "./scripts/feeds update -a" to get all the latest package definitions
defined in feeds.conf / feeds.conf.default respectively
and "./scripts/feeds install -a" to install symlinks of all of them into
package/feeds/.

Use "make menuconfig" to configure your image.

Simply running "make" will build your firmware.
It will download all sources, build the cross-compile toolchain, 
the kernel and all choosen applications.

You can use "scripts/flashing/flash.sh" for remotely updating your embedded
system via tftp.

The OpenWrt system is documented in docs/. You will need a LaTeX distribution
and the tex4ht package to build the documentation. Type "make -C docs/" to build it.

To build your own firmware you need to have access to a Linux, BSD or MacOSX system
(case-sensitive filesystem required). Cygwin will not be supported because of
the lack of case sensitiveness in the file system.


Sunshine!
	Your OpenWrt Project
	http://openwrt.org


