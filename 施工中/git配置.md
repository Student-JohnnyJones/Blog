# Git配置

Git下载页：[Git - Downloading Package](https://git-scm.com/downloads/win)

在下载页点击“**[64-bit Git for Windows Setup](https://github.com/git-for-windows/git/releases/download/v2.49.0.windows.1/Git-2.49.0-64-bit.exe)**”，即可下载Git。

安装操作：
①路径改成D盘
②默认编辑器改成VSCode
③分支名选择main
④HTTPS transport backend改成“Use the OpenSSL library”
然后后面一路默认安装即可

安装完成会看到“Launch Git Bash”和“View Release Notes”，全部取消勾选即可。

打开cmd，输入`git --version`，能够输出git版本，则安装过程正常。重启vscode，按下ctrl + shift + G，可以看到两个蓝色框