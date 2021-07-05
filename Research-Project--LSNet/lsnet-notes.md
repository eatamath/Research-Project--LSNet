

idea

- 原图multi-scale
- 整体可导

achive sota 水平







#### SNIP

image pyramid

多个detector分别约束不同scale的图片进行

减少domain-shift

实验显示了上采样对于检测小目标实例的重要性。

- 特定尺寸检测器：尺寸变化问题通过对每一个尺寸范围的实例训练一个单独的检测器得到解决。
  原因：在分类与检测数据集上使用相同尺寸的实例训练神经网络能减小域偏移。
  缺点：特定尺寸检测器的设计也减小每个尺寸的训练样本的数量，这会导致表现下降。
- 尺寸不变的检测器：使用所有的训练样本训练单一的目标检测器会导致学习任务变难。
  原因：因为神经网络需要在一个尺寸差异很大的检测实例上学习卷积核。

#### CenterNet

避免了NMS后处理

keypoints heatmap基于cornernet

cornernet给出了penalty的解释





### 参考文献

[FCOS：全卷积目标检测](https://www.jianshu.com/p/76c03635f8f9)

[目标检测论文解读（一）:FCOS原理解读](https://www.jianshu.com/p/fadaa61133fb)

[[读论文]Scale Normalization for Image Pyramids（小目标检测）](https://zhuanlan.zhihu.com/p/38557212)

[SNIP算法详解（极端尺寸检测）](https://blog.csdn.net/woduitaodong2698/article/details/86556206)

[RoI Transformer 精读](https://blog.csdn.net/qq_30612045/article/details/107741011)

[遥感检测——RoI Transformer（CVPR2019）](https://zhuanlan.zhihu.com/p/267484680)

[目标检测算法之ICCV 2019 TridentNet](https://cloud.tencent.com/developer/article/1558531)



FCOS

STN

SNIP

TridentNet

CornerNet

CenterNet