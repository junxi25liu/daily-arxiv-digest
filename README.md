# Daily arXiv Digest - Text-to-Audio, Text-to-Speech & Generative Model

> 🤖 每日 arXiv 论文自动摘要 - Text-to-Audio, Text-to-Speech & Generative Model

[![Last Updated](https://img.shields.io/github/last-commit/junxi25liu/daily-arxiv-digest)](https://github.com/junxi25liu/daily-arxiv-digest/commits/main)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📅 最新论文推荐

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
| 总推荐论文 | 10 篇 (保留最近) |
| 今日新增 | 5 篇 |
| 搜索范围 | cs.SD, cs.CL, cs.AI, cs.LG, eess.AS |
| 时间范围 | 过去 48 小时 |
| 最近更新 | 2026-04-08 |

---

## 📁 历史摘要

- [2026-04-08](../daily-digests/2026-04-08-daily-digest.md) - 5 篇
- [2026-04-07](../daily-digests/2026-04-07-daily-digest.md) - 5 篇
- [2026-04-06](../daily-digests/2026-04-06-daily-digest.md) - 5 篇
- [2026-04-05](../daily-digests/2026-04-05-daily-digest.md) - 5 篇
- [2026-04-04](../daily-digests/arxiv-digest-2026-04-04.md) - 4 篇
- [2026-04-03](../daily-digests/arxiv-digest-2026-04-03.md) - 5 篇
- [2026-04-02](../daily-digests/arxiv-digest-2026-04-02.md) - 3 篇
- [2026-04-01](../daily-digests/arxiv-digest-2026-04-01.md) - 3 篇
- [2026-03-31](../daily-digests/arxiv-digest-2026-03-31.md) - 3 篇

---

## 🔗 相关链接

- [arXiv](https://arxiv.org/)
- [arXiv 今日论文](https://arxiv.org/list/recent)
- [GitHub 仓库](https://github.com/junxi25liu/daily-arxiv-digest)

---

**自动生成**: Daily arXiv Digest Skill v1.1.0  
**专注领域**: Text-to-Speech, Text-to-Audio, Generative Models, Speech Processing  
**更新频率**: 每日早上 8:00 (Asia/Shanghai)
