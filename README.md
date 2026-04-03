# Daily arXiv Digest - Text-to-Audio, Text-to-Speech & Generative Model

> 🤖 每日 arXiv 论文自动摘要 - Text-to-Audio, Text-to-Speech & Generative Model

[![Last Updated](https://img.shields.io/github/last-commit/junxi25liu/daily-arxiv-digest)](https://github.com/junxi25liu/daily-arxiv-digest/commits/main)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📅 最新论文推荐

### 2026-04-03 (5 篇)

#### 1️⃣ Woosh: A Sound Effects Foundation Model

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

#### 2️⃣ T5Gemma-TTS Technical Report

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

#### 3️⃣ OmniVoice: Towards Omnilingual Zero-Shot Text-to-Speech with Diffusion Language Models

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

#### 4️⃣ FastTurn: Unifying Acoustic and Streaming Semantic Cues for Low-Latency and Robust Turn Detection

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

#### 5️⃣ Diff-VS: Efficient Audio-Aware Diffusion U-Net for Vocals Separation

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

### 2026-04-02 (3 篇)

#### 6️⃣ MambaVoiceCloning: Efficient and Expressive Text-to-Speech via State-Space Modeling and Diffusion Control

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

#### 7️⃣ FineLAP: Taming Heterogeneous Supervision for Fine-grained Language-Audio Pretraining

**arXiv**: [2604.01155](https://arxiv.org/abs/2604.01155)  
**作者**: Xiquan Li 等  
**机构**: -  
**分类**: cs.SD

> **一句话总结**: 提出细粒度语言 - 音频预训练范式，通过双流 sigmoid 损失和聚类采样策略，联合学习片段级和帧级对齐，在音频理解任务上实现 SOTA 性能。

**核心创新**:
- ✅ 双流 Sigmoid 损失，联合学习片段级和帧级对齐
- ✅ 解耦音频投影器，同时捕获全局语义和局部细节
- ✅ FineLAP-100k 数据集，缓解时序标注数据稀缺

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-02.md#2-finelap-taming-heterogeneous-supervision-for-fine-grained-language-audio-pretraining)**

---

#### 8️⃣ Sona: Real-Time Multi-Target Sound Attenuation for Noise Sensitivity

**arXiv**: [2604.00447](https://arxiv.org/abs/2604.00447)  
**作者**: Jeremy Zhengqi Huang 等  
**机构**: -  
**分类**: cs.SD, cs.HC

> **一句话总结**: 交互式移动系统，支持实时多目标声音衰减，帮助噪声敏感人群选择性减弱烦人声音，同时保持对周围环境的感知。

**核心创新**:
- ✅ 多目标同时衰减，克服单目标限制
- ✅ 目标条件神经管道，用户可扩展声音类别
- ✅ 实时设备端运行，低延迟

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-02.md#3-sona-real-time-multi-target-sound-attenuation-for-noise-sensitivity)**

---

### 2026-04-01 (2 篇，保留最近 10 篇)

#### 9️⃣ LongCat-AudioDiT: High-Fidelity Diffusion Text-to-Speech in the Waveform Latent Space

**arXiv**: [2603.29339](https://arxiv.org/abs/2603.29339)  
**作者**: Detai Xin 等  
**机构**: Meituan LongCat  
**分类**: cs.SD, eess.AS

> **一句话总结**: 提出直接在波形潜空间操作的扩散 TTS 模型，无需中间声学特征，简化 TTS 流程并实现 SOTA 的零样本声音克隆性能。

**核心创新**:
- ✅ 波形潜空间直接生成，摒弃 mel 频谱等中间表示
- ✅ 自适应投影引导替代传统 CFG，提升生成质量
- ✅ SOTA 零样本克隆，超越 Seed-TTS

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-01.md#1-longcat-audiokit-high-fidelity-diffusion-text-to-speech-in-the-waveform-latent-space)**

---

#### 🔟 OmniVoice: Towards Omnilingual Zero-Shot Text-to-Speech with Diffusion Language Models

**arXiv**: [2604.00688](https://arxiv.org/abs/2604.00688)  
**作者**: Han Zhu, Lingxuan Ye, Wei Kang, et al.  
**机构**: -  
**分类**: cs.CL, eess.AS

> **一句话总结**: 支持 600+ 语言的大规模多语言零样本 TTS 模型，基于扩散语言模型离散非自回归架构，直接使用预训练 LLM 初始化。

**核心创新**:
- ✅ 600+ 语言覆盖，目前最广的多语言 TTS
- ✅ 扩散语言模型架构，直接文本到声学 token
- ✅ 581k 小时开源数据训练

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-01.md#5-omnivoice-towards-omnilingual-zero-shot-text-to-speech-with-diffusion-language-models)**

---

## 📊 今日统计

| 指标 | 数值 |
|------|------|
| 检索论文总数 (04-03) | ~112 篇 |
| 过去 48 小时论文 (04-03) | 23 篇 |
| 筛选推荐 (04-03) | 5 篇 |
| 筛选推荐 (04-02) | 3 篇 |
| 筛选推荐 (04-01) | 4 篇 |
| 搜索分类 | cs.CL, cs.SD, cs.AI, cs.LG, eess.AS |
| 搜索方向 | TTS, Speech Synthesis, Audio Generation, Generative Models |

---

## 📁 历史摘要

| 日期 | 论文数 | 主要方向 | 链接 |
|------|--------|----------|------|
| 2026-04-03 | 5 | Sound Effects, Encoder-Decoder TTS, 600+ Language TTS, Turn Detection, Vocal Separation | [查看](daily-digests/arxiv-digest-2026-04-03.md) |
| 2026-04-02 | 3 | SSM TTS, Fine-grained Pretraining, Sound Attenuation | [查看](daily-digests/arxiv-digest-2026-04-02.md) |
| 2026-04-01 | 4 | Waveform Latent TTS, Intelligibility, Binaural Audio, Deepfake Detection | [查看](daily-digests/arxiv-digest-2026-04-01.md) |
| 2026-03-31 | 5 | Masked Diffusion TTS, Stylistic Pretraining, Singing Voice | [查看](daily-digests/arxiv-digest-2026-03-31.md) |

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
- 👨🔬 高影响力作者 (h-index > 15)
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

**Last Updated**: 2026-04-03  
**Total Papers Recommended**: 10 (最近 10 篇概览)

---

<div align="center">

**🌟 如果这个项目对你有帮助，请给个 Star！**

</div>
