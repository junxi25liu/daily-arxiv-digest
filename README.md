# Daily arXiv Digest - Text-to-Audio, Text-to-Speech & Generative Model

> 🤖 每日 arXiv 论文自动摘要 - Text-to-Audio, Text-to-Speech & Generative Model

[![Last Updated](https://img.shields.io/github/last-commit/junxi25liu/daily-arxiv-digest)](https://github.com/junxi25liu/daily-arxiv-digest/commits/main)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📅 最新论文推荐

### 2026-04-10 (3 篇)

#### 1️⃣ Anchored Cyclic Generation: A Novel Paradigm for Long-Sequence Symbolic Music Generation

**arXiv**: [2604.05343](https://arxiv.org/abs/2604.05343)  
**作者**: Haoyu Gu, et al.  
**机构**: Academic  
**分类**: cs.SD, cs.AI  
**会议**: ACL 2026 Findings

> **一句话总结**: 提出 Anchored Cyclic Generation (ACG) 新范式，通过锚定特征引导自回归生成过程，有效缓解长序列符号音乐生成中的误差累积问题，在长序列音乐生成任务中显著优于现有主流方法。

**核心创新**:
- ✅ ACG 范式：利用已识别音乐的锚定特征在自回归过程中引导后续生成，缓解误差累积
- ✅ Hi-ACG 框架：分层锚定循环生成框架，采用全局到局部生成策略
- ✅ 钢琴 Token 设计：高效音乐表示 token，与 Hi-ACG 框架高度兼容
- ✅ 性能提升：预测特征向量与真实语义向量余弦距离平均减少 34.7%

**[详细摘要 →](../daily-digests/2026-04-10-daily-digest.md#📄-paper-1-anchored-cyclic-generation-a-novel-paradigm-for-long-sequence-symbolic-music-generation)**

---

#### 2️⃣ Active Noise Cancellation on Open-Ear Smart Glasses

**arXiv**: [2604.05519](https://arxiv.org/abs/2604.05519)  
**作者**: Kuang Yuan, et al.  
**机构**: Academic  
**分类**: eess.AS, cs.HC, cs.LG, cs.SD, eess.SP

> **一句话总结**: 提出首个用于开放式智能眼镜的实时主动降噪 (ANC) 系统，仅使用眼镜框架上的麦克风和微型开放式扬声器，无需耳道内误差麦克风即可实现环境噪声抑制。

**核心创新**:
- ✅ 开放式 ANC 首创：首个专为开放式智能眼镜设计的实时 ANC 系统
- ✅ 8 麦克风阵列：利用分布在眼镜框架周围的麦克风阵列估计耳部噪声
- ✅ 低延迟管道：实时生成反噪声信号，在 100-1000 Hz 频段有效降噪
- ✅ 降噪效果：无校准 9.6 dB，有校准 11.2 dB 平均降噪

**[详细摘要 →](../daily-digests/2026-04-10-daily-digest.md#📄-paper-2-active-noise-cancellation-on-open-ear-smart-glasses)**

---

#### 3️⃣ Generalizable Audio-Visual Navigation via Binaural Difference Attention and Action Transition Prediction

**arXiv**: [2604.05007](https://arxiv.org/abs/2604.05007)  
**作者**: Yinfeng Yu, et al.  
**机构**: Academic  
**分类**: cs.SD, cs.AI, eess.AS  
**会议**: IJCNN 2026

> **一句话总结**: 提出 BDATP 框架，通过双耳差异注意力模块和动作转移预测任务，提升音频 - 视觉导航在未见环境中的泛化能力，在 Replica 数据集上对未听过声音的成功率提升达 21.6 个百分点。

**核心创新**:
- ✅ 双耳差异注意力 (BDA)：显式建模双耳差异增强空间定位，减少语义依赖
- ✅ 动作转移预测 (ATP)：辅助任务作为正则化项，减轻环境特定过拟合
- ✅ 联合优化：同时优化感知和策略模块，实现端到端音频 - 视觉导航
- ✅ 强泛化能力：在 Replica 数据集上对未听过声音成功率提升 21.6 个百分点

**[详细摘要 →](../daily-digests/2026-04-10-daily-digest.md#📄-paper-3-generalizable-audio-visual-navigation-via-binaural-difference-attention-and-action-transition-prediction)**

---

### 2026-04-09 (5 篇)

#### 1️⃣ AudioKV: KV Cache Eviction in Efficient Large Audio Language Models

**arXiv**: [2604.06694](https://arxiv.org/abs/2604.06694)  
**作者**: Yuxuan Wang, Peize He, Xiyan Gui, Xiaoqian Liu, Junhao He, Xuyang Liu, Zichen Wen, Xuming Hu, Linfeng Zhang  
**机构**: Academic  
**分类**: cs.SD

> **一句话总结**: 提出 AudioKV 框架，通过硬件友好的语义 - 声学对齐机制优先处理音频关键的注意力头，在大型音频语言模型（LALM）中实现高效的 KV 缓存压缩，在 40% 压缩率下仅损失 0.45% 的准确率。

**核心创新**:
- ✅ 模态专用头识别：通过分析 ASR 任务中的注意力分数，识别音频关键的注意力头
- ✅ 动态 KV 缓存预算分配：优先为模态专用头分配 KV 缓存预算
- ✅ 频谱分数平滑（SSS）：基于 FFT 的全局滤波策略，抑制高频噪声并恢复重要性分数的平滑全局趋势
- ✅ 硬件友好设计：整个框架设计考虑硬件效率，便于实际部署

**[详细摘要 →](../daily-digests/2026-04-09-daily-digest.md#📄-paper-1-audiokv-kv-cache-eviction-in-efficient-large-audio-language-models)**

---

#### 2️⃣ A Novel Automatic Framework for Speaker Drift Detection in Synthesized Speech

**arXiv**: [2604.06327](https://arxiv.org/abs/2604.06327)  
**作者**: Jia-Hong Huang, Seulgi Kim, Yi Chieh Liu, Yixian Shen, Hongyi Zhu, Prayag Tiwari, Stevan Rudinac, Evangelos Kanoulas  
**机构**: Academic (ICASSP 2026)  
**分类**: cs.SD, cs.AI

> **一句话总结**: 提出首个自动检测合成语音中"说话人漂移"现象的框架，通过计算重叠片段的余弦相似度并结合 LLM 推理，将说话人一致性评估形式化为二分类任务。

**核心创新**:
- ✅ 说话人漂移问题定义：首次将扩散式 TTS 模型中说话人身份在单个话语内逐渐漂移的现象作为独立研究问题
- ✅ 余弦相似度检测：基于说话人嵌入在单位球面上的几何聚类特性，计算重叠片段的余弦相似度
- ✅ LLM 推理管道：将嵌入表示结构化后输入 LLM 进行漂移评估，桥接几何信号分析与感知推理
- ✅ 理论保证：为基于余弦的漂移检测提供理论保证

**[详细摘要 →](../daily-digests/2026-04-09-daily-digest.md#📄-paper-2-a-novel-automatic-framework-for-speaker-drift-detection-in-synthesized-speech)**

---

#### 3️⃣ Generating Synthetic Doctor-Patient Conversations for Long-form Audio Summarization

**arXiv**: [2604.06138](https://arxiv.org/abs/2604.06138)  
**作者**: Yanis Labrak, David Grünert, Séverin Baroudi, Jiyun Chun, Pawel Cyrta, Sergio Burdisso, Ahmed Hassoon, David Liu, Andrew Perrault, Ricard Marxer, Thomas Schaaf  
**机构**: Academic (Interspeech 2026)  
**分类**: cs.SD, cs.AI

> **一句话总结**: 提出合成数据生成管道，生成 8800 个医生 - 患者对话（1300 小时音频）用于长上下文音频推理训练和评估，发现级联方法仍显著优于端到端模型。

**核心创新**:
- ✅ 三阶段合成管道：角色驱动对话生成 + 多说话人音频合成 + 基于 LLM 的 SOAP 笔记生成
- ✅ 大规模数据集：发布 8800 个合成对话，对应 1300 小时音频和参考笔记
- ✅ 开放权重模型：整个管道完全基于开放权重模型构建
- ✅ 长上下文评估：为长上下文音频推理提供受控评估环境

**[详细摘要 →](../daily-digests/2026-04-09-daily-digest.md#📄-paper-3-generating-synthetic-doctor-patient-conversations-for-long-form-audio-summarization)**

---

#### 4️⃣ Brain-to-Speech: Prosody Feature Engineering and Transformer-Based Reconstruction

**arXiv**: [2604.05751](https://arxiv.org/abs/2604.05751)  
**作者**: Mohammed Salah Al-Radhi, Géza Németh, Andon Tchechmedjiev, Binbin Xu  
**机构**: Academic  
**分类**: eess.SP, cs.LG, cs.SD

> **一句话总结**: 提出从颅内脑电图（iEEG）信号进行脑到语音合成的新方法，通过韵律特征工程和 Transformer 编码器架构实现高保真语音重建。

**核心创新**:
- ✅ 韵律特征提取：从复杂脑 iEEG 信号中提取关键韵律特征（语调、音高、节奏）
- ✅ 专用 Transformer 架构：设计专门用于脑到语音任务的 Transformer 编码器
- ✅ 韵律特征整合：将提取的韵律特征整合到模型中，显著提升语音重建的自然度和表现力
- ✅ 多指标评估：在定量和感知指标上均优于传统基线方法

**[详细摘要 →](../daily-digests/2026-04-09-daily-digest.md#📄-paper-4-brain-to-speech-prosody-feature-engineering-and-transformer-based-reconstruction)**

---

#### 5️⃣ Time-Domain Voice Identity Morphing (TD-VIM): A Signal-Level Approach to Morphing Attacks

**arXiv**: [2604.05683](https://arxiv.org/abs/2604.05683)  
**作者**: Aravinda Reddy PN, Raghavendra Ramachandra, K. Sreenivasa Rao, Pabitra Mitra, Kunal Singh  
**机构**: Academic  
**分类**: cs.SD

> **一句话总结**: 提出时域语音身份变形（TD-VIM）方法，在信号级别混合两个不同身份的语音特征，生成的变形样本在说话人验证系统上达到 99.40-99.74% 的攻击成功率。

**核心创新**:
- ✅ 信号级变形：首次提出在时域信号级别进行语音身份变形的方法
- ✅ 双身份混合：能够混合两个不同身份的语音特征，生成可同时匹配两个身份的样本
- ✅ 多因子评估：基于不同变形因子创建四种变形信号，进行全面评估
- ✅ 高攻击成功率：在多个说话人验证系统上达到极高的攻击成功率

**[详细摘要 →](../daily-digests/2026-04-09-daily-digest.md#📄-paper-5-time-domain-voice-identity-morphing-td-vim-a-signal-level-approach-to-morphing-attacks-on-speaker-verification-systems)**

---

### 2026-04-08 (5 篇)

#### 1️⃣ Brain-to-Speech: Prosody Feature Engineering and Transformer-Based Reconstruction

**arXiv**: [2604.05751](https://arxiv.org/abs/2604.05751)  
**作者**: Mohammed Salah Al-Radhi, Géza Németh, Andon Tchechmedjiev, Binbin Xu  
**机构**: Academic  
**分类**: eess.SP, cs.LG, cs.SD

> **一句话总结**: 提出基于颅内脑电图 (iEEG) 的脑 - 语音合成新方法，通过韵律特征工程和专用 Transformer 编码器实现高保真语音重建，为言语障碍患者的神经假体技术开辟新方向。

**核心创新**:
- ✅ 韵律特征提取管道：从 iEEG 信号提取音调、音高、节奏等关键韵律特征
- ✅ 专用 Transformer 编码器：针对脑 - 语音任务设计，整合韵律特征增强重建
- ✅ 多模态融合：整合神经科学、AI 和信号处理技术解码脑活动生成语音
- ✅ 优越性能：在定量和感知指标上均优于传统 Griffin-Lim 和 CNN 基线方法

**[详细摘要 →](../daily-digests/2026-04-08-daily-digest.md#论文-1-brain-to-speech-prosody-feature-engineering-and-transformer-based-reconstruction)**

---

#### 2️⃣ Time-Domain Voice Identity Morphing (TD-VIM): A Signal-Level Approach to Morphing Attacks

**arXiv**: [2604.05683](https://arxiv.org/abs/2604.05683)  
**作者**: Aravinda Reddy PN, Raghavendra Ramachandra, K. Sreenivasa Rao, Pabitra Mitra, Kunal Singh  
**机构**: Academic  
**分类**: cs.SD

> **一句话总结**: 提出时域语音身份混合 (TD-VIM) 方法，在信号层面混合两个不同身份的语音特征，生成能欺骗多个说话人验证系统的混合样本，揭示语音生物识别系统的安全风险。

**核心创新**:
- ✅ 信号层面语音混合：首次提出语音领域的信号级混合攻击方法
- ✅ TD-VIM 框架：在时域直接混合两个身份的语音特征
- ✅ 高攻击成功率：G-MAP 值达 99.40% (iPhone-11) 和 99.74% (Samsung S8)
- ✅ 全面评估：在两个深度学习 SVS 和一个商用系统 (Verispeak) 上验证

**[详细摘要 →](../daily-digests/2026-04-08-daily-digest.md#论文-2-time-domain-voice-identity-morphing-td-vim-a-signal-level-approach-to-morphing-attacks-on-speaker-verification-systems)**

---

#### 3️⃣ AI-Driven Modular Services for Accessible Multilingual Education in Immersive XR Settings

**arXiv**: [2604.05591](https://arxiv.org/abs/2604.05591)  
**作者**: N. D. Tantaroudas, A. J. McCracken, I. Karachalios, E. Papatheou  
**机构**: Academic  
**分类**: cs.CE, cs.AI, cs.CL, cs.CY, cs.ET

> **一句话总结**: 提出模块化 AI 服务平台，集成 Whisper 语音识别、NLLB 翻译、AWS Polly 语音合成、RoBERTa 情感分类、Flan-T5 对话摘要和 MediaPipe 手语渲染，在 VR 环境中实现无障碍多语言教育。

**核心创新**:
- ✅ 六模块 AI 服务集成：语音识别 + 翻译 + 语音合成 + 情感分类 + 对话摘要 + 手语渲染
- ✅ 3D 虚拟人手语：基于 MediaPipe 手部地标坐标生成 VR 环境中的国际手语动画
- ✅ 实时 XR 部署：技术评估确认平台适合实时扩展现实部署
- ✅ 模块化设计：支持独立扩展和适应不同教育场景

**[详细摘要 →](../daily-digests/2026-04-08-daily-digest.md#论文-3-ai-driven-modular-services-for-accessible-multilingual-education-in-immersive-extended-reality-settings)**

---

#### 4️⃣ FastDiSS: Few-step Match Many-step Diffusion Language Model on Sequence-to-Sequence Generation

**arXiv**: [2604.05551](https://arxiv.org/abs/2604.05551)  
**作者**: Dat Nguyen-Cong, Tung Kieu, Hoang Thanh-Tung  
**机构**: Academic  
**分类**: cs.CL, cs.AI, cs.LG

> **一句话总结**: 提出 FastDiSS 训练框架，通过扰动自条件信号匹配推理噪声和 token 级噪声感知机制，解决少步采样中自条件不准确问题，实现高达 400 倍推理加速。

**核心创新**:
- ✅ 自条件扰动训练：扰动自条件信号匹配推理噪声，提升鲁棒性
- ✅ Token 级噪声感知：防止训练饱和，优化效果提升
- ✅ 400 倍加速：相比标准连续扩散模型推理速度提升高达 400 倍
- ✅ 竞争力强：与其他单步扩散框架相比保持竞争力

**[详细摘要 →](../daily-digests/2026-04-08-daily-digest.md#论文-4-fastdiss-few-step-match-many-step-diffusion-language-model-on-sequence-to-sequence-generation-full-version)**

---

#### 5️⃣ Controllable Singing Style Conversion with Boundary-Aware Information Bottleneck

**arXiv**: [2604.05526](https://arxiv.org/abs/2604.05526)  
**作者**: Zhetao Hu, Yiquan Zhou, Wenyu Wang, Zhiyu Wu, Xin Gao, Jihua Zhu  
**机构**: Academic (SVCC2025 S4 团队)  
**分类**: cs.SD, cs.AI

> **一句话总结**: S4 团队提交 SVCC2025 的歌声风格转换系统，通过边界感知 Whisper 瓶颈、帧级技巧矩阵和高频带完成策略，在官方评估中取得最佳自然度性能。

**核心创新**:
- ✅ 边界感知 Whisper 瓶颈：池化音素跨度表示，抑制残留源风格保留语言内容
- ✅ 帧级技巧矩阵：显式帧级技巧矩阵 + 推理时 F0 处理，实现稳定动态风格渲染
- ✅ 高频带完成策略：利用辅助 48kHz SVC 模型增强高频谱，克服数据稀缺
- ✅ SVCC2025 最佳自然度：官方主观评估中取得最佳自然度性能

**[详细摘要 →](../daily-digests/2026-04-08-daily-digest.md#论文-5-controllable-singing-style-conversion-with-boundary-aware-information-bottleneck)**

---

### 2026-04-07 (5 篇，保留最近 10 篇)

#### 6️⃣ AffectSpeech: A Large-Scale Emotional Speech Dataset with Fine-Grained Textual Descriptions

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

**[详细摘要 →](../daily-digests/2026-04-07-daily-digest.md#论文-1-affectspeech-a-large-scale-emotional-speech-dataset-with-fine-grained-textual-descriptions-for-speech-emotion-captioning-and-synthesis)**

---

#### 7️⃣ DynFOA: Generating First-Order Ambisonics with Conditional Diffusion for 360-Degree Videos

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

**[详细摘要 →](../daily-digests/2026-04-07-daily-digest.md#论文-2-dynfoa-generating-first-order-ambisonics-with-conditional-diffusion-for-dynamic-and-acoustically-complex-360-degree-videos)**

---

#### 8️⃣ Speaker-Reasoner: Scaling Interaction Turns for Timestamped Speaker-Attributed ASR

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

**[详细摘要 →](../daily-digests/2026-04-07-daily-digest.md#论文-3-speaker-reasoner-scaling-interaction-turns-and-reasoning-patterns-for-timestamped-speaker-attributed-asr)**

---

#### 9️⃣ Unmixing the Crowd: Enrollment-Free Target Speech Extraction

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

**[详细摘要 →](../daily-digests/2026-04-07-daily-digest.md#论文-4-unmixing-the-crowd-learning-mixture-to-set-speaker-embeddings-for-enrollment-free-target-speech-extraction)**

---

#### 🔟 Split and Conquer Partial Deepfake Speech

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

**[详细摘要 →](../daily-digests/2026-04-07-daily-digest.md#论文-5-split-and-conquer-partial-deepfake-speech)**

---

## 📊 统计信息

| 指标 | 数值 |
|------|------|
| 总推荐论文 | 13 篇 (保留最近 10 天) |
| 今日新增 | 3 篇 |
| 搜索范围 | cs.SD, cs.CL, cs.AI, cs.LG, eess.AS |
| 时间范围 | 过去 48 小时 |
| 最近更新 | 2026-04-10 |

---

## 📁 历史摘要

- [2026-04-10](../daily-digests/2026-04-10-daily-digest.md) - 3 篇
- [2026-04-09](../daily-digests/2026-04-09-daily-digest.md) - 5 篇
- [2026-04-08](../daily-digests/2026-04-08-daily-digest.md) - 5 篇
- [2026-04-07](../daily-digests/2026-04-07-daily-digest.md) - 5 篇
- [2026-04-06](../daily-digests/2026-04-06-daily-digest.md) - 5 篇
- [2026-04-05](../daily-digests/2026-04-05-daily-digest.md) - 5 篇
- [2026-04-04](../daily-digests/arxiv-digest-2026-04-04.md) - 4 篇
- [2026-04-03](../daily-digests/arxiv-digest-2026-04-03.md) - 5 篇
- [2026-04-02](../daily-digests/arxiv-digest-2026-04-02.md) - 3 篇
- [2026-04-01](../daily-digests/arxiv-digest-2026-04-01.md) - 3 篇

---

## 🔗 相关链接

- [arXiv](https://arxiv.org/)
- [arXiv 今日论文](https://arxiv.org/list/recent)
- [GitHub 仓库](https://github.com/junxi25liu/daily-arxiv-digest)

---

**自动生成**: Daily arXiv Digest Skill v1.1.0  
**专注领域**: Text-to-Speech, Text-to-Audio, Generative Models, Speech Processing  
**更新频率**: 每日早上 8:00 (Asia/Shanghai)
