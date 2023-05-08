## 项目介绍

本项目包含三大模块：

1.计算特定矩阵的特征向量，并根据特征向量计算实耦合

2.从仿真数据或真人实验数据中计算出策略之间的协方差

3.对数据进行分析。将实耦合与协方差数据进行线性回归，计算相关系数，绘制拟合线段



## 项目配置：

环境：
python：3.9.12

编译器：
Visual Studio Code：1.77.3

插件：
Jupyter v2023.3.1201040234



## 文件介绍

from_eigenvector_out_XY.py：实现模块一，使用sympy库计算三种矩阵（A4，A5，Y5）的特征向量，并计算实耦合。其中A4矩阵需要一个参数，A5矩阵需要两个参数。具体见代码

calculate.py：实现从csv文件中计算策略之间的协方差。

demo.ipynb：Y5,A4,A5三种矩阵各自有一个demo。第一部分调用上述文件的函数得到计算结果，进行拟合，计算相关系数。第二部分分析数据，对数据结果绘制拟合线段。

data：数据文件，文件名格式：矩阵类型 + a值 + Strategy_distributions  数据来源：abed仿真

result：计算结果，文件名格式：矩阵类型 + a值 + result

figure：线性回归拟合的图形，其中A5矩阵对两种模式进行了二元线性回归

