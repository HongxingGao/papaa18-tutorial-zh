# PAPAA'18 教程

本教程由帝国理工学院的陆永青教授制作，旨在介绍现场可编程逻辑门阵列（FPGA）上实现卷积神经网络的应用及工作原理。

## 大纲

教程大纲:

_A 部分_

-   [教程 1](https://github.com/corerain/papaa18-tutorial/blob/master/notebooks/01%20Introduction%20to%20CNN%20and%20TensorFlow.ipynb): TensorFlow 基础
-   [教程 2](https://github.com/corerain/papaa18-tutorial/blob/master/notebooks/02%20Build%20CNN%20in%20DFG%20IR.ipynb): 数据流图 IR 和 TensorFlow模型解析

_B 部分_

-   [教程 3](https://github.com/corerain/papaa18-tutorial/blob/master/notebooks/03%20Fixed-Point%20Representation%20of%20CNN.ipynb): CNN量化效应和探索
-   [教程 4](https://github.com/corerain/papaa18-tutorial/blob/master/notebooks/04%20Deploy%20DFG%20IR%20on%20FPGA.ipynb): 硬件设计生成和部署

```bash
.
├── data
│   ├── figs
│   └── mnist_model
└── notebooks  # 这里是教程
    └── Answer # 这里是答案，请尝试后再查看 ;)
├── model      # 这里是检查点文件和模型文件
   └── ssd_ckpt
```

## 安装及要求

### 第1步：VirtualBox

我们需要安装一台虚拟机，如果对此不熟悉，请参考以下步骤：

#### 步骤1.1: 下载VirtualBox 

请根据计算机系统和版本自行到以下网址进行下载：https://www.virtualbox.org/.

#### 步骤1.2 安装VirtualBox

请根据软件安装教程指导自行安装。

### 第2步：搭建虚拟机

#### 步骤2.1： 下载安装光盘

请下载 papaa-tutorial.ova映像文件，此文件已经预先安装所有的配置项，可直接使用。

AWS下载链接: <http://bit.ly/imperial_vm>. 

百度云链接 <https://pan.baidu.com/s/1A2barVEPNhvtUW1eR6gnjA>.

#### 步骤2.2：搭建和启动虚拟机

进入到VirtualBox点击`File -> Import Aplliance`, 找到下载的映像文件并将其加进目录，然后点击Continue继续。你会看到屏幕上显示所有设置已完成，你只需要点击Import导入。这个过程大约需要5-10分钟或者更少（取决于你的计算机）。

##### 步骤2.2.1：打开虚拟机

双击打开导入的虚拟机，让我们开始吧！

我们将在演示中主要使用python。 如果您不熟悉python，请查看此链接[Link](https://learnxinyminutes.com/docs/python/)。 该链接中很好的介绍了python的基础知识。


### 第3步：开始教程

```shell
# 进入教程的根目录
cd /home/jack/papaa18-tutorial/

# 进入python的虚拟环境
source venv/bin/activate

# 启动jupyter
jupyter notebook

# 你应该可以在终端界面上看到一个链接，如果你的浏览器自动打开了这个链接，
# 你就不需要把这个链接复制到你打开的浏览器地址栏了。
```

如果你想在自己的设备上安装`jupyter notebooks`, 执行如下命令：

```shell
# 假设你已经安装了pip
pip3 install --upgrade pip
pip3 install jupyter
```

## 联系我们

如果您想了解更多信息，请随时与我们联系:

-   Professor Wayne Luk (w.luk@imperial.ac.uk)

-   Martin Ferianc (martin.ferianc@corerain.com)

-   Ruizhe (Vincent) Zhao (vincent.zhao@corerain.com)
