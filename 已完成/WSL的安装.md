# WSL的安装

## 什么是 WSL？

Windows Subsystem for Linux（简称 WSL）是微软为开发者提供的一种运行在 Windows 操作系统上的兼容层。它允许用户直接在 Windows 上运行原生的 Linux 命令行工具和应用程序，而无需传统的虚拟机或双系统启动方式。借助 WSL，开发者可以在 Windows 和 Linux 环境之间无缝切换，极大地提高了开发效率。
## 安装 WSL
WSL的安装总体分为2步，一步是在Windows上启用WSL，一步是在WSL里安装对应的Linux发行版。

#### 步骤1：事前准备

Win + R 输入control打开控制面板 -> 程序 -> 启用或关闭Windows功能，勾选“Virtual Machine Platform” “适用于Linux的Windows子系统”，选择确定，重启电脑

#### 步骤 2：启用 WSL 功能

1. 首先在系统上安装wsl，执行以下命令：
   ```powershell
   wsl --install
   ```

   这一步可能会很慢，甚至可能会因为网络问题报错，我们可以试试这样做
   ```powershell
   wsl --set-default-version 2
   # 随后按下任意键，即可下载，速度极快，比那个沟槽的下载速度快一万倍
   ```

2. 我们可以首先检查和设置wsl的基础信息，打开 PowerShell 作为管理员,运行以下命令：

   ```powershell
   # 这会输出wsl版本信息
   wsl --version
   # wsl -v
   
   # 这会输出wsl已经存在的Linux系统
   wsl --list --verbose
   # wsl -l -v
   
   # 这会更新wsl
   wsl --update
   
   # 这会将wsl设置为wsl2
   wsl --set-default-version 2
   ```

3. 接下来进行wsl里Linux系统的安装，执行以下命令：
   ```powershell
   # 这会列出所有的与WSL兼容的Linux发行版
   wsl --list --online
   # wsl -l -o
   
   # 安装想要的发行版
   wsl --install -d <distribution>
   
   # 以Ubuntu为例
   wsl --install -d Ubuntu
   ```

安装完成后，记得**重启计算机**以完成 WSL 的安装。