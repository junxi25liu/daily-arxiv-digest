# Daily arXiv Digest - Text-to-Audio, Text-to-Speech & Generative Model

> 🤖 每日 arXiv 论文自动摘要 - Text-to-Audio, Text-to-Speech & Generative Model

[![Last Updated](https://img.shields.io/github/last-commit/junxi25liu/daily-arxiv-digest)](https://github.com/junxi25liu/daily-arxiv-digest/commits/main)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📅 最新论文推荐

### 2026-04-05 (5 篇)

#### 1️⃣ T5Gemma-TTS Technical Report

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

#### 2️⃣ Woosh: A Sound Effects Foundation Model

**arXiv**: [2604.01929](https://arxiv.org/abs/2604.01929)  
**作者**: Gaëtan Hadjeres, Marc Ferras, Khaled Koutini, et al.  
**机构**: Sony AI  
**分类**: cs.SD, cs.AI, cs.LG

> **一句话总结**: Sony AI 开源的音效基础模型 Woosh，提供完整的音频编码器/解码器、文本 - 音频对齐、文本生成音频和视频生成音频模型套件。

**核心创新**:
- ✅ 完整开源的音效基础模型 (T2A + V2A)
- ✅ 蒸馏模型支持低资源快速推理
- ✅ 性能媲美或超越 StableAudio-Open 和 TangoFlux
- ✅ 公开演示页面和代码

**[详细摘要 →](daily-digests/2026-04-05-daily-digest.md#2-woosh-a-sound-effects-foundation-model)**

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

**[详细摘要 →](daily-digests/2026-04-05-daily-digest.md#3-fastturn-unifying-acoustic-and-streaming-semantic-cues-for-low-latency-and-robust-turn-detection)**

---

#### 4️⃣ GAP-URGENet: A Generative-Predictive Fusion Framework for Universal Speech Enhancement

**arXiv**: [2604.01832](https://arxiv.org/abs/2604.01832)  
**作者**: Xiaobin Rong, Yushi Wang, Zheng Wang, Jing Lu  
**机构**: -  
**分类**: eess.AS, cs.SD

> **一句话总结**: 提出生成 - 预测融合框架 GAP-URGENet，结合自监督表示域的全栈语音修复和频谱图域增强，在 ICASSP 2026 URGENT Challenge 中取得目标评估第 1 名。

**核心创新**:
- ✅ 生成 - 预测双分支架构，互补增强
- ✅ 神经声码器重建，保持高质量语音
- ✅ 后处理融合模块，带宽扩展至 48kHz
- ✅ ICASSP 2026 URGENT Challenge 目标评估第 1 名

**[详细摘要 →](daily-digests/2026-04-05-daily-digest.md#4-gap-urgenet-a-generative-predictive-fusion-framework-for-universal-speech-enhancement)**

---

#### 5️⃣ Prosodic ABX: A Language-Agnostic Method for Measuring Prosodic Contrast in Speech Representations

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

### 2026-04-04 (4 篇，保留最近 10 篇)

#### 6️⃣ BidirLM: From Text to Omnimodal Bidirectional Encoders by Adapting and Composing Causal LLMs

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

#### 7️⃣ PhiNet: Speaker Verification with Phonetic Interpretability

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

#### 8️⃣ OmniVoice: Towards Omnilingual Zero-Shot Text-to-Speech with Diffusion Language Models

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

#### 9️⃣ Diff-VS: Efficient Audio-Aware Diffusion U-Net for Vocals Separation

**arXiv**: [2604.01120](https://arxiv.org/abs/2604.01120)  
**作者**: Yun-Ning Hung, Richard Vogl, Filip Korzeniowski, Igor Pereira  
**机构**: -  
**分类**: eess.AS

> **一句话总结**: 基于 EDM 框架的生成式人声分离模型，在客观指标上匹配判别式基线，感知质量达到 SOTA，ICASSP 2026 接收。

**核心创新**:
- ✅ EDM 框架应用于音乐源分离
- ✅ 改进 U-Net 架构，处理复数 STFT 频谱图
- ✅ 客观指标匹配判别式，感知质量 SOTA

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-03.md#5-diff-vs-efficient-audio-aware-diffusion-u-net-for-vocals-separation)**

---

#### 🔟 MambaVoiceCloning: Efficient and Expressive Text-to-Speech via State-Space Modeling and Diffusion Control

**arXiv**: [2604.00292](https://arxiv.org/abs/2604.00292)  
**作者**: Sahil Kumar 等  
**机构**: ICLR 2026 接收  
**分类**: cs.SD, cs.LG

> **一句话总结**: 首次实现扩散 TTS 的条件路径在推理时完全使用状态空间模型（SSM），移除所有注意力和显式 RNN 层，实现线性时间复杂度和 1.6 倍吞吐提升。

**核心创新**:
- ✅ 纯 SSM 条件路径，移除注意力和 RNN 层
- ✅ 线性时间复杂度 O(T)，支持流式推理
- ✅ 编码器参数降至 21M，吞吐提升 1.6 倍

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-02.md#1-mambavoicecloning-efficient-and-expressive-text-to-speech-via-state-space-modeling-and-diffusion-control)**

#### 1️⃣ GAP-URGENet: A Generative-Predictive Fusion Framework for Universal Speech Enhancement

**arXiv**: [2604.01832](https://arxiv.org/abs/2604.01832)  
**作者**: Xiaobin Rong, Yushi Wang, Zheng Wang, Jing Lu  
**机构**: -  
**分类**: eess.AS, cs.SD

> **一句话总结**: 提出生成 - 预测融合框架 GAP-URGENet，结合自监督表示域的全栈语音修复和频谱图域增强，在 ICASSP 2026 URGENT Challenge 中取得目标评估第 1 名。

**核心创新**:
- ✅ 生成 - 预测双分支架构，互补增强
- ✅ 神经声码器重建，保持高质量语音
- ✅ 后处理融合模块，带宽扩展至 48kHz
- ✅ ICASSP 2026 URGENT Challenge 目标评估第 1 名

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-04.md#1-gap-urgenet-a-generative-predictive-fusion-framework-for-universal-speech-enhancement)**

---

#### 2️⃣ BidirLM: From Text to Omnimodal Bidirectional Encoders by Adapting and Composing Causal LLMs

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

#### 3️⃣ Prosodic ABX: A Language-Agnostic Method for Measuring Prosodic Contrast in Speech Representations

**arXiv**: [2604.02102](https://arxiv.org/abs/2604.02102)  
**作者**: Haitong Sun, Stephen McIntosh, Kwanghee Choi, Eunjung Yeo, Daisuke Saito, Nobuaki Minematsu  
**机构**: University of Tokyo  
**分类**: cs.CL, cs.LG, cs.SD, eess.AS

> **一句话总结**: 提出 prosodic ABX 判别任务，扩展经典 ABX 框架以评估自监督语音模型对韵律对比的敏感性，仅需少量示例且无需显式标注，发布英语和日语最小对数据集。

**核心创新**:
- ✅ 韵律 ABX 任务，首次扩展到韵律对比
- ✅ 语言无关方法，无需显式韵律标注
- ✅ 多语言数据集，英语、日语、中文评估
- ✅ 跨条件稳定性，适合低资源场景

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-04.md#3-prosodic-abx-a-language-agnostic-method-for-measuring-prosodic-contrast-in-speech-representations)**

---

#### 4️⃣ PhiNet: Speaker Verification with Phonetic Interpretability

**arXiv**: [2604.01590](https://arxiv.org/abs/2604.01590)  
**作者**: Yi Ma, Shuai Wang, Tianchi Liu, Haizhou Li  
**机构**: -  
**分类**: eess.AS, cs.SD

> **一句话总结**: 提出具有音素可解释性的说话人验证网络 PhiNet，通过利用音素证据增强决策透明度，在 VoxCeleb、SITW 和 LibriSpeech 基准上取得与传统黑盒模型相当的性能，同时提供有意义的解释。

**核心创新**:
- ✅ 音素级可解释性，详细音素对比
- ✅ 法医说话人对比启发，模仿人类专家
- ✅ 双重可解释性，局部和全局增强
- ✅ 性能不妥协，与传统黑盒模型相当

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-04.md#4-phinet-speaker-verification-with-phonetic-interpretability)**

---

### 2026-04-03 (5 篇，保留最近 10 篇)

#### 5️⃣ Woosh: A Sound Effects Foundation Model

**arXiv**: [2604.01929](https://arxiv.org/abs/2604.01929)  
**作者**: Gaëtan Hadjeres, Marc Ferras, Khaled Koutini, et al.  
**机构**: Sony AI  
**分类**: cs.SD, cs.AI, cs.LG

> **一句话总结**: Sony AI 开源的音效基础模型 Woosh，提供高质量的文本生成音频和视频生成音频能力，性能媲美或超越 StableAudio-Open 和 TangoFlux。

**核心创新**:
- ✅ 完整开源的音效基础模型 (T2A + V2A)
- ✅ 蒸馏模型支持低资源快速推理
- ✅ 全面评估，性能超越现有开源方案

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-03.md#1-woosh-a-sound-effects-foundation-model)**

---

#### 6️⃣ T5Gemma-TTS Technical Report

**arXiv**: [2604.01760](https://arxiv.org/abs/2604.01760)  
**作者**: Chihiro Arata, Kiyoshi Kurihara  
**机构**: -  
**分类**: eess.AS

> **一句话总结**: 基于 T5Gemma 编码器 - 解码器架构的 TTS 模型，通过交叉注意力维持持久文本条件，引入 PM-RoPE 改进时长控制，多语言零样本克隆 SOTA。

**核心创新**:
- ✅ 编码器 - 解码器架构，解决长语音文本条件减弱问题
- ✅ PM-RoPE 位置嵌入，注入进度信号控制时长
- ✅ 170k 小时多语言训练，韩语零样本泛化 0.747

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-03.md#2-t5gemma-tts-technical-report)**

---

#### 7️⃣ OmniVoice: Towards Omnilingual Zero-Shot Text-to-Speech with Diffusion Language Models

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

#### 8️⃣ FastTurn: Unifying Acoustic and Streaming Semantic Cues for Low-Latency and Robust Turn Detection

**arXiv**: [2604.01897](https://arxiv.org/abs/2604.01897)  
**作者**: Chengyou Wang, Hongfei Xue, Chunjiang He, et al.  
**机构**: -  
**分类**: cs.SD

> **一句话总结**: 统一流式 CTC 解码与声学特征的轮次检测框架，实现低延迟高准确率的全双工对话交互，发布真实对话测试集。

**核心创新**:
- ✅ 流式 CTC+ 声学特征，早期决策保持语义
- ✅ 真实对话测试集，包含重叠语音、回应等
- ✅ 低延迟高准确率，鲁棒性强

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-03.md#4-fastturn-unifying-acoustic-and-streaming-semantic-cues-for-low-latency-and-robust-turn-detection)**

---

#### 9️⃣ Diff-VS: Efficient Audio-Aware Diffusion U-Net for Vocals Separation

**arXiv**: [2604.01120](https://arxiv.org/abs/2604.01120)  
**作者**: Yun-Ning Hung, Richard Vogl, Filip Korzeniowski, Igor Pereira  
**机构**: -  
**分类**: eess.AS

> **一句话总结**: 基于 EDM 框架的生成式人声分离模型，在客观指标上匹配判别式基线，感知质量达到 SOTA，ICASSP 2026 接收。

**核心创新**:
- ✅ EDM 框架应用于音乐源分离
- ✅ 改进 U-Net 架构，处理复数 STFT 频谱图
- ✅ 客观指标匹配判别式，感知质量 SOTA

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-03.md#5-diff-vs-efficient-audio-aware-diffusion-u-net-for-vocals-separation)**

---

#### 🔟 MambaVoiceCloning: Efficient and Expressive Text-to-Speech via State-Space Modeling and Diffusion Control

**arXiv**: [2604.00292](https://arxiv.org/abs/2604.00292)  
**作者**: Sahil Kumar 等  
**机构**: ICLR 2026 接收  
**分类**: cs.SD, cs.LG

> **一句话总结**: 首次实现扩散 TTS 的条件路径在推理时完全使用状态空间模型（SSM），移除所有注意力和显式 RNN 层，实现线性时间复杂度和 1.6 倍吞吐提升。

**核心创新**:
- ✅ 纯 SSM 条件路径，移除注意力和 RNN 层
- ✅ 线性时间复杂度 O(T)，支持流式推理
- ✅ 编码器参数降至 21M，吞吐提升 1.6 倍

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-02.md#1-mambavoicecloning-efficient-and-expressive-text-to-speech-via-state-space-modeling-and-diffusion-control)**

---

## 📊 今日统计

| 指标 | 数值 |
|------|------|
| 检索论文总数 (04-05) | ~77 篇 |
| 过去 48 小时新论文 (04-05) | 5 篇精选 |
| 筛选推荐 (04-05) | 5 篇 |
| 保留历史 (04-04) | 2 篇 |
| 保留历史 (04-03) | 2 篇 |
| 保留历史 (04-02) | 1 篇 |
| 搜索分类 | cs.CL, cs.SD, cs.AI, cs.LG, eess.AS |
| 搜索方向 | TTS, Speech Synthesis, Audio Generation, Generative Models, Speech Enhancement |

---

## 📁 历史摘要

| 日期 | 论文数 | 主要方向 | 链接 |
|------|--------|----------|------|
| 2026-04-05 | 5 | Encoder-Decoder TTS, Sound Effects Foundation, Turn Detection, Speech Enhancement, Prosodic Evaluation | [查看](daily-digests/2026-04-05-daily-digest.md) |
| 2026-04-04 | 4 | Speech Enhancement, Omnimodal Encoder, Prosodic Evaluation, Speaker Verification | [查看](daily-digests/arxiv-digest-2026-04-04.md) |
| 2026-04-03 | 5 | Sound Effects, Encoder-Decoder TTS, 600+ Language TTS, Turn Detection, Vocal Separation | [查看](daily-digests/arxiv-digest-2026-04-03.md) |
| 2026-04-02 | 1 | SSM TTS | [查看](daily-digests/arxiv-digest-2026-04-02.md) |
| 2026-04-01 | 4 | Waveform Latent TTS, Intelligibility, Binaural Audio, Deepfake Detection | [查看](daily-digests/arxiv-digest-2026-04-01.md) |

---

## 🔍 搜索配置

### 搜索分类
- **cs.CL** - 计算语言学
- **cs.SD** - 语音
- **cs.AI** - 人工智能
- **cs.LG** - 机器学习
- **eess.AS** - 音频与语音处理

### 主要搜索方向
1. **Text-to-Audio** - 文本生成音频
2. **Text-to-Speech (TTS)** - 文本转语音
3. **Generative Model** - 生成式模型

### 关键词
text-to-audio, text to audio, text-to-speech, text to speech, TTS, speech synthesis, audio generation, generative model, generative models, diffusion model, transformer

### 筛选标准
- 🏛️ 知名机构 (MIT, Stanford, Google, Meta, Sony AI, 等)
- 👨‍🔬 高影响力作者 (h-index > 15)
- 🔥 热门方向 (LLM, Diffusion, Zero-Shot, 等)
- 💻 代码可用 (优先)

---

## ⏰ 自动更新

本仓库每天早上 **8:00 (Asia/Shanghai)** 自动更新最新论文摘要。

定时任务配置：
- **执行时间**: 每天早上 8:00
- **搜索范围**: 过去 24-48 小时 arXiv 论文
- **推荐数量**: 3-5 篇精品论文

---

## 🛠️ 技术栈

- **数据源**: [arXiv API](https://arxiv.org/help/api)
- **技能框架**: OpenClaw Skills
- **自动化**: Cron 定时任务
- **技能仓库**: [daily-arxiv-digest-skill](https://github.com/junxi25liu/daily-arxiv-digest-skill)

---

## 📝 自定义配置

### 修改搜索方向

编辑配置文件 `config.json`:

```json
{
  "search": {
    "categories": ["cs.CL", "cs.SD", "cs.AI", "cs.LG", "eess.AS"],
    "customKeywords": [
      "text-to-speech", "TTS", "speech synthesis",
      "audio generation", "generative model", "diffusion"
    ]
  }
}
```

### 修改执行时间

```json
{
  "schedule": {
    "cron": "0 9 * * *"  // 改为每天早上 9 点
  }
}
```

---

## 📬 订阅更新

- 🔔 **Watch** 本仓库获取更新通知
- ⭐ **Star** 支持本项目
- 🍴 **Fork** 自定义你的论文推荐

---

## 📄 许可

MIT License - 详见 [LICENSE](LICENSE)

---

## 👤 作者

**Liu** (@junxi25liu)

---

## 🙏 致谢

- [arXiv](https://arxiv.org/) - 论文数据源
- [OpenClaw](https://openclaw.ai/) - AI 助手框架
- [karpathy/nanochat](https://github.com/karpathy/nanochat) - 论文阅读技能参考
- [huangkiki/dailypaper-skills](https://github.com/huangkiki/dailypaper-skills) - 每日论文技能参考

---

**Last Updated**: 2026-04-05  
**Total Papers Recommended**: 10 (最近 10 篇概览)

---

<div align="center">

**🌟 如果这个项目对你有帮助，请给个 Star！**

</div>
