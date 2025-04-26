# zsh配置与美化

本文是对“zsh配置与美化”一文的补充。

**powerlevel10k 字体问题**

在进行powerlevel10k时，如果lock图标显示不出来，就可能是字体问题。
浏览器打开https://github.com/romkatv/powerlevel10k?tab=readme-ov-file#fonts，找到下面的“Manual font installation”，下载字体文件，双击安装。
打开Terminal的设置（ctrl + ,），将字体更改为MesloLGS NF，保存即可。
回到Ubuntu，运行`p10k configure`，若能正常显示lock图标，则表示安装完成。

**插件列表**：
git
sudo
copypath
history
zsh-autosuggestions
zsh-syntax-highlighting
z
extract
web-search
conda-zsh-completion