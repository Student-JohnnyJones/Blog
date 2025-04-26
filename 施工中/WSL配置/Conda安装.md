# Conda安装

### **1. 准备工作**

* 确保已启用 WSL 并安装 Linux 发行版（如 Ubuntu）。
* 打开 WSL 终端（如 Ubuntu）。

---

### **2. 下载 Miniconda 安装脚本**

推荐使用 **Miniconda**（轻量版），执行以下命令下载安装脚本：

```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

---

### **3. 运行安装脚本**

```bash
bash Miniconda3-latest-Linux-x86_64.sh
```

* 按回车阅读许可协议，输入 `yes` 同意条款。
* 设置安装路径（默认：`~/miniconda3`），直接回车使用默认路径。
* 安装完成后，选择是否初始化 Conda（输入 `yes`）。

------

### **4. 激活 Conda 环境**

关闭并重新打开终端，或手动激活配置：

```bash
source ~/.bashrc  # 如果使用 Bash
# 或
source ~/.zshrc   # 如果使用 Zsh
```

---

### **5. 验证安装**

```bash
conda --version
```

输出类似 `conda 24.5.0` 表示安装成功。

---

### **6. 基本使用**

- **查看环境**：

```bash
conda env list
```

* **创建新环境**：

```bash
conda create --name myenv python=3.9
```

- **激活环境**：

```bash
conda activate myenv
```

- **退出环境**：

```bash
conda deactivate
```

