# 1. 环境配置

## 步骤

1. 安装Miniconda（推荐）或者Anaconda
  - 注意安装时要添加环境变量（默认不会勾上）
  - 使用conda创建新的环境: `conda create -n <环境名称> python=<python版本> -y`
  - （可选但推荐）为conda配置[清华源](https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/)
2. 安装深度学习框架（以`PyTorch为例`）
  - 有Nvidia独立显卡，且CUDA版本为11.8的：`pip install torch=1.12.0 torchvision=0.13.0 https://download.pytorch.org/whl/cu118`
  - 没有独立显卡的，上面的指令去掉后面的url即可
3. 下载D2L Notebook
  - 以此完成以下命令：
  ```
  mkdir d2l-zh && cd d2l-zh
  curl https://zh-v2.d2l.ai/d2l-zh-2.0.0.zip -o d2l-zh.zip
  unzip d2l-zh.zip && rm d2l-zh.zip
  cd pytorch
  ``` 
  - 随后可以通过`jupyter notebook`启动笔记本
