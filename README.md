# HSI-SVM

## 简介
　　针对高光谱遥感影像识别与分类中存在的问题，开展了以下几方面的研究工作。
+ 针对在实际应用中，当特征维数增加到某一个临界点时，继续增加特征维数反而会导致分类器的性能变差，即出现所谓的"休斯(Hughes)现象"的问题。提出了基于波段组合(2D)2PCA 的高光谱遥感影像降维方法，达到了降低数据冗余，消除"休斯现象"的目的，为后续的特征提取和分类工作奠定了基础。
+ 提出了基于双通道卷积神经网络的HSI空谱特征提取模型，该模型综合利用了高光谱遥感影像中所包含的光谱特征和空间特征，可有效的提高识别和分类的效率。
+ 针对分类器的泛化能力较弱的问题，提出了基于双通道CNN-SVM相融合的HSI识别与分类模型，该模型充分利用了卷积神经网络强大的图像特征提取能力，同时将SVM的泛化能力最大化，最大限度的提高了模型的分类精度，并将该模型应用到高光谱遥感影像分类中。

## 下载

```shell
git clone  https://github.com/Yangget/HSI-SVM.git
```
## 分割数据集

```
python create_PCA.py
```

## 训练一个简单的模型
```
python testmodel.py
```

## 训练HSI
```shell
cd Part_2
python HSI.py
```
#### HSI
![HIS_](https://github.com/Yangget/HSI-SVM/blob/master/Part_2/all.png)
#### HSI_K模型
![HIS_K](https://github.com/Yangget/HSI-SVM/blob/master/Part_2/HSI_K.png)
#### HSI_G模型
![HIS_G](https://github.com/Yangget/HSI-SVM/blob/master/Part_2/HSI_G.png)
#### HSI模型
![HIS](https://github.com/Yangget/HSI-SVM/blob/master/Part_2/HSI_A.png)

## 训练HSI_SVM
```shell
cd Part_3
python HSI.py
```
