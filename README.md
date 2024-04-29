# yggycs-scale-sim

## 项目简介

学习 SCALE-Sim 模拟器的使用方法以及记录，开个仓库留存

原项目地址：https://github.com/scalesim-project/scale-sim-v2

## 环境配置

- **编辑器**：vscode

- **python 环境**：Anaconda3

1. 将原项目中 release v2.0.2 的源码下载并解压到该项目下

2. 创建一个新的 Python3 环境并配置

```powershell
# 进入原项目文件夹
cd .\scale-sim-v2-2.0.2\

# 查看 conda 已有环境
conda env list

# 创建一个新的 Python3 环境
conda create -n python3-scale-sim python=3.7

# 激活新环境
conda init
conda activate python3-scale-sim

# 安装依赖
pip3 install -r .\requirements.txt

# 安装 scale-sim-v2
python setup.py install

# 运行一个自带的测试 demo
python scale.py -c ../configs/eyeriss.cfg -t ../topologies/conv_nets/yolo.csv -i gemm

# 退出 conda 环境
conda deactivate

```