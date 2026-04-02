# Daily arXiv Digest - Text-to-Audio, Text-to-Speech & Generative Model

> 🤖 每日 arXiv 论文自动摘要 - Text-to-Audio, Text-to-Speech & Generative Model

[![Last Updated](https://img.shields.io/github/last-commit/junxi25liu/daily-arxiv-digest)](https://github.com/junxi25liu/daily-arxiv-digest/commits/main)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📅 最新论文推荐

### 2026-04-02 (3 篇)

#### 1️⃣ MambaVoiceCloning: Efficient and Expressive Text-to-Speech via State-Space Modeling and Diffusion Control

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

#### 2️⃣ FineLAP: Taming Heterogeneous Supervision for Fine-grained Language-Audio Pretraining

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

#### 3️⃣ Sona: Real-Time Multi-Target Sound Attenuation for Noise Sensitivity

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

### 2026-04-01 (4 篇)

#### 4️⃣ LongCat-AudioDiT: High-Fidelity Diffusion Text-to-Speech in the Waveform Latent Space

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

#### 5️⃣ Covertly Improving Intelligibility with Data-Driven Adaptations of Speech Timing

**arXiv**: [2603.30032](https://arxiv.org/abs/2603.30032)  
**作者**: Paige Tuttösí 等  
**机构**: -  
**分类**: cs.CL, cs.SD

> **一句话总结**: 研究发现针对性调整语速（而非全局减速）能显著提升语音可懂度，并据此构建了数据驱动的 TTS 算法，在听者无感知的情况下改善理解。

**核心创新**:
- ✅ 剪刀式语速模式，针对性调整而非全局减速
- ✅ 跨语言稳定性，母语者和 L2 听者均有效
- ✅ 隐蔽性改善，听者未察觉但理解度提升

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-01.md#2-covertly-improving-intelligibility-with-data-driven-adaptations-of-speech-timing)**

---

#### 6️⃣ SIREN: Spatially-Informed Reconstruction of Binaural Audio with Vision

**arXiv**: [2603.29820](https://arxiv.org/abs/2603.29820)  
**作者**: Seoyeon Ko 等  
**机构**: ICASSP 2026  
**分类**: cs.SD

> **一句话总结**: 视觉引导的单声道到双耳音频转换框架，通过显式预测左右声道，实现沉浸式空间音频重建。

**核心创新**:
- ✅ ViT 编码器 + 双头自注意力，学习共享场景图
- ✅ 软退火空间先验，避免过度约束
- ✅ 两阶段置信度加权融合，抑制串扰

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-01.md#3-siren-spatially-informed-reconstruction-of-binaural-audio-with-vision)**

---

#### 7️⃣ TRACE: Training-Free Partial Audio Deepfake Detection via Embedding Trajectory Analysis

**arXiv**: [2604.01083](https://arxiv.org/abs/2604.01083)  
**作者**: Awais Khan 等  
**机构**: -  
**分类**: cs.SD, cs.AI, cs.CV

> **一句话总结**: 无需训练的音频深度伪造检测框架，通过分析语音基础模型嵌入轨迹的一阶动态，检测部分合成的音频片段。

**核心创新**:
- ✅ 无需训练，利用冻结的语音基础模型
- ✅ 嵌入轨迹分析，检测拼接边界突变
- ✅ 泛化能力强，跨语言、跨合成方法表现优异

**[详细摘要 →](daily-digests/arxiv-digest-2026-04-01.md#4-trace-training-free-partial-audio-deepfake-detection-via-embedding-trajectory-analysis)**

---

### 2026-03-31 (3 篇，保留最近 10 篇)

#### 8️⃣ LLaDA-TTS: Unifying Speech Synthesis and Zero-Shot Editing via Masked Diffusion Modeling

**arXiv**: [2603.26364](https://arxiv.org/abs/2603.26364)  
**作者**: Xiaoyu Fan, Huizhi Xie, Wei Zou, Yunzhang Chen  
**机构**: -  
**分类**: cs.SD

> **一句话总结**: 首次将预训练自回归 TTS 模型成功转换为掩码扩散模型，在保持同等音质的同时实现 2 倍推理加速，并原生支持零样本语音编辑。

**核心创新**:
- ✅ 掩码扩散替代自回归，2 倍推理加速
- ✅ 仅需 50 小时微调数据即可迁移预训练权重
- ✅ 原生支持零样本语音编辑（插入、删除、替换）

**[详细摘要 →](daily-digests/arxiv-digest-2026-03-31.md#1-llada-tts-unifying-speech-synthesis-and-zero-shot-editing-via-masked-diffusion-modeling)**

---

#### 9️⃣ ParaSpeechCLAP: A Dual-Encoder Speech-Text Model for Rich Stylistic Language-Audio Pretraining

**arXiv**: [2603.28737](https://arxiv.org/abs/2603.28737)  
**作者**: Anuj Diwan, Eunsol Choi, David Harwath  
**机构**: UT Austin  
**分类**: eess.AS, cs.AI, cs.CL, cs.SD

> **一句话总结**: 提出双编码器对比学习框架，将语音和文本风格描述映射到统一嵌入空间，支持远超现有模型的丰富风格描述符（音高、质感、情感等）。

**核心创新**:
- ✅ 支持丰富风格描述（音高、质感、情感等）
- ✅ 三种变体：Intrinsic、Situational、Combined
- ✅ 可作为推理时奖励模型用于风格提示 TTS

**[详细摘要 →](daily-digests/arxiv-digest-2026-03-31.md#2-paraspeechclap-a-dual-encoder-speech-text-model-for-rich-stylistic-language-audio-pretraining)**

---

#### 🔟 YingMusic-Singer: Controllable Singing Voice Synthesis with Multi-Level Conditioning

**arXiv**: [2603.24589](https://arxiv.org/abs/2603.24589)  
**作者**: -  
**机构**: 西北工业大学  
**分类**: cs.SD

> **一句话总结**: 可控歌声合成系统，支持多层级条件控制（音高、歌词、情感等）。

**核心创新**:
- ✅ 多层级条件控制
- ✅ 支持歌声合成与编辑
- ✅ 中文歌声合成优化

**[详细摘要 →](daily-digests/arxiv-digest-2026-03-31.md#3-yingmusic-singer-controllable-singing-voice-synthesis-with-multi-level-conditioning)**

---

## 📊 今日统计

| 指标 | 数值 |
|------|------|
| 检索论文总数 (04-02) | ~25 篇 |
| 检索论文总数 (04-01) | ~30 篇 |
| 筛选推荐 (04-02) | 3 篇 |
| 筛选推荐 (04-01) | 4 篇 |
| 搜索分类 | cs.CL, cs.SD, cs.AI, cs.LG, eess.AS |
| 搜索方向 | TTS, Speech Synthesis, Audio Generation, Generative Models |

---

## 📁 历史摘要

| 日期 | 论文数 | 主要方向 | 链接 |
|------|--------|----------|------|
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
- 🏛️ 知名机构 (MIT, Stanford, Google, Meta, 等)
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

**Last Updated**: 2026-04-02  
**Total Papers Recommended**: 10 (最近 10 篇概览)

---

<div align="center">

**🌟 如果这个项目对你有帮助，请给个 Star！**

</div>
