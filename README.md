# <p align="center"> 项目名称/论文名称 </p>

##### <p align="center"> [Wenjie Xu<sup>1,2</sup>](https://wenjiexucn.github.io/), Author<sup>1</sup>, Author<sup>2</sup>

##### <p align="center"> <sup>1</sup>Institutes of Science and Development, Chinese Academy of Sciences, Beijing 100190, China; <br> <sup>2</sup>School of Public Policy and Management, University of Chinese Academy of Sciences, Beijing 100049, China</p>

![Model](results/imgs/model.png)

---
This repository contains the source codes and data for our paper submitted and under review :

Wenjie Xu, Author, and Author, **项目名称/论文名称**.

The source code is mainly implemented in Python.

# Intro

在这一部分详细描述项目的背景、动机和研究问题。可以包括：

- 研究的领域背景
- 具体的研究问题或假设
- 项目的目标和期望解决的问题

例如：

> 本项目旨在研究使用机器学习模型预测房价的可行性。通过使用来自`Kaggle`的波士顿房价数据集，我们将探索不同模型的表现，并分析数据中的特征对价格的影响。

### 项目结构

简要描述项目的目录结构，帮助新开发者或合作者快速理解项目的组成部分。

```bash
project_name/
│
├── README.md               # 项目简介
├── requirements.txt        # Python依赖库
├── setup.py                # 项目安装配置（可选）
├── data/                   # 数据目录
│   ├── raw/                # 原始数据
│   ├── processed/          # 处理过的数据
│
├── notebooks/              # Jupyter notebooks
│   ├── exploration.ipynb   # 数据探索分析
│   └── experiment.ipynb    # 实验分析
│
├── src/                    # 代码目录
│   ├── __init__.py         # 使其成为包
│   ├── data_loader.py      # 数据加载模块
│   ├── preprocess.py       # 数据预处理模块
│   ├── model.py            # 模型定义模块
│   └── train.py            # 训练模型模块
│
├── tests/                  # 单元测试目录
├── logs/                   # 训练或实验日志
├── results/                # 实验结果
└── config/                 # 配置文件
```

# Installation

详细描述如何安装和配置项目。这部分可能包括如何获取代码、安装依赖项、配置数据路径等。

### Environment

- **Tested OS:** Windows
- Python >= 3.10

### Dependencies

1. Run `pip install -r requirements.txt` to install all dependencies required in your machine.
2. Import [PyTorch](https://pytorch.org) with the correct CUDA version.

The installation time will take no longer than 30 minutes on a "normal" desktop computer with good Internet conditions.

### Data availability

You can access the data from [Google Drive link](https://drive.google.com/drive/folders/1HTYuJuaRMUV2grBbELBRpB6ZnkRXsc4A?usp=sharing).

Download the data and put it into the `data` folder.

# 使用说明

列出如何运行代码或项目的主要功能。可以包括具体的命令行指令或使用示例。

```bash
# 运行数据预处理
python src/preprocess.py --input data/raw/dataset.csv --output data/processed/processed_data.csv

# 训练模型
python src/train.py --config config/config.yaml
```

如果项目涉及Jupyter Notebook，可以说明如何打开和运行notebooks：

```bash
# 启动Jupyter Notebook
jupyter notebook notebooks/exploration.ipynb
```

# 实验/结果

列出项目的实验设计和结果，通常包括以下内容：

- 不同实验的设置
- 模型性能的比较（例如，准确率、F1分数等）
- 可视化结果（可以插入模型的性能图表、混淆矩阵等）

示例：

> 我们在训练集中使用了多种模型，包括线性回归和随机森林模型。实验结果表明，随机森林模型在测试集上的表现更优，MSE为0.15，而线性回归模型的MSE为0.22。

**图表1：模型性能比较**

```
| 模型           | MSE  |
| -------------- | ---- |
| 线性回归       | 0.22 |
| 随机森林       | 0.15 |
| 支持向量机     | 0.18 |
```

# 贡献

如果你希望别人贡献代码或实验，可以说明如何贡献：

> 欢迎任何形式的贡献！你可以通过以下方式贡献：
>
> 1. Fork 本项目
> 2. 创建你自己的分支 (`git checkout -b feature/AmazingFeature`)
> 3. 提交你的更改 (`git commit -m 'Add some AmazingFeature'`)
> 4. Push 到你的分支 (`git push origin feature/AmazingFeature`)
> 5. 创建一个 Pull Request

# 许可证

> 本项目使用 [GPL v3.0 License](LICENSE) 进行授权。请在使用本项目代码时遵循相关许可规定。
