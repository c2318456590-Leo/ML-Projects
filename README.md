# Machine Learning Projects

机器学习项目集合，包含课程作业和个人练习。

## 项目列表

| 编号 | 项目 | 算法/框架 | 数据集 | 亮点 |
|------|------|----------|--------|------|
| 01 | [KNN 分类模型](./01-KNN-Classification/knn_classification.ipynb) | K近邻 (KNN) | sklearn内置：breast_cancer, wine | 决策边界可视化，参数调优曲线 |
| 02 | [CNN 猫狗分类](./02-CNN-CatDog/cnn_catdog_classification.ipynb) | PyTorch 卷积神经网络 | Kaggle Dogs vs. Cats | 自定义Dataset，数据增强，5层CNN架构 |
| 03 | [逻辑回归分类](./03-Logistic-Regression/logistic_regression.ipynb) | 逻辑回归 | sklearn内置：iris, breast_cancer | 三个层次任务：模拟数据→鸢尾花→乳腺肿瘤 |
| 04 | [加州房价预测](./04-California-Housing/california_housing.ipynb) | 线性回归/决策树/随机森林 | California Housing | Spark MLlib实现，多模型对比 |
| 05 | [线性回归作业](./05-Linear-Regression/linear_regression.ipynb) | 线性回归 | 自定义数据集 | 完整的数据预处理流程 |

## 环境依赖

```bash
# 基础环境
python >= 3.8

# 核心库
numpy
pandas
scikit-learn
matplotlib
seaborn

# 深度学习
torch
torchvision

# Spark (可选)
pyspark

# Notebook
jupyter
jupyterlab
```

## 快速开始

```bash
# 克隆仓库
git clone https://github.com/c2318456590-Leo/ML-Projects.git
cd ML-Projects

# 安装依赖
pip install -r requirements.txt

# 启动 Jupyter
jupyter notebook
```

## 项目说明

### 01-KNN-Classification
K近邻算法的教学演示项目，包含三个层次任务：
- 人工生成数据的二分类 + 决策边界可视化
- 红酒数据集的多分类
- 乳腺肿瘤良恶性二分类 + n_neighbors 参数调优曲线

### 02-CNN-CatDog
基于 PyTorch 实现的猫狗图像二分类项目：
- 自定义 `DogsVsCatsDatasets(Dataset)` 类封装数据加载
- 自定义 `DogsVsCatsModel(nn.Module)`：5层 Conv2d + BN + 4层 FC
- 数据增强：随机裁剪、水平翻转、归一化

### 03-Logistic-Regression
逻辑回归算法的基础演示：
- 模拟数据（复习时长/效率与及格关系）二分类
- 鸢尾花三分类
- 乳腺肿瘤二分类

### 04-California-Housing
基于 Spark MLlib 的加州房价预测项目：
- 数据预处理（缺失值填充、标准化）
- 多种回归模型对比（线性回归、决策树、随机森林）
- RMSE评估指标对比

### 05-Linear-Regression
线性回归基础作业：
- 单变量线性回归
- 多变量线性回归
- 梯度下降实现

## 许可证

仅供学习和展示用途。
