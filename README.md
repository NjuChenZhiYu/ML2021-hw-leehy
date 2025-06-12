# 李宏毅2021机器学习作业思路

## 作业代码更新概述
- **HW01**：增加了 Adam, Momentum, Normalization, L2 regularization, Feature selection, K-fold cross validation 等相关代码，并使用了 Optuna 库进行了参数的自动搜寻。
- **HW02**：修改了原代码的小bug，增加了 tensorboard 和 scheduler 的使用，默认执行的是 strong baseline，你可以检查代码中的 TODO 选项去达成 Boss baseline（使用了BiLSTM）。
- **HW03**：代码根据 baseline 分为了三个部分(Medium, Strong,)，方便大家查看，之后的代码都会遵循这一点。代码仅针对 sample code 的基础架构进行了训练，所以没有达到 boss baseline。目前代码的分数为0.85200，先上传给大家一点参考思路，闲暇后会重新进行 boss baseline 的跟进。
- **HW04**：
  - Medium: 通过 grid search 搜寻了几十个参数组合后修改了 transformer 模块中的参数。
  - Strong:  Medium 的基础上修改使用了 Conformer 论文中的 ConformerBlock 架构。
  - Boss: 添加了 hints 中描述的 Self-Attention Pooling 和 Additive Margin Softmax 模块，但实际上仅需要将 Strong 中 Classifier 部分的 pred_layer 同 Conformer 本身一样修改为单层的全连接层便可以非常轻易的达到 Boss baseline。
- **HW05**：
  - Medium: 增加了学习率的调度和延长了训练的时间。
  - Strong: 将模型架构转变为了 Transformer，并根据 [Attention is all you need](https://arxiv.org/abs/1706.03762) 修改了模型的超参数。
  - Boss: 应用了 back-translation。
