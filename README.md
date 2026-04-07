# Daily arXiv Digest - Text-to-Audio, Text-to-Speech & Generative Model

> 🤖 每日 arXiv 论文自动摘要 - Text-to-Audio, Text-to-Speech & Generative Model

[![Last Updated](https://img.shields.io/github/last-commit/junxi25liu/daily-arxiv-digest)](https://github.com/junxi25liu/daily-arxiv-digest/commits/main)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📅 最新论文推荐

### 2026-04-07 (5 篇)

#### 1️⃣ AffectSpeech: A Large-Scale Emotional Speech Dataset with Fine-Grained Textual Descriptions

**arXiv**: [2604.04160](https://arxiv.org/abs/2604.04160)  
**作者**: Tianhua Qi, Wenming Zheng, Björn W. Schuller, Zhaojie Luo, Haizhou Li  
**机构**: Academic (Haizhou Li 为知名语音学者)  
**分类**: eess.AS, cs.SD, eess.SP

> **一句话总结**: 提出 AffectSpeech 大规模情感语音数据集，采用六维度细粒度文本描述标注体系和人 -LLM 协作标注流程，支持语音情感描述生成和情感语音合成任务。

**核心创新**:
- ✅ 六维度情感标注体系 (极性、描述、强度、韵律、片段、语义)
- ✅ 人 -LLM 协作标注流程，平衡质量与可扩展性
- ✅ 多样化描述风格，减少下游建模风格偏差
- ✅ 大规模高质量语料，填补情感语音数据集空白

**[详细摘要 →](daily-digests/2026-04-07-daily-digest.md#1-affectspeech-a-large-scale-emotional-speech-dataset-with-fine-grained-textual-descriptions-for-speech-emotion-captioning-and-synthesis)**

---

#### 2️⃣ DynFOA: Generating First-Order Ambisonics with Conditional Diffusion for 360-Degree Videos

**arXiv**: [2604.02781](https://arxiv.org/abs/2604.02781)  
**作者**: Ziyu Luo, Lin Chen, Qiang Qu, Xiaoming Chen, Yiran Shen  
**机构**: Academic  
**分类**: cs.SD

> **一句话总结**: 提出 DynFOA 框架，结合动态场景重建与条件扩散模型，为动态和声学复杂的 360 度视频自动生成一阶 Ambisonics (FOA) 空间音频。

**核心创新**:
- ✅ 首次使用扩散模型为 360 度视频生成 FOA 空间音频
- ✅ 3D Gaussian Splatting 场景重建，提供物理基础特征
- ✅ 动态场景处理，支持声源位置和环境变化
- ✅ 多条件扩散生成，视觉 + 深度 + 运动 + 几何融合

**[详细摘要 →](daily-digests/2026-04-07-daily-digest.md#2-dynfoa-generating-first-order-ambisonics-with-conditional-diffusion-for-dynamic-and-acoustically-complex-360-degree-videos)**

---

#### 3️⃣ Speaker-Reasoner: Scaling Interaction Turns for Timestamped Speaker-Attributed ASR

**arXiv**: [2604.03074](https://arxiv.org/abs/2604.03074)  
**作者**: Zhennan Lin, Shuai Wang, Zhaokai Sun, Pengyuan Xie, Chuan Xie, Jie Liu, Qiang Zhang, Lei Xie  
**机构**: Academic (Lei Xie 为西工大知名语音学者)  
**分类**: eess.AS, cs.CL, cs.SD

> **一句话总结**: 提出 Speaker-Reasoner，具有代理式多轮时序推理能力的端到端语音大语言模型，实现说话人归属 ASR。

**核心创新**:
- ✅ 代理式多轮时序推理，迭代分析音频结构
- ✅ 联合建模说话人身份、性别、时间戳和转录
- ✅ 说话人感知缓存，支持长音频处理
- ✅ 三阶段渐进训练策略

**[详细摘要 →](daily-digests/2026-04-07-daily-digest.md#3-speaker-reasoner-scaling-interaction-turns-and-reasoning-patterns-for-timestamped-speaker-attributed-asr)**

---

#### 4️⃣ Unmixing the Crowd: Enrollment-Free Target Speech Extraction

**arXiv**: [2604.03219](https://arxiv.org/abs/2604.03219)  
**作者**: FNU Sidharth, Meysam Asgari, Hao-Wen Dong, Dhruv Jain  
**机构**: Industry Lab  
**分类**: eess.AS, cs.SD

> **一句话总结**: 提出无需注册的目标语音提取方法，直接从混合音频中预测每个说话人的嵌入向量，消除对干净注册音频的依赖。

**核心创新**:
- ✅ 无需注册的语音提取，从混合音频预测说话人嵌入
- ✅ Mixture-to-Set 映射，输出候选说话人嵌入集
- ✅ 排列不变教师监督，对齐到单人嵌入空间
- ✅ 结构化嵌入空间，优于 WavLM+K-means

**[详细摘要 →](daily-digests/2026-04-07-daily-digest.md#4-unmixing-the-crowd-learning-mixture-to-set-speaker-embeddings-for-enrollment-free-target-speech-extraction)**

---

#### 5️⃣ Split and Conquer Partial Deepfake Speech

**arXiv**: [2604.02913](https://arxiv.org/abs/2604.02913)  
**作者**: Inbal Rimon, Oren Gal, Haim Permuter  
**机构**: Academic  
**分类**: cs.SD, cs.AI, cs.LG

> **一句话总结**: 提出分而治之的局部深度伪造语音检测框架，将问题分解为边界检测和片段级分类两阶段，在 PartialSpoof 基准上取得最先进性能。

**核心创新**:
- ✅ 两阶段分解：边界检测 + 片段级分类
- ✅ 边界检测器识别时间转换点
- ✅ 反射式多长度训练，提升鲁棒性
- ✅ 多配置融合，互补预测

**[详细摘要 →](daily-digests/2026-04-07-daily-digest.md#5-split-and-conquer-partial-deepfake-speech)**

---

### 2026-04-06 (5 篇，保留最近 10 篇)

#### 6️⃣ Woosh: A Sound Effects Foundation Model

**arXiv**: [2604.01929](https://arxiv.org/abs/2604.01929)  
**作者**: Gaëtan Hadjeres, Marc Ferras, Khaled Koutini, et al.  
**机构**: Sony AI  
**分类**: cs.SD, cs.AI, cs.LG

> **一句话总结**: Sony AI 开源的音效基础模型 Woosh，提供完整的音频编码器/解码器、文本 - 音频对齐、文本生成音频和视频生成音频模型套件，性能媲美或超越 StableAudio-Open 和 TangoFlux。

**核心创新**:
- ✅ 完整开源的音效基础模型 (T2A + V2A)
- ✅ 蒸馏模型支持低资源快速推理
- ✅ 性能媲美或超越 StableAudio-Open 和 TangoFlux
- ✅ 公开演示页面和代码

**[详细摘要 →](daily-digests/2026-04-06-daily-digest.md#1-woosh-a-sound-effects-foundation-model)**

---

#### 7️⃣ GAP-URGENet: A Generative-Predictive Fusion Framework for Universal Speech Enhancement

**arXiv**: [2604.01832](https://arxiv.org/abs/2604.01832)  
**作者**: Xiaobin Rong, Yushi Wang, Zheng Wang, Jing Lu  
**机构**: ICASSP 2026 URGENT Challenge  
**分类**: eess.AS, cs.SD

> **一句话总结**: 提出生成 - 预测融合框架 GAP-URGENet，结合自监督表示域的全栈语音修复和频谱图域增强，在 ICASSP 2026 URGENT Challenge 中取得目标评估第 1 名。

**核心创新**:
- ✅ 生成 - 预测双分支架构，互补增强
- ✅ 神经声码器重建，保持高质量语音
- ✅ 后处理融合模块，带宽扩展至 48kHz
- ✅ ICASSP 2026 URGENT Challenge 目标评估第 1 名

**[详细摘要 →](daily-digests/2026-04-06-daily-digest.md#2-gap-urgenet-a-generative-predictive-fusion-framework-for-universal-speech-enhancement)**

---

#### 8️⃣ FastTurn: Unifying Acoustic and Streaming Semantic Cues for Low-Latency Turn Detection

**arXiv**: [2604.01897](https://arxiv.org/abs/2604.01897)  
**作者**: Chengyou Wang, Hongfei Xue, Chunjiang He, et al.  
**机构**: Industry Lab  
**分类**: cs.SD

> **一句话总结**: 统一流式 CTC 解码与声学特征的轮次检测框架，实现低延迟高准确率的全双工对话交互，发布真实对话测试集。

**核心创新**:
- ✅ 流式 CTC+ 声学特征，早期决策保持语义
- ✅ 真实对话测试集，包含重叠语音、回应等
- ✅ 低延迟高准确率，鲁棒性强
- ✅ 适用于 AudioLLM 全双工对话系统

**[详细摘要 →](daily-digests/2026-04-06-daily-digest.md#3-fastturn-unifying-acoustic-and-streaming-semantic-cues-for-low-latency-turn-detection)**

---

#### 9️⃣ DynFOA: Generating First-Order Ambisonics with Conditional Diffusion

**arXiv**: [2604.02781](https://arxiv.org/abs/2604.02781)  
**作者**: Ziyu Luo, Lin Chen, Qiang Qu, et al.  
**机构**: Academic  
**分类**: cs.SD

> **一句话总结**: 使用条件扩散模型为动态和声学复杂的 360 度视频自动生成一阶 Ambisonics (FOA) 空间音频，解决 360 度视频录制中空间音频捕获困难的问题。

**核心创新**:
- ✅ 首次使用扩散模型为 360 度视频生成 FOA 空间音频
- ✅ 动态场景处理，支持声源位置和环境变化
- ✅ 视觉 - 音频条件融合，多模态信息作为条件
- ✅ 显式建模房间冲击响应和混响效果

**[详细摘要 →](daily-digests/2026-04-06-daily-digest.md#4-dynfoa-generating-first-order-ambisonics-with-conditional-diffusion)**

---

#### 🔟 FineLAP: Taming Heterogeneous Supervision for Fine-grained Language-Audio Pretraining

**arXiv**: [2604.01155](https://arxiv.org/abs/2604.01155)  
**作者**: Xiquan Li, Xuenan Xu, Ziyang Ma, et al.  
**机构**: Academic  
**分类**: cs.SD

> **一句话总结**: 提出 FineLAP 框架，有效利用不同粒度的音频 - 文本数据 (从 clip 级到 frame 级) 进行对比预训练，解决现有音频 - 语言模型在帧级任务上表现不佳的问题。

**核心创新**:
- ✅ 异构监督统一框架，同时利用多粒度数据
- ✅ 细粒度对齐，多粒度对比学习
- ✅ 无需额外标注，利用隐含粒度信息
- ✅ 帧级任务显著提升，音频字幕和声音事件检测

**[详细摘要 →](daily-digests/2026-04-06-daily-digest.md#5-finelap-taming-heterogeneous-supervision-for-fine-grained-language-audio-pretraining)**

---

## 📊 统计信息

| 指标 | 数值 |
|------|------|
| 总推荐论文 | 10 篇 (保留最近) |
| 今日新增 | 5 篇 |
| 搜索范围 | cs.SD, cs.CL, cs.AI, cs.LG, eess.AS |
| 时间范围 | 过去 48 小时 |
| 最近更新 | 2026-04-07 |

---

## 📁 历史摘要

- [2026-04-07](daily-digests/2026-04-07-daily-digest.md) - 5 篇
- [2026-04-06](daily-digests/2026-04-06-daily-digest.md) - 5 篇
- [2026-04-05](daily-digests/2026-04-05-daily-digest.md) - 5 篇
- [2026-04-04](daily-digests/arxiv-digest-2026-04-04.md) - 4 篇
- [2026-04-03](daily-digests/arxiv-digest-2026-04-03.md) - 5 篇
- [2026-04-02](daily-digests/arxiv-digest-2026-04-02.md) - 3 篇
- [2026-04-01](daily-digests/arxiv-digest-2026-04-01.md) - 3 篇
- [2026-03-31](daily-digests/arxiv-digest-2026-03-31.md) - 3 篇

---

## 🔗 相关链接

- [arXiv](https://arxiv.org/)
- [arXiv 今日论文](https://arxiv.org/list/recent)
- [GitHub 仓库](https://github.com/junxi25liu/daily-arxiv-digest)

---

**自动生成**: Daily arXiv Digest Skill v1.1.0  
**专注领域**: Text-to-Speech, Text-to-Audio, Generative Models, Speech Processing  
**更新频率**: 每日早上 8:00 (Asia/Shanghai)
