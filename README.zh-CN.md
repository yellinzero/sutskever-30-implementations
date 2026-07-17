# Sutskever 30——完整实现套件

[English](README.md) | 简体中文

> 本文件是 [`pageman/sutskever-30-implementations`](https://github.com/pageman/sutskever-30-implementations) 的非官方中文学习译本，仅用于个人学习与交流。原项目、代码及相关内容的权利归原作者所有。翻译可能存在疏漏，请以英文原文为准。

**用简单但完整的代码，实现 Ilya Sutskever 推荐的 30 篇奠基性论文**

[![实现进度](https://img.shields.io/badge/实现进度-30%2F30-brightgreen)](https://github.com/pageman/sutskever-30-implementations)
[![覆盖率](https://img.shields.io/badge/覆盖率-100%25-blue)](https://github.com/pageman/sutskever-30-implementations)
[![Python](https://img.shields.io/badge/Python-仅使用%20NumPy-yellow)](https://numpy.org/)

[**在 Gumroad 购买本仓库对应的 Google Colab 代码**](https://pageman.gumroad.com/l/sutskever30colabcode)

## 项目概述

本仓库对 Ilya Sutskever 著名阅读清单中的论文进行了详细、面向教学的实现。据称，他曾告诉 John Carmack：学完这个清单，就能掌握深度学习中“90% 真正重要的内容”。

**进度：30/30 篇（100%）——全部完成！🎉**

每个实现都具有以下特点：

- ✅ 仅使用 NumPy，不依赖深度学习框架，便于理解底层原理
- ✅ 内置合成或自举数据，可以立即运行
- ✅ 包含丰富的可视化和讲解
- ✅ 展示每篇论文的核心概念
- ✅ 使用 Jupyter Notebook，便于交互式学习

## 快速开始

```bash
# 进入项目目录
cd sutskever-30-implementations

# 安装依赖
pip install numpy matplotlib scipy

# 运行任意 Notebook
jupyter notebook 02_char_rnn_karpathy.ipynb
```

## Sutskever 30 篇论文

### 基础概念（论文 1～5）

| # | 论文 | Notebook | 核心概念 |
|---|------|----------|----------|
| 1 | 复杂动力学第一定律（The First Law of Complexodynamics） | ✅ `01_complexity_dynamics.ipynb` | 熵、复杂度增长、元胞自动机 |
| 2 | RNN 不可思议的有效性（The Unreasonable Effectiveness of RNNs） | ✅ `02_char_rnn_karpathy.ipynb` | 字符级模型、RNN 基础、文本生成 |
| 3 | 理解 LSTM 网络（Understanding LSTM Networks） | ✅ `03_lstm_understanding.ipynb` | 门控、长期记忆、梯度流 |
| 4 | RNN 正则化（RNN Regularization） | ✅ `04_rnn_regularization.ipynb` | 序列 Dropout、变分 Dropout |
| 5 | 保持神经网络简单（Keeping Neural Networks Simple） | ✅ `05_neural_network_pruning.ipynb` | MDL 原理、权重剪枝、90% 以上稀疏度 |

### 架构与机制（论文 6～15）

| # | 论文 | Notebook | 核心概念 |
|---|------|----------|----------|
| 6 | 指针网络（Pointer Networks） | ✅ `06_pointer_networks.ipynb` | 作为指针的注意力、组合问题 |
| 7 | ImageNet/AlexNet | ✅ `07_alexnet_cnn.ipynb` | CNN、卷积、数据增强 |
| 8 | 顺序很重要：面向集合的 Seq2Seq | ✅ `08_seq2seq_for_sets.ipynb` | 集合编码、置换不变性、注意力池化 |
| 9 | GPipe | ✅ `09_gpipe.ipynb` | 流水线并行、微批次、重计算 |
| 10 | 深度残差学习（ResNet） | ✅ `10_resnet_deep_residual.ipynb` | 跳跃连接、梯度高速通道 |
| 11 | 空洞卷积（Dilated Convolutions） | ✅ `11_dilated_convolutions.ipynb` | 感受野、多尺度 |
| 12 | 神经消息传递（GNN） | ✅ `12_graph_neural_networks.ipynb` | 图网络、消息传递 |
| 13 | **注意力就是你所需要的一切** | ✅ `13_attention_is_all_you_need.ipynb` | Transformer、自注意力、多头注意力 |
| 14 | 神经机器翻译 | ✅ `14_bahdanau_attention.ipynb` | Seq2seq、Bahdanau 注意力 |
| 15 | ResNet 中的恒等映射 | ✅ `15_identity_mappings_resnet.ipynb` | 预激活、梯度流 |

### 进阶主题（论文 16～22）

| # | 论文 | Notebook | 核心概念 |
|---|------|----------|----------|
| 16 | 关系推理（Relational Reasoning） | ✅ `16_relational_reasoning.ipynb` | 关系网络、成对函数 |
| 17 | **变分有损自编码器** | ✅ `17_variational_autoencoder.ipynb` | VAE、ELBO、重参数化技巧 |
| 18 | **关系型 RNN** | ✅ `18_relational_rnn.ipynb` | 关系记忆、多头自注意力、手动反向传播（约 1100 行） |
| 19 | 咖啡自动机（The Coffee Automaton） | ✅ `19_coffee_automaton.ipynb` | 不可逆性、熵、时间箭头、Landauer 原理 |
| 20 | **神经图灵机** | ✅ `20_neural_turing_machine.ipynb` | 外部记忆、可微寻址 |
| 21 | Deep Speech 2（CTC） | ✅ `21_ctc_speech.ipynb` | CTC 损失、语音识别 |
| 22 | **缩放定律（Scaling Laws）** | ✅ `22_scaling_laws.ipynb` | 幂律、计算最优训练 |

### 理论与元学习（论文 23～30）

| # | 论文 | Notebook | 核心概念 |
|---|------|----------|----------|
| 23 | MDL 原理 | ✅ `23_mdl_principle.ipynb` | 信息论、模型选择、压缩 |
| 24 | **机器超级智能** | ✅ `24_machine_super_intelligence.ipynb` | 通用 AI、AIXI、Solomonoff 归纳、智能度量、自我改进 |
| 25 | Kolmogorov 复杂度 | ✅ `25_kolmogorov_complexity.ipynb` | 压缩、算法随机性、通用先验 |
| 26 | **CS231n：用于视觉识别的 CNN** | ✅ `26_cs231n_cnn_fundamentals.ipynb` | 图像分类流程、kNN/线性模型/神经网络/CNN、反向传播、优化、训练调试 |
| 27 | 多词元预测 | ✅ `27_multi_token_prediction.ipynb` | 同时预测多个未来词元、样本效率、速度提升 2～3 倍 |
| 28 | 稠密段落检索 | ✅ `28_dense_passage_retrieval.ipynb` | 双编码器、MIPS、批内负样本 |
| 29 | 检索增强生成 | ✅ `29_rag.ipynb` | RAG-Sequence、RAG-Token、知识检索 |
| 30 | 中间信息丢失（Lost in the Middle） | ✅ `30_lost_in_middle.ipynb` | 位置偏差、长上下文、U 形曲线 |

## 精选实现

### 🌟 必读 Notebook

这些实现涵盖最具影响力的论文，并展示深度学习的核心概念。

#### 基础

1. **`02_char_rnn_karpathy.ipynb`**——字符级 RNN
   - 从零构建 RNN
   - 理解随时间反向传播（BPTT）
   - 生成文本

2. **`03_lstm_understanding.ipynb`**——LSTM 网络
   - 实现遗忘门、输入门和输出门
   - 可视化门激活值
   - 与普通 RNN 比较

3. **`04_rnn_regularization.ipynb`**——RNN 正则化
   - RNN 的变分 Dropout
   - 正确放置 Dropout
   - 改进训练过程

4. **`05_neural_network_pruning.ipynb`**——网络剪枝与 MDL
   - 基于权重幅值的剪枝
   - 迭代剪枝与微调
   - 在损失很小的情况下实现 90% 以上稀疏度
   - 最小描述长度（MDL）原理

#### 计算机视觉

5. **`07_alexnet_cnn.ipynb`**——CNN 与 AlexNet
   - 从零实现卷积层
   - 最大池化与 ReLU
   - 数据增强技术

6. **`10_resnet_deep_residual.ipynb`**——ResNet
   - 用跳跃连接解决网络退化问题
   - 梯度流可视化
   - 理解恒等映射

7. **`15_identity_mappings_resnet.ipynb`**——预激活 ResNet
   - 比较预激活与后激活
   - 改善梯度流
   - 训练超过 1000 层的网络

8. **`11_dilated_convolutions.ipynb`**——空洞卷积
   - 多尺度感受野
   - 无需池化
   - 语义分割

#### 注意力与 Transformer

9. **`14_bahdanau_attention.ipynb`**——神经机器翻译
   - 原始注意力机制
   - 带对齐机制的 Seq2seq
   - 注意力可视化

10. **`13_attention_is_all_you_need.ipynb`**——Transformer
    - 缩放点积注意力
    - 多头注意力
    - 位置编码
    - 现代大语言模型的基础

11. **`06_pointer_networks.ipynb`**——指针网络
    - 将注意力用作选择机制
    - 组合优化
    - 可变输出大小

12. **`08_seq2seq_for_sets.ipynb`**——面向集合的 Seq2Seq
    - 具有置换不变性的集合编码器
    - Read-Process-Write 架构
    - 对无序元素应用注意力
    - 排序与集合运算
    - 比较顺序敏感与顺序不变模型

13. **`09_gpipe.ipynb`**——GPipe 流水线并行
    - 将模型拆分到多个设备
    - 用微批次提升流水线利用率
    - F-then-B 调度：先完成全部前向传播，再完成全部反向传播
    - 重计算，也称梯度检查点
    - 流水线气泡时间分析
    - 训练单个设备内存无法容纳的大模型

#### 进阶主题

14. **`12_graph_neural_networks.ipynb`**——图神经网络
    - 消息传递框架
    - 图卷积
    - 分子性质预测

15. **`16_relational_reasoning.ipynb`**——关系网络
    - 成对关系推理
    - 视觉问答
    - 置换不变性

16. **`18_relational_rnn.ipynb`**——关系型 RNN
    - 结合关系记忆的 LSTM
    - 跨记忆槽的多头自注意力
    - 架构演示（前向传播）
    - 序列推理任务
    - **第 11 节：手动实现反向传播（约 1100 行）**
    - 完整计算所有组件的梯度
    - 使用数值方法验证梯度

17. **`20_neural_turing_machine.ipynb`**——记忆增强网络
    - 基于内容和位置的寻址
    - 可微读写
    - 外部记忆

18. **`21_ctc_speech.ipynb`**——CTC 损失与语音识别
    - 连接主义时间分类（CTC）
    - 无需对齐的训练
    - 前向算法

#### 生成模型

19. **`17_variational_autoencoder.ipynb`**——VAE
    - 生成建模
    - ELBO 损失
    - 潜在空间可视化

#### 现代应用

20. **`27_multi_token_prediction.ipynb`**——多词元预测
    - 预测多个未来词元
    - 提高 2～3 倍样本效率
    - 推测式解码
    - 加快训练与推理

21. **`28_dense_passage_retrieval.ipynb`**——稠密检索
    - 双编码器架构
    - 批内负样本
    - 语义搜索

22. **`29_rag.ipynb`**——检索增强生成（RAG）
    - 比较 RAG-Sequence 与 RAG-Token
    - 结合检索与生成
    - 基于知识的输出

23. **`30_lost_in_middle.ipynb`**——长上下文分析
    - 位置偏差
    - U 形性能曲线
    - 文档排序策略

#### 缩放与理论

24. **`22_scaling_laws.ipynb`**——缩放定律
    - 幂律关系
    - 计算最优训练
    - 性能预测

25. **`23_mdl_principle.ipynb`**——最小描述长度
    - 基于信息论的模型选择
    - 压缩即理解
    - 比较 MDL、AIC 与 BIC
    - 神经网络架构选择
    - 基于 MDL 的剪枝，与论文 5 相呼应
    - Kolmogorov 复杂度预览

26. **`25_kolmogorov_complexity.ipynb`**——Kolmogorov 复杂度
    - K(x) 表示生成 x 的最短程序
    - 随机性等价于不可压缩性
    - 算法概率（Solomonoff）
    - 用于归纳的通用先验
    - 与 Shannon 熵的联系
    - 对奥卡姆剃刀的形式化
    - 机器学习的理论基础

27. **`24_machine_super_intelligence.ipynb`**——通用人工智能
    - **智能的形式化理论（Legg 与 Hutter）**
    - 心理测量学中的 g 因子与通用智能 Υ(π)
    - 用于序列预测的 Solomonoff 归纳
    - AIXI：理论最优的强化学习智能体
    - Monte Carlo AIXI（MC-AIXI）近似
    - Kolmogorov 复杂度估计
    - 跨环境的智能测量
    - 递归式自我改进动力学
    - 智能爆炸情景
    - **共 6 节：从心理测量学到超级智能**
    - 关联论文 23（MDL）、25（Kolmogorov）和 8（DQN）

28. **`01_complexity_dynamics.ipynb`**——复杂度与熵
    - 元胞自动机（规则 30）
    - 熵增长
    - 不可逆性的基础介绍

28. **`19_coffee_automaton.ipynb`**——咖啡自动机（深入研究）
    - **全面探索不可逆性**
    - 咖啡混合与扩散过程
    - 熵增长与粗粒化
    - 相空间与 Liouville 定理
    - Poincaré 回归定理：经过 e^N 的时间后，咖啡会重新分离
    - Maxwell 妖与 Landauer 原理
    - 计算不可逆性：单向函数与哈希
    - 机器学习中的信息瓶颈
    - 生物不可逆性：生命与热力学第二定律
    - 时间箭头：基本规律还是涌现现象
    - **通过 10 个完整章节探索不同尺度上的不可逆性**

29. **`26_cs231n_cnn_fundamentals.ipynb`**——CS231n：从第一性原理理解视觉
    - **用纯 NumPy 实现完整视觉流程**
    - k 近邻基线
    - 线性分类器（SVM 和 Softmax）
    - 优化：SGD、Momentum、Adam 与学习率调度
    - 带反向传播的两层神经网络
    - 卷积层：卷积、池化和 ReLU
    - 完整 CNN 架构（Mini-AlexNet）
    - 可视化技术：滤波器和显著性图
    - 迁移学习原理
    - 训练调试技巧：健全性检查、超参数调优和监控
    - **10 个章节覆盖完整 CS231n 课程**
    - 串联论文 7（AlexNet）、10（ResNet）与 11（空洞卷积）

## 仓库结构

```text
sutskever-30-implementations/
├── README.md                           # 英文说明
├── README.zh-CN.md                     # 中文学习译本
├── PROGRESS.md                         # 实现进度跟踪
├── IMPLEMENTATION_TRACKS.md            # 30 篇论文的详细实现路线
│
├── 01_complexity_dynamics.ipynb        # 熵与复杂度
├── 02_char_rnn_karpathy.ipynb          # 普通 RNN
├── 03_lstm_understanding.ipynb         # LSTM 门控
├── 04_rnn_regularization.ipynb         # RNN 的 Dropout
├── 05_neural_network_pruning.ipynb     # 剪枝与 MDL
├── 06_pointer_networks.ipynb           # 注意力指针
├── 07_alexnet_cnn.ipynb                # CNN 与 AlexNet
├── 08_seq2seq_for_sets.ipynb           # 置换不变集合
├── 09_gpipe.ipynb                      # 流水线并行
├── 10_resnet_deep_residual.ipynb       # 残差连接
├── 11_dilated_convolutions.ipynb       # 多尺度卷积
├── 12_graph_neural_networks.ipynb      # 消息传递 GNN
├── 13_attention_is_all_you_need.ipynb  # Transformer 架构
├── 14_bahdanau_attention.ipynb         # 原始注意力机制
├── 15_identity_mappings_resnet.ipynb   # 预激活 ResNet
├── 16_relational_reasoning.ipynb       # 关系网络
├── 17_variational_autoencoder.ipynb    # VAE
├── 18_relational_rnn.ipynb             # 关系型 RNN
├── 19_coffee_automaton.ipynb           # 深入研究不可逆性
├── 20_neural_turing_machine.ipynb      # 外部记忆
├── 21_ctc_speech.ipynb                 # CTC 损失
├── 22_scaling_laws.ipynb               # 经验缩放规律
├── 23_mdl_principle.ipynb              # MDL 与压缩
├── 24_machine_super_intelligence.ipynb # 通用 AI 与 AIXI
├── 25_kolmogorov_complexity.ipynb      # K(x) 与随机性
├── 26_cs231n_cnn_fundamentals.ipynb    # 从第一性原理理解视觉
├── 27_multi_token_prediction.ipynb     # 多词元预测
├── 28_dense_passage_retrieval.ipynb    # 稠密检索
├── 29_rag.ipynb                        # RAG 架构
└── 30_lost_in_middle.ipynb             # 长上下文分析
```

**全部 30 篇论文均已实现！（完成度 100%）🎉**

## 学习路线

### 初级路线（从这里开始）

1. **字符级 RNN**（`02_char_rnn_karpathy.ipynb`）——学习 RNN 基础
2. **LSTM**（`03_lstm_understanding.ipynb`）——理解门控机制
3. **CNN**（`07_alexnet_cnn.ipynb`）——计算机视觉基础
4. **ResNet**（`10_resnet_deep_residual.ipynb`）——跳跃连接
5. **VAE**（`17_variational_autoencoder.ipynb`）——生成模型

### 中级路线

6. **RNN 正则化**（`04_rnn_regularization.ipynb`）——改进训练
7. **Bahdanau 注意力**（`14_bahdanau_attention.ipynb`）——注意力基础
8. **指针网络**（`06_pointer_networks.ipynb`）——将注意力用作选择机制
9. **面向集合的 Seq2Seq**（`08_seq2seq_for_sets.ipynb`）——置换不变性
10. **CS231n**（`26_cs231n_cnn_fundamentals.ipynb`）——完整视觉流程（kNN → CNN）
11. **GPipe**（`09_gpipe.ipynb`）——大模型流水线并行
12. **Transformer**（`13_attention_is_all_you_need.ipynb`）——现代架构
13. **空洞卷积**（`11_dilated_convolutions.ipynb`）——感受野
14. **缩放定律**（`22_scaling_laws.ipynb`）——理解规模效应

### 高级路线

15. **预激活 ResNet**（`15_identity_mappings_resnet.ipynb`）——架构细节
16. **图神经网络**（`12_graph_neural_networks.ipynb`）——图学习
17. **关系网络**（`16_relational_reasoning.ipynb`）——关系推理
18. **神经图灵机**（`20_neural_turing_machine.ipynb`）——外部记忆
19. **CTC 损失**（`21_ctc_speech.ipynb`）——语音识别
20. **稠密检索**（`28_dense_passage_retrieval.ipynb`）——语义搜索
21. **RAG**（`29_rag.ipynb`）——检索增强生成
22. **中间信息丢失**（`30_lost_in_middle.ipynb`）——长上下文分析

### 理论与基础路线

23. **MDL 原理**（`23_mdl_principle.ipynb`）——通过压缩选择模型
24. **Kolmogorov 复杂度**（`25_kolmogorov_complexity.ipynb`）——随机性与信息
25. **复杂度动力学**（`01_complexity_dynamics.ipynb`）——熵与涌现
26. **咖啡自动机**（`19_coffee_automaton.ipynb`）——深入理解不可逆性

## Sutskever 30 的关键启示

### 架构演进

- **RNN → LSTM**：门控机制解决梯度消失问题
- **普通网络 → ResNet**：跳跃连接让更深的网络成为可能
- **RNN → Transformer**：注意力机制支持并行计算
- **固定词表 → 指针**：输出可以直接引用输入

### 基本机制

- **注意力**：可微分的选择机制
- **残差连接**：梯度的高速通道
- **门控**：通过学习控制信息流
- **外部记忆**：将存储与计算分离

### 训练经验

- **缩放定律**：性能随着规模以可预测的方式提升
- **正则化**：Dropout、权重衰减和数据增强
- **优化**：梯度裁剪与学习率调度
- **计算最优**：平衡模型大小与训练数据量

### 理论基础

- **信息论**：压缩、熵与 MDL
- **复杂度**：Kolmogorov 复杂度与幂律
- **生成建模**：VAE、ELBO 与潜在空间
- **记忆**：可微数据结构

## 实现理念

### 为什么只使用 NumPy？

这些实现刻意不使用 PyTorch 或 TensorFlow，目的是：

- **加深理解**：看清框架替你隐藏了什么
- **教学清晰**：没有魔法，每个运算都明确可见
- **聚焦核心概念**：关注算法，而不是框架 API
- **知识可迁移**：这些原理适用于任何框架

### 合成数据方法

每个 Notebook 都会生成自己的数据，以便：

- **立即执行**：无需下载数据集
- **受控实验**：在简单场景中理解模型行为
- **聚焦概念**：避免数据掩盖算法本身
- **快速迭代**：可以立即修改并重新运行

## 扩展与后续步骤

### 在这些实现上继续探索

理解核心概念后，可以尝试：

1. **扩大规模**：使用 PyTorch 或 JAX，在真实数据集上实现
2. **组合技术**：例如 ResNet 加注意力机制
3. **现代变体**：
   - RNN → GRU → Transformer
   - VAE → β-VAE → VQ-VAE
   - ResNet → ResNeXt → EfficientNet
4. **实际应用**：将这些方法用于真实问题

### 研究方向

Sutskever 30 指向以下方向：

- 规模：更大的模型、更多的数据
- 效率：稀疏模型、量化
- 能力：推理、多模态
- 理解：可解释性与理论

## 资源

### 原始论文

完整引用和链接参见 `IMPLEMENTATION_TRACKS.md`。

### 延伸阅读

- [Ilya Sutskever 阅读清单（GitHub）](https://github.com/dzyim/ilya-sutskever-recommended-reading)
- [Aman's AI Journal——Sutskever 30 导读](https://aman.ai/primers/ai/top-30-papers/)
- [带注释的 Transformer](http://nlp.seas.harvard.edu/annotated-transformer/)
- [Andrej Karpathy 的博客](http://karpathy.github.io/)

### 课程

- Stanford CS231n：卷积神经网络
- Stanford CS224n：使用深度学习处理自然语言
- MIT 6.S191：深度学习导论

## 贡献

这些实现以教学为目的，仍有改进空间，可以考虑：

- 添加更多可视化
- 实现缺失的论文
- 改进讲解
- 查找错误
- 添加与框架实现的对比

## 引用

如果在工作或教学中使用这些实现，请引用：

```bibtex
@misc{sutskever30implementations,
  title={Sutskever 30: Complete Implementation Suite},
  author={Paul "The Pageman" Pajo, pageman@gmail.com},
  year={2025},
  note={Educational implementations of Ilya Sutskever's recommended reading list, inspired by https://papercode.vercel.app/}
}
```

## 许可说明

英文原文写明：“Educational use. See individual papers for original research citations.”（用于教育用途；原始研究引用请参见各篇论文。）

原仓库当前没有提供标准 `LICENSE` 文件，因此这句话不能替代明确的软件许可证。本中文版本仅作为个人学习译本，不主张获得额外的复制、修改、再许可或商业使用权。

## 致谢

- **Ilya Sutskever**：整理这份重要的阅读清单
- **论文作者**：完成这些奠基性研究
- **社区**：让这些思想更容易被大众理解

---

## 最近新增内容（2025 年 12 月）

### 最近实现的 21 篇论文

- ✅ **论文 4**：RNN 正则化（变分 Dropout）
- ✅ **论文 5**：神经网络剪枝（MDL，90% 以上稀疏度）
- ✅ **论文 7**：AlexNet（从零实现 CNN）
- ✅ **论文 8**：面向集合的 Seq2Seq（置换不变性、注意力池化）
- ✅ **论文 9**：GPipe（流水线并行、微批次、重计算）
- ✅ **论文 19**：咖啡自动机（深入研究不可逆性、熵和 Landauer 原理）
- ✅ **论文 26**：CS231n（从 kNN 到 CNN 的完整视觉流程，全部使用 NumPy）
- ✅ **论文 11**：空洞卷积（多尺度）
- ✅ **论文 12**：图神经网络（消息传递）
- ✅ **论文 14**：Bahdanau 注意力（原始注意力机制）
- ✅ **论文 15**：ResNet 恒等映射（预激活）
- ✅ **论文 16**：关系推理（关系网络）
- ✅ **论文 18**：关系型 RNN（关系记忆，以及第 11 节约 1100 行手动反向传播）
- ✅ **论文 21**：Deep Speech 2（CTC 损失）
- ✅ **论文 23**：MDL 原理（压缩、模型选择，关联论文 5 与 25）
- ✅ **论文 24**：机器超级智能（通用 AI、AIXI、Solomonoff 归纳、智能度量、递归式自我改进）
- ✅ **论文 25**：Kolmogorov 复杂度（随机性、算法概率、理论基础）
- ✅ **论文 27**：多词元预测（样本效率提升 2～3 倍）
- ✅ **论文 28**：稠密段落检索（双编码器）
- ✅ **论文 29**：RAG（检索增强生成）
- ✅ **论文 30**：中间信息丢失（长上下文）

## 实现复杂度速查

### 一个下午可以完成

- ✅ 字符级 RNN
- ✅ LSTM
- ✅ ResNet
- ✅ 简单 VAE
- ✅ 空洞卷积

### 周末项目

- ✅ Transformer
- ✅ 指针网络
- ✅ 图神经网络
- ✅ 关系网络
- ✅ 神经图灵机
- ✅ CTC 损失
- ✅ 稠密检索

### 一周深入研究

- ✅ 完整 RAG 系统
- ⚠️ 大规模实验
- ⚠️ 超参数优化

---

**“如果你真正学会了这些内容，就会掌握当今 90% 真正重要的知识。”**——Ilya Sutskever

学习愉快！🚀
