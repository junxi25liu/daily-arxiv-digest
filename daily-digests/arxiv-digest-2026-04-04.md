# Daily arXiv Digest - 2026-04-04

> Text-to-Audio, Text-to-Speech & Generative Model

**Date**: 2026-04-04  
**Papers Recommended**: 4  
**Search Categories**: cs.CL, cs.SD, cs.AI, cs.LG, eess.AS  
**Time Range**: Past 48 hours (April 2-4, 2026)

---

## 📋 今日论文概览

| # | arXiv ID | 标题 | 机构 | 方向 |
|---|----------|------|------|------|
| 1️⃣ | 2604.01832 | GAP-URGENet: Generative-Predictive Fusion for Speech Enhancement | - | 语音增强，生成式模型 |
| 2️⃣ | 2604.02045 | BidirLM: From Text to Omnimodal Bidirectional Encoders | - | 多模态编码器，LLM 适配 |
| 3️⃣ | 2604.02102 | Prosodic ABX: Language-Agnostic Prosodic Contrast Measurement | University of Tokyo | 韵律评估，自监督学习 |
| 4️⃣ | 2604.01590 | PhiNet: Speaker Verification with Phonetic Interpretability | - | 说话人验证，可解释性 |

---

## 📄 详细摘要

### 1️⃣ GAP-URGENet: A Generative-Predictive Fusion Framework for Universal Speech Enhancement

