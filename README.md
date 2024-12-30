# Readme
本项目包括三个阶段，数据探索，机器学习数据分析及预测，深度学习数据预测三个部分。

为了省略数据预处理的时间，代码中涉及处理-保存数据-读取数据的部分皆注释前两个部分，直接快进到读取数据，如果要复现代码，需要在运行的时候手动运行注释部分。



实验所需硬件设备为4090（128g ram）

## 数据探索

`quickstat.Rmd`

`feature_engineering.Rmd`

`PySmiles.ipynb`

`EDA_Smiles.ipynb`

`Module_Representations.ipynb`衔接后续机器学习`ML_Morgan_Training.ipynb`



## 机器学习数据分析及预测

`ML_Preprocessing.ipynb`提取表层数据特征进行训练

`ML_Morgan_Training.ipynb`提取morgan数据特征进行训练



## 深度学习数据预测

`BELKA_CNN.ipynb`1D卷积训练全部数据（约$1 \times 10^9$条数据，三种label）训练时间900min

`BELKA_KANLinear.ipynb`1D卷积+KANLinear训练全部数据，（约$1 \times 10^9$条数据，三种label）训练时间700min

`BELKA_Transformer.ipynb`CNN+Transformers训练30%数据

`BELKA_1D_GNN.ipynb`图神经网络（1D图卷积+linear）训练1%数据

`BELKA_GNN.ipynb`图神经网络小样本训练