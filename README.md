# Daily arXiv Digest - Text-to-Audio, Text-to-Speech & Generative Model

> 🤖 每日 arXiv 论文自动摘要 - Text-to-Audio, Text-to-Speech & Generative Model

[![Last Updated](https://img.shields.io/github/last-commit/junxi25liu/daily-arxiv-digest)](https://github.com/junxi25liu/daily-arxiv-digest/commits/main)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📅 最新论文推荐

### 2026-04-06 (5 篇)

#### 1️⃣ Woosh: A Sound Effects Foundation Model

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

#### 2️⃣ GAP-URGENet: A Generative-Predictive Fusion Framework for Universal Speech Enhancement

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

#### 3️⃣ FastTurn: Unifying Acoustic and Streaming Semantic Cues for Low-Latency Turn Detection

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

#### 4️⃣ DynFOA: Generating First-Order Ambisonics with Conditional Diffusion for Dynamic and Acoustically Complex 360-Degree Videos

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

#### 5️⃣ FineLAP: Taming Heterogeneous Supervision for Fine-grained Language-Audio Pretraining

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

### 2026-04-05 (5 篇，保留最近 10 篇)

#### 6️⃣ T5Gemma-TTS Technical Report

**arXiv**: [2604.01760](https://arxiv.org/abs/2604.01760)  
**作者**: Chihiro Arata, Kiyoshi Kurihara  
**机构**: Independent Research  
**分类**: eess.AS

> **一句话总结**: 基于 T5Gemma 编码器 - 解码器架构的 TTS 模型，通过交叉注意力维持持久文本条件，引入 PM-RoPE 改进时长控制，日语说话人相似度 0.677 超越 XTTSv2。

**核心创新**:
- ✅ 编码器 - 解码器架构，解决长语音文本条件减弱问题
- ✅ PM-RoPE 位置嵌入，注入进度信号控制时长
- ✅ 170k 小时多语言训练，韩语零样本泛化 0.747
- ✅ 开源代码和权重

**[详细摘要 →](daily-digests/2026-04-05-daily-digest.md#1-t5gemma-tts-technical-report)**

---

#### 7️⃣ Prosodic ABX: A Language-Agnostic Method for Measuring Prosodic Contrast in Speech Representations

**arXiv**: [2604.02102](https://arxiv.org/abs/2604.02102)  
**作者**: Haitong Sun, Stephen McIntosh, Kwanghee Choi, et al.  
**机构**: Academic (Japanese Institutions)  
**分类**: cs.CL, cs.LG, cs.SD, eess.AS

> **一句话总结**: 提出 prosodic ABX 判别任务，扩展经典 ABX 框架以评估自监督语音模型对韵律对比的敏感性，仅需少量示例且无需显式标注。

**核心创新**:
- ✅ 韵律 ABX 任务，首次扩展到韵律对比
- ✅ 语言无关方法，无需显式韵律标注
- ✅ 多语言数据集，英语、日语、中文评估
- ✅ 跨条件稳定性，适合低资源场景

**[详细摘要 →](daily-digests/2026-04-05-daily-digest.md#5-prosodic-abx-a-language-agnostic-method-for-measuring-prosodic-contrast-in-speech-representations)**

---

#### 8️⃣ BidirLM: From Text to Omnimodal Bidirectional Encoders by Adapting and Composing Causal LLMs

**arXiv**: [2604.02045](https://arxiv.org/abs/2604.02045)  
**作者**: Nicolas Boizard, Théo Deschamps-Berger, Hippolyte Gisserot-Boukhlef, Céline Hudelot, Pierre Colombo  
**机构**: -  
**分类**: cs.CL, cs.AI

> **一句话总结**: 提出将因果生成式 LLM 转换为双向编码器的系统化方法，通过权重合并和轻量数据混合避免灾难性遗忘，生成在文本、视觉和音频基准上超越替代方案的 BidirLM 编码器家族。

**核心创新**:
- ✅ 先验掩码阶段，关键适配因素
- ✅ 线性权重合并，无需原始预训练数据
- ✅ 轻量多域数据混合，缓解灾难性遗忘
- ✅ 专业化模型组合，转移模态特定能力

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-04.md#2-bidirlm-from-text-to-omnimodal-bidirectional-encoders-by-adapting-and-composing-causal-llms)**

---

#### 9️⃣ PhiNet: Speaker Verification with Phonetic Interpretability

**arXiv**: [2604.01590](https://arxiv.org/abs/2604.01590)  
**作者**: Yi Ma, Shuai Wang, Tianchi Liu, Haizhou Li  
**机构**: -  
**分类**: eess.AS, cs.SD

> **一句话总结**: 提出具有音素可解释性的说话人验证网络 PhiNet，通过利用音素证据增强决策透明度，在 VoxCeleb、SITW 和 LibriSpeech 基准上取得与传统黑盒模型相当的性能。

**核心创新**:
- ✅ 音素级可解释性，详细音素对比
- ✅ 法医说话人对比启发，模仿人类专家
- ✅ 双重可解释性，局部和全局增强
- ✅ 性能不妥协，与传统黑盒模型相当

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-04.md#4-phinet-speaker-verification-with-phonetic-interpretability)**

---

#### 🔟 OmniVoice: Towards Omnilingual Zero-Shot Text-to-Speech with Diffusion Language Models

**arXiv**: [2604.00688](https://arxiv.org/abs/2604.00688)  
**作者**: Han Zhu, Lingxuan Ye, Wei Kang, et al.  
**机构**: -  
**分类**: cs.CL, eess.AS

> **一句话总结**: 支持 600+ 语言的大规模多语言零样本 TTS 模型，基于扩散语言模型离散非自回归架构，直接使用预训练 LLM 初始化实现最优可懂度。

**核心创新**:
- ✅ 600+ 语言覆盖，目前最广的多语言 TTS
- ✅ 扩散语言模型架构，直接文本到声学 token
- ✅ 581k 小时开源数据训练，完全开源

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-03.md#3-omnivoice-towards-omnilingual-zero-shot-text-to-speech-with-diffusion-language-models)**

---

## 📊 统计信息

| 指标 | 数值 |
|------|------|
| 总推荐论文 | 10 篇 (保留最近) |
| 今日新增 | 5 篇 |
| 搜索范围 | cs.SD, cs.CL, cs.AI, cs.LG, eess.AS |
| 时间范围 | 过去 48 小时 |
| 最近更新 | 2026-04-06 |

---

## 📁 历史摘要

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
