# Daily arXiv Digest - 2026-04-03

> 🤖 自动生成的每日 arXiv 论文摘要 - Text-to-Audio, Text-to-Speech & Generative Model

**生成时间**: 2026-04-03 09:00 AM (Asia/Shanghai)  
**搜索范围**: 过去 48 小时 (2026-04-01 至 2026-04-03)  
**搜索分类**: cs.CL, cs.SD, cs.AI, cs.LG, eess.AS

---

## 📅 今日推荐论文

共推荐 **5 篇** 论文

---

## 1️⃣ Woosh: A Sound Effects Foundation Model

**arXiv**: [2604.01929](https://arxiv.org/abs/2604.01929)  
**作者**: Gaëtan Hadjeres, Marc Ferras, Khaled Koutini, Benno Weck, Alexandre Bittar, Thomas Hummel, Zineb Lahrici, Hakim Missoum, Joan Serrà, Yuki Mitsufuji  
**机构**: Sony AI  
**分类**: cs.SD, cs.AI, cs.LG  
**代码**: [GitHub - SonyResearch/Woosh](https://github.com/SonyResearch/Woosh)  
**Demo**: [Woosh Demo](https://sonyresearch.github.io/Woosh/)

### 📌 一句话总结

Sony AI 开源的音效基础模型 Woosh，提供高质量的文本生成音频和视频生成音频能力，性能媲美或超越 StableAudio-Open 和 TangoFlux 等现有开源模型。

### 💡 核心创新点

1. **完整开源的音效基础模型**: 包含高质量音频编码器/解码器、文本 - 音频对齐模型、文本生成音频模型和视频生成音频模型
2. **蒸馏模型支持低资源部署**: 提供蒸馏版本的文本生成音频和视频生成音频模型，支持低资源环境下的快速推理
3. **全面评估**: 在公开和私有数据集上评估，各模块性能均达到或超越现有开源替代方案

### 🔧 技术方法

- **音频编码器/解码器**: 高质量音频压缩与重建
- **文本 - 音频对齐模型**: 用于条件生成的文本和音频特征对齐
- **文本生成音频 (T2A)**: 从文本描述生成音效
- **视频生成音频 (V2A)**: 从视频内容生成配套音效
- **蒸馏模型**: 通过知识蒸馏实现更小的模型尺寸和更快的推理速度

### 📊 实验结果

- 在公开和私有数据集上评估
- 各模块性能与 StableAudio-Open 和 TangoFlux 相比具有竞争力或更优
- 支持快速推理和低资源部署

### 🤔 个人评价

Woosh 的发布为音效生成研究社区提供了重要的开源基线模型。Sony AI 选择完全开源模型权重和推理代码，这对于推动音效生成领域的发展具有重要意义。蒸馏模型的提供也降低了使用门槛，使得资源有限的研究者也能使用这些先进模型。

### 🔗 相关链接

- [arXiv 页面](https://arxiv.org/abs/2604.01929)
- [代码仓库](https://github.com/SonyResearch/Woosh)
- [Demo 页面](https://sonyresearch.github.io/Woosh/)
- [PDF](https://arxiv.org/pdf/2604.01929.pdf)

---

## 2️⃣ T5Gemma-TTS Technical Report

**arXiv**: [2604.01760](https://arxiv.org/abs/2604.01760)  
**作者**: Chihiro Arata, Kiyoshi Kurihara  
**机构**: -  
**分类**: eess.AS  
**代码**: [GitHub - Aratako/T5Gemma-TTS](https://github.com/Aratako/T5Gemma-TTS)

### 📌 一句话总结

提出基于 T5Gemma 预训练编码器 - 解码器架构的 TTS 模型，通过交叉注意力维持持久文本条件，并引入进度监控旋转位置嵌入 (PM-RoPE) 改进时长控制，在多语言零样本声音克隆上取得 SOTA 性能。

### 💡 核心创新点

1. **编码器 - 解码器架构**: 区别于传统的仅解码器架构，通过交叉注意力在所有解码器层路由双向文本表示，维持持久文本条件，解决长语音生成中文本条件减弱的问题
2. **PM-RoPE 位置嵌入**: 在所有 26 个交叉注意力层引入进度监控旋转位置嵌入，注入归一化进度信号，帮助解码器跟踪目标语音长度
3. **无需音素转换**: 直接在子词级别处理文本，继承 T5Gemma 预训练的丰富语言知识

### 🔧 技术方法

- **架构**: 基于 T5Gemma 预训练编码器 - 解码器骨干网络 (2B 编码器 + 2B 解码器，共 4B 参数)
- **交叉注意力**: 所有解码器层使用交叉注意力维持文本条件
- **PM-RoPE**: 进度监控旋转位置嵌入，提供时长控制信号
- **训练数据**: 170,000 小时多语言语音 (英语、中文、日语)

### 📊 实验结果

- **日语说话人相似度**: 0.677 vs XTTSv2 的 0.622 (95% 置信区间不重叠，统计显著)
- **韩语说话人相似度**: 0.747 (韩语未包含在训练中，零样本泛化)
- **日语字符错误率 (CER)**: 0.126 (5 个基线中最低)
- **PM-RoPE 消融**: 推理时禁用 PM-RoPE 导致 CER 从 0.129 恶化到 0.982，时长准确率从 79% 下降到 46%

### 🤔 个人评价

T5Gemma-TTS 展示了编码器 - 解码器架构在 TTS 任务上的优势，特别是对于长语音生成。PM-RoPE 的设计非常巧妙，通过位置嵌入注入进度信息来解决时长控制问题。在韩语上的零样本泛化能力也令人印象深刻，尽管韩语未包含在训练数据中。

### 🔗 相关链接

- [arXiv 页面](https://arxiv.org/abs/2604.01760)
- [代码仓库](https://github.com/Aratako/T5Gemma-TTS)
- [PDF](https://arxiv.org/pdf/2604.01760.pdf)

---

## 3️⃣ OmniVoice: Towards Omnilingual Zero-Shot Text-to-Speech with Diffusion Language Models

**arXiv**: [2604.00688](https://arxiv.org/abs/2604.00688)  
**作者**: Han Zhu, Lingxuan Ye, Wei Kang, Zengwei Yao, Liyong Guo, Fangjun Kuang, Zhifeng Han, Weiji Zhuang, Long Lin, Daniel Povey  
**机构**: -  
**分类**: cs.CL, eess.AS  
**代码**: [GitHub - k2-fsa/OmniVoice](https://github.com/k2-fsa/OmniVoice)

### 📌 一句话总结

提出支持超过 600 种语言的大规模多语言零样本 TTS 模型 OmniVoice，基于新颖的扩散语言模型风格离散非自回归架构，直接使用预训练 LLM 初始化实现最优可懂度。

### 💡 核心创新点

1. **扩散语言模型架构**: 采用离散非自回归 (NAR) 架构，直接从文本映射到多码本声学 token，避免传统两阶段 (文本 - 语义 - 声学) 流程的性能瓶颈
2. **全码本随机掩码策略**: 提出高效的训练策略，通过全码本随机掩码实现快速收敛
3. **LLM 初始化**: 从预训练 LLM 初始化，确保卓越的可懂度和语言理解能力

### 🔧 技术方法

- **架构**: 扩散语言模型风格的离散非自回归架构
- **训练策略**: 全码本随机掩码，高效训练
- **初始化**: 从预训练 LLM 初始化模型权重
- **训练数据**: 581k 小时多语言数据集，完全来自开源数据

### 📊 实验结果

- **语言覆盖**: 支持超过 600 种语言，是目前语言覆盖最广的 TTS 模型
- **性能**: 在中文、英语和多样化多语言基准测试上达到 SOTA 性能
- **数据规模**: 使用 581k 小时开源多语言数据训练

### 🤔 个人评价

OmniVoice 在语言覆盖范围上实现了重大突破，600+ 语言的支持使其成为真正的全球性 TTS 模型。使用扩散语言模型架构直接生成声学 token 的设计避免了传统两阶段方法的误差累积问题。完全使用开源数据训练也体现了研究的透明度和可复现性。

### 🔗 相关链接

- [arXiv 页面](https://arxiv.org/abs/2604.00688)
- [代码仓库](https://github.com/k2-fsa/OmniVoice)
- [PDF](https://arxiv.org/pdf/2604.00688.pdf)

---

## 4️⃣ FastTurn: Unifying Acoustic and Streaming Semantic Cues for Low-Latency and Robust Turn Detection

**arXIV**: [2604.01897](https://arxiv.org/abs/2604.01897)  
**作者**: Chengyou Wang, Hongfei Xue, Chunjiang He, Jingbin Hu, Shuiyuan Wang, Bo Wu, Yuyu Ji, Jimeng Zheng, Ruofei Chen, Zhou Zhu, Lei Xie  
**机构**: -  
**分类**: cs.SD  
**代码**: -

### 📌 一句话总结

提出 FastTurn 统一框架，结合流式 CTC 解码与声学特征，实现低延迟和鲁棒的语音轮次检测，支持全双工对话系统的实时交互。

### 💡 核心创新点

1. **流式 CTC 解码 + 声学特征**: 结合流式 CTC 解码与声学特征，从部分观测中实现早期决策，同时保持语义线索
2. **真实对话测试集**: 发布基于真实人类对话的测试集，捕捉真实的轮次转换、重叠语音、回应、停顿、音高变化和环境噪声
3. **低延迟高准确率**: 相比代表性基线，实现更高的决策准确率和更低的中断延迟

### 🔧 技术方法

- **统一框架**: 同时利用声学线索和语义线索进行轮次检测
- **流式 CTC 解码**: 支持从部分观测中进行早期决策
- **真实数据测试集**: 包含真实交互动态的测试数据

### 📊 实验结果

- 相比基线方法实现更高的决策准确率
- 更低的中断延迟
- 在挑战性声学条件下保持鲁棒性

### 🤔 个人评价

FastTurn 解决了全双工对话系统中的关键问题——轮次检测。现有方法要么依赖缺乏语义理解的语音活动检测，要么依赖引入延迟的 ASR 模块。FastTurn 的统一框架在延迟和性能之间取得了良好平衡。发布的真实对话测试集也将促进该领域的研究。

### 🔗 相关链接

- [arXiv 页面](https://arxiv.org/abs/2604.01897)
- [PDF](https://arxiv.org/pdf/2604.01897.pdf)

---

## 5️⃣ Diff-VS: Efficient Audio-Aware Diffusion U-Net for Vocals Separation

**arXiv**: [2604.01120](https://arxiv.org/abs/2604.01120)  
**作者**: Yun-Ning Hung, Richard Vogl, Filip Korzeniowski, Igor Pereira  
**机构**: -  
**分类**: eess.AS  
**接收**: ICASSP 2026

### 📌 一句话总结

提出基于 Elucidated Diffusion Model (EDM) 框架的新型生成式人声分离模型，在客观指标上匹配判别式基线，在感知质量上达到 SOTA 水平。

### 💡 核心创新点

1. **EDM 框架的人声分离**: 将 Elucidated Diffusion Model 框架应用于音乐源分离任务
2. **改进的 U-Net 架构**: 基于音乐信息设计选择，处理复数短时傅里叶变换频谱图
3. **生成式方法的新突破**: 解决当前生成式音乐源分离方法在标准客观指标上表现不佳的问题

### 🔧 技术方法

- **架构**: 基于 EDM 框架的扩散 U-Net
- **输入**: 复数 STFT 频谱图
- **设计**: 音乐信息驱动的网络架构选择

### 📊 实验结果

- 客观指标上匹配判别式基线
- 感知质量与 SOTA 系统相当 (通过代理主观指标评估)
- ICASSP 2026 接收

### 🤔 个人评价

Diff-VS 展示了扩散模型在音频源分离任务上的潜力。传统上，生成式方法在客观指标上往往落后于判别式方法，但这项工作通过精心设计的架构和训练策略实现了两者的平衡。ICASSP 2026 的接收也证明了这项工作的重要性。

### 🔗 相关链接

- [arXiv 页面](https://arxiv.org/abs/2604.01120)
- [PDF](https://arxiv.org/pdf/2604.01120.pdf)

---

## 📊 今日统计

| 指标 | 数值 |
|------|------|
| 搜索论文总数 | ~112 篇 |
| 过去 48 小时论文 | 23 篇 |
| 筛选后推荐 | 5 篇 |
| 主要领域 | cs.SD, eess.AS, cs.CL, cs.AI |
| 重点方向 | TTS, Audio Generation, Diffusion Models, Sound Effects |

---

## 🔍 搜索配置

### 搜索分类
- **cs.CL** - 计算语言学
- **cs.SD** - 语音
- **cs.AI** - 人工智能
- **cs.LG** - 机器学习
- **eess.AS** - 音频与语音处理

### 主要关键词
text-to-speech, TTS, speech synthesis, text-to-audio, audio generation, diffusion model, generative model, voice synthesis, neural vocoder

### 筛选标准
- 🏛️ 知名机构 (Sony AI, 等)
- 🔥 热门方向 (TTS, Diffusion, Zero-Shot, Generative)
- 💻 代码可用 (优先)
- 📈 接收会议/期刊 (ICASSP 2026, 等)

---

## 🔗 相关链接

- [GitHub 仓库](https://github.com/junxi25liu/daily-arxiv-digest)
- [arXiv 今日论文](https://arxiv.org/list/recent)

---

**Generated by**: Daily arXiv Digest Skill  
**License**: MIT
