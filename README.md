# Daily arXiv Digest - Text-to-Audio, Text-to-Speech & Generative Model

> 🤖 每日 arXiv 论文自动摘要 - Text-to-Audio, Text-to-Speech & Generative Model

[![Last Updated](https://img.shields.io/github/last-commit/junxi25liu/daily-arxiv-digest)](https://github.com/junxi25liu/daily-arxiv-digest/commits/main)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📅 最新论文推荐

### 2026-04-11 (4 篇)

#### 1️⃣ AVGen-Bench: A Task-Driven Benchmark for Multi-Granular Evaluation of Text-to-Audio-Video Generation

**arXiv**: [2604.08540](https://arxiv.org/abs/2604.08540)  
**作者**: Ziwei Zhou, Zeyuan Lai, Rui Wang, Yifan Yang, Zhen Xing, Yuqing Yang, Qi Dai, Lili Qiu, Chong Luo  
**机构**: Microsoft Research  
**分类**: cs.CV, cs.AI, cs.CL

> **一句话总结**: 提出首个任务驱动的 T2AV 生成基准 AVGen-Bench，包含 11 个真实世界类别和多粒度评估框架，揭示当前 T2AV 系统在音频 - 视觉美学与语义可靠性之间存在显著差距。

**核心创新**:
- ✅ 任务驱动基准设计：11 个真实世界类别，超越孤立的音频/视频评估
- ✅ 多粒度评估框架：结合轻量级专家模型与 MLLM，从感知质量到细粒度语义可控性
- ✅ 失败模式分析：揭示文本渲染、语音连贯性、物理推理和音乐音高控制的普遍失败
- ✅ 美学 - 语义差距发现：暴露强音频 - 视觉美学与弱语义可靠性之间的显著差距

**[详细摘要 →](../daily-digests/2026-04-11-daily-digest.md#📄-paper-1-avgen-bench-a-task-driven-benchmark-for-multi-granular-evaluation-of-text-to-audio-video-generation)**

---

#### 2️⃣ CapTalk: Unified Voice Design for Single-Utterance and Dialogue Speech Generation

**arXiv**: [2604.08363](https://arxiv.org/abs/2604.08363)  
**作者**: Xiaosu Su, Zihan Sun, Peilei Jia, Jun Gao  
**机构**: Academic  
**分类**: cs.SD, cs.AI

> **一句话总结**: 提出首个统一的字幕条件文本 - 音频自回归框架 CapTalk，将语音设计从自然语言描述扩展到对话设置，实现单次话语和对话语音设计的统一处理。

**核心创新**:
- ✅ 对话语音设计扩展：首次将语音设计从单次话语生成扩展到多轮对话设置
- ✅ 统一字幕条件框架：单次话语使用话语级字幕，对话使用说话人级字幕
- ✅ CoT 控制序列：引入思维链控制序列显式规划对话中的回合级动态属性
- ✅ 分层变分条件模块：平衡稳定音色保持与上下文自适应表达

**[详细摘要 →](../daily-digests/2026-04-11-daily-digest.md#📄-paper-2-captalk-unified-voice-design-for-single-utterance-and-dialogue-speech-generation)**

---

#### 3️⃣ A Novel Automatic Framework for Speaker Drift Detection in Synthesized Speech

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

**[详细摘要 →](../daily-digests/2026-04-11-daily-digest.md#📄-paper-3-a-novel-automatic-framework-for-speaker-drift-detection-in-synthesized-speech)**

---

#### 4️⃣ Towards Real-Time Human-AI Musical Co-Performance: Accompaniment Generation with Latent Diffusion Models and MAX/MSP

**arXiv**: [2604.07612](https://arxiv.org/abs/2604.07612)  
**作者**: Academic (12 pages, 6 figures)  
**机构**: Academic  
**分类**: cs.SD, cs.AI

> **一句话总结**: 提出实时人机音乐协同表演框架，使用潜在扩散模型生成伴奏，通过一致性蒸馏实现 5.4 倍加速达到实时操作，揭示延迟、前瞻深度和生成质量之间的基本权衡。

**核心创新**:
- ✅ 实时人机协同框架：首个结合 MAX/MSP 实时音频环境与 Python 潜在扩散模型的系统
- ✅ OSC/UDP 通信架构：通过 OSC/UDP 消息桥接 MAX/MSP 前端与 Python 推理服务器
- ✅ 滑动窗口前瞻协议：将伴奏生成形式化为从部分上下文预测未来音频
- ✅ 一致性蒸馏加速：应用一致性蒸馏实现 5.4 倍采样时间减少，达到实时操作

**[详细摘要 →](../daily-digests/2026-04-11-daily-digest.md#📄-paper-4-towards-real-time-human-ai-musical-co-performance-accompaniment-generation-with-latent-diffusion-models-and-maxmsp)**

---

### 2026-04-10 (3 篇)

#### 5️⃣ Anchored Cyclic Generation: A Novel Paradigm for Long-Sequence Symbolic Music Generation

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

#### 6️⃣ Active Noise Cancellation on Open-Ear Smart Glasses

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

#### 7️⃣ Generalizable Audio-Visual Navigation via Binaural Difference Attention and Action Transition Prediction

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

### 2026-04-09 (3 篇，保留最近 10 篇)

#### 8️⃣ AudioKV: KV Cache Eviction in Efficient Large Audio Language Models

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

#### 9️⃣ Generating Synthetic Doctor-Patient Conversations for Long-form Audio Summarization

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

#### 🔟 Brain-to-Speech: Prosody Feature Engineering and Transformer-Based Reconstruction

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

## 📊 统计信息

| 指标 | 数值 |
|------|------|
| 总推荐论文 | 10 篇 (保留最近 3 天) |
| 今日新增 | 4 篇 |
| 搜索范围 | cs.SD, cs.CL, cs.AI, cs.LG, eess.AS, cs.CV |
| 时间范围 | 过去 48 小时 |
| 最近更新 | 2026-04-11 |

---

## 📁 历史摘要

- [2026-04-11](../daily-digests/2026-04-11-daily-digest.md) - 4 篇
- [2026-04-10](../daily-digests/2026-04-10-daily-digest.md) - 3 篇
- [2026-04-09](../daily-digests/2026-04-09-daily-digest.md) - 5 篇
- [2026-04-08](../daily-digests/2026-04-08-daily-digest.md) - 5 篇
- [2026-04-07](../daily-digests/2026-04-07-daily-digest.md) - 5 篇
- [2026-04-06](../daily-digests/2026-04-06-daily-digest.md) - 5 篇
- [2026-04-05](../daily-digests/2026-04-05-daily-digest.md) - 5 篇
- [2026-04-04](../daily-digests/arxiv-digest-2026-04-04.md) - 4 篇
- [2026-04-03](../daily-digests/arxiv-digest-2026-04-03.md) - 5 篇
- [2026-04-02](../daily-digests/arxiv-digest-2026-04-02.md) - 3 篇

---

## 🔗 相关链接

- [arXiv](https://arxiv.org/)
- [arXiv 今日论文](https://arxiv.org/list/recent)
- [GitHub 仓库](https://github.com/junxi25liu/daily-arxiv-digest)

---

**自动生成**: Daily arXiv Digest Skill v1.1.0  
**专注领域**: Text-to-Speech, Text-to-Audio, Generative Models, Speech Processing  
**更新频率**: 每日早上 8:00 (Asia/Shanghai)