**arXiv**: [2604.01832](https://arxiv.org/abs/2604.01832)  
**作者**: Xiaobin Rong, Yushi Wang, Zheng Wang, Jing Lu  
**机构**: -  
**分类**: eess.AS, cs.SD  
**PDF**: [下载](https://arxiv.org/pdf/2604.01832.pdf)  
**代码/演示**: [https://xiaobin-rong.github.io/gap-urgenet_demo/](https://xiaobin-rong.github.io/gap-urgenet_demo/)

> **一句话总结**: 提出生成 - 预测融合框架 GAP-URGENet，结合自监督表示域的全栈语音修复和频谱图域增强，在 ICASSP 2026 URGENT Challenge 中取得目标评估第 1 名。

**核心创新点**:
- ✅ **生成 - 预测双分支架构**: 生成分支在自监督表示域执行全栈语音修复，预测分支在频谱图域进行增强，两者互补
- ✅ **神经声码器重建**: 生成分支通过神经声码器从自监督表示重建波形，保持高质量语音
- ✅ **后处理融合模块**: 融合双分支输出并执行带宽扩展，生成 48kHz 增强波形
- ✅ **盲测性能优异**: 在 ICASSP 2026 URGENT Challenge 盲测阶段取得顶级性能，目标评估排名第 1

**技术方法详解**:
1. **生成分支**: 使用自监督语音表示模型提取特征，在表示域进行去噪和修复，然后通过神经声码器（如 HiFi-GAN）重建波形
2. **预测分支**: 传统频谱图域增强方法，提供互补的增强线索
3. **融合模块**: 学习加权融合双分支输出，同时执行带宽扩展（从低采样率到 48kHz）
4. **后处理**: 将 48kHz 波形下采样到原始采样率，保持兼容性

**实验结果摘要**:
- ICASSP 2026 URGENT Challenge Track 1 目标评估排名第 1
- 盲测阶段取得顶级性能
- 生成 - 预测融合显著提升鲁棒性和感知质量
- 音频示例可在项目页面查看

**相关链接**:
- 📄 [arXiv 论文](https://arxiv.org/abs/2604.01832)
- 📥 [PDF 下载](https://arxiv.org/pdf/2604.01832.pdf)
- 🔗 [项目页面与音频示例](https://xiaobin-rong.github.io/gap-urgenet_demo/)

---

### 2️⃣ BidirLM: From Text to Omnimodal Bidirectional Encoders by Adapting and Composing Causal LLMs

**arXiv**: [2604.02045](https://arxiv.org/abs/2604.02045)  
**作者**: Nicolas Boizard, Théo Deschamps-Berger, Hippolyte Gisserot-Boukhlef, Céline Hudelot, Pierre Colombo  
**机构**: -  
**分类**: cs.CL, cs.AI  
**PDF**: [下载](https://arxiv.org/pdf/2604.02045.pdf)

> **一句话总结**: 提出将因果生成式 LLM 转换为双向编码器的系统化方法，通过权重合并和轻量数据混合避免灾难性遗忘，生成在文本、视觉和音频基准上超越替代方案的 BidirLM 编码器家族。

**核心创新点**:
- ✅ **先验掩码阶段**: 识别出常被忽略的先验掩码（prior masking）阶段对成功适配至关重要
- ✅ **线性权重合并**: 无需原始预训练数据，通过线性权重合并扩展适配过程
- ✅ **轻量多域数据混合**: 缓解灾难性遗忘，保持通用能力
- ✅ **专业化模型组合**: 通过将编码器与专业化因果模型合并，无缝转移模态和领域特定能力
- ✅ **开源方案**: 适用于任何因果解码器 LLM 的开放源码方案

**技术方法详解**:
1. **系统消融研究**: 在 Gemma3 和 Qwen3 家族上进行系统消融，识别成功适配的关键因素
2. **先验掩码**: 在适配前对模型进行掩码训练，为双向注意力做准备
3. **权重合并策略**: 使用线性插值合并原始 LLM 权重和适配后权重，避免完全遗忘
4. **多域数据混合**: 使用轻量级多领域数据集（文本、视觉、音频）进行微调
5. **模型组合**: 将适配后的编码器与专业化因果模型（如视觉、音频模型）合并，转移特定能力

**实验结果摘要**:
- 生成 5 个 BidirLM 编码器变体
- 在文本、视觉和音频表示基准上超越替代方案
- 保持与原始 LLM 相当的通用能力
- 成功转移视觉和音频模态的 specialized 能力

**相关链接**:
- 📄 [arXiv 论文](https://arxiv.org/abs/2604.02045)
- 📥 [PDF 下载](https://arxiv.org/pdf/2604.02045.pdf)

---

### 3️⃣ Prosodic ABX: A Language-Agnostic Method for Measuring Prosodic Contrast in Speech Representations

**arXiv**: [2604.02102](https://arxiv.org/abs/2604.02102)  
**作者**: Haitong Sun, Stephen McIntosh, Kwanghee Choi, Eunjung Yeo, Daisuke Saito, Nobuaki Minematsu  
**机构**: University of Tokyo (部分作者)  
**分类**: cs.CL, cs.LG, cs.SD, eess.AS  
**PDF**: [下载](https://arxiv.org/pdf/2604.02102.pdf)

> **一句话总结**: 提出 prosodic ABX 判别任务，扩展经典 ABX 框架以评估自监督语音模型对韵律对比的敏感性，仅需少量示例且无需显式标注，发布英语和日语最小对数据集。

**核心创新点**:
- ✅ **韵律 ABX 任务**: 首次将 ABX 判别任务扩展到韵律对比评估，仅需少量示例
- ✅ **语言无关方法**: 无需显式韵律标注，适用于低资源语言
- ✅ **多语言数据集**: 构建并发布英语和日语韵律最小对数据集，配合中文数据集进行评估
- ✅ **跨条件稳定性**: 模型和层级排序在多种实验条件下保持一致，适合低资源场景

**技术方法详解**:
1. **ABX 任务扩展**: 经典 ABX 任务通过最小对测量音素对比，本工作扩展到韵律对比（如重音、声调、音调）
2. **最小对构建**: 收集仅在韵律特征上不同的语音对（如英语重音、日语音高重音、中文声调）
3. **表示提取**: 从自监督语音模型（如 Wav2Vec 2.0, HuBERT）提取不同层级的表示
4. **距离度量**: 计算 A-X 和 B-X 的距离，判断模型是否能区分韵律对比
5. **跨语言评估**: 在英语、日语和中文数据集上评估多个模型

**实验结果摘要**:
- 评估多个自监督语音模型（Wav2Vec 2.0, HuBERT, WavLM 等）
- 发现模型和层级排序在多种实验条件下保持稳定
- 某些模型层级对韵律对比特别敏感
- 发布英语和日语最小对数据集，促进后续研究

**相关链接**:
- 📄 [arXiv 论文](https://arxiv.org/abs/2604.02102)
- 📥 [PDF 下载](https://arxiv.org/pdf/2604.02102.pdf)

---

### 4️⃣ PhiNet: Speaker Verification with Phonetic Interpretability

**arXiv**: [2604.01590](https://arxiv.org/abs/2604.01590)  
**作者**: Yi Ma, Shuai Wang, Tianchi Liu, Haizhou Li  
**机构**: -  
**分类**: eess.AS, cs.SD  
**PDF**: [下载](https://arxiv.org/pdf/2604.01590.pdf)

> **一句话总结**: 提出具有音素可解释性的说话人验证网络 PhiNet，通过利用音素证据增强决策透明度，在 VoxCeleb、SITW 和 LibriSpeech 基准上取得与传统黑盒模型相当的性能，同时提供有意义的解释。

**核心创新点**:
- ✅ **音素级可解释性**: 提供详细的音素级比较，使用户能够手动检查说话人特定特征
- ✅ **法医说话人对比启发**: 模仿人类专家进行法医说话人对比（FSC）的方式
- ✅ **双重可解释性**: 同时增强局部（音素级）和全局（决策级）可解释性
- ✅ **性能不妥协**: 在多个基准上取得与传统黑盒 ASV 模型相当的性能

**技术方法详解**:
1. **音素证据提取**: 从输入语音中提取音素级特征，作为说话人对比的证据
2. **可解释性模块**: 设计专门模块生成音素级对比可视化，显示哪些音素对决策贡献最大
3. **决策透明度**: 为每个验证决策提供明确的推理链，显示基于哪些音素特征做出判断
4. **误差追踪**: 开发者可利用可解释性简化误差分析，指导超参数选择

**实验结果摘要**:
- 在 VoxCeleb、SITW、LibriSpeech 等多个基准上评估
- 性能与传统黑盒 ASV 模型相当
- 提供有意义的可解释性输出
- 展示在分析超参数影响等实际应用中的价值
- 弥合 ASV 与法医分析之间的差距

**相关链接**:
- 📄 [arXiv 论文](https://arxiv.org/abs/2604.01590)
- 📥 [PDF 下载](https://arxiv.org/pdf/2604.01590.pdf)

---

## 📊 今日统计

| 指标 | 数值 |
|------|------|
| 检索论文总数 | ~80 篇 |
| 过去 48 小时论文 | 11 篇 (新论文，未在前几日摘要中) |
| 筛选推荐 | 4 篇 |
| 搜索分类 | cs.CL, cs.SD, cs.AI, cs.LG, eess.AS |
| 搜索方向 | TTS, Speech Synthesis, Audio Generation, Generative Models, Speech Enhancement |

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
4. **Speech Enhancement** - 语音增强
5. **Speech Representation** - 语音表示学习

### 关键词
text-to-audio, text to audio, text-to-speech, text to speech, TTS, speech synthesis, audio generation, generative model, generative models, diffusion model, speech enhancement, speaker verification

### 筛选标准
- 🏛️ 知名机构 (MIT, Stanford, Google, Meta, Sony AI, University of Tokyo, 等)
- 👨‍🔬 高影响力作者 (h-index > 15)
- 🔥 热门方向 (LLM, Diffusion, Zero-Shot, Generative, Multimodal, 等)
- 💻 代码可用 (优先)

---

**Generated by**: daily-arxiv-digest skill  
**Last Updated**: 2026-04-04 09:00 (Asia/Shanghai)
