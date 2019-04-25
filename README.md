# 多模态学习

1、多模态表示学习 Multimodal Representation

联合表示（Joint Representations）：联合表示将多个模态的信息一起映射到一个统一的多模态向量空间。

协同表示（Coordinated Representations）：协同表示负责将多模态中的每个模态分别映射到各自的表示空间，但映射后的向量之间满足一定的相关性约束（例如线性相关）。

2、模态转化 Translation

负责将一个模态的信息转换为另一个模态的信息.

eg:机器翻译、图片描述（Image captioning) 或者视频描述（Video captioning)、语音合成（Speech Synthesis）等

3、对齐 Alignment

多模态的对齐负责对来自同一个实例的不同模态信息的子分支/元素寻找对应关系。

eg:这个对应关系可以是时间维度的，比如下图所示的 Temporal sequence alignment，将一组动作对应的视频流同骨骼图片对齐。
类似的还有电影画面-语音-字幕的自动对齐。可以是空间维度的，图片语义分割 （Image Semantic Segmentation）

4、多模态融合 Multimodal Fusion

多模态融合（Multimodal Fusion ）负责联合多个模态的信息，进行目标预测（分类或者回归）。将多模态融合分为 pixel level，feature level 和 decision level。 三类，分别对应对原始数据进行融合、对抽象的特征进行融合和对决策结果进行融合。
而 feature level 又可以分为 early 和 late 两个大类，代表了融合发生在特征抽取的早期和晚期。当然还有将多种融合层次混合的 hybrid 方法。

eg:视觉-音频识别（Visual-Audio Recognition)、多模态情感分析（Multimodal sentiment analysis）、手机身份认证（Mobile Identity Authentication）

5、协同学习 Co-learning

使用一个资源丰富的模态信息来辅助另一个资源相对贫瘠的模态进行学习

eg:迁移学习（Transfer Learning）:零样本学习（Zero-Shot Learning）和一样本学习（One-Shot Learning）

协同训练（Co-training ），它负责研究如何在多模态数据中将少量的标注进行扩充，得到更多的标注信息。
