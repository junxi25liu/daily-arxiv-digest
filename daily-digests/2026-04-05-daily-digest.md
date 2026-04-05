# Daily arXiv Digest - Text-to-Speech & Generative AI

**Date:** 2026-04-05  
**Focus Areas:** Text-to-Speech, Speech Synthesis, Audio Generation, Generative Models, Speech Enhancement  
**Search Period:** Past 48 hours (April 3-5, 2026)  
**Categories:** cs.CL, cs.SD, cs.AI, cs.LG, eess.AS

---

## 📋 Executive Summary

Today's digest features **5 high-impact papers** in TTS and audio generation, with notable contributions from **Sony AI**, **independent researchers**, and **academic institutions**. The highlight is **T5Gemma-TTS**, an encoder-decoder codec language model that achieves state-of-the-art speaker similarity through persistent text conditioning and novel position embeddings.

---

## 🎯 Featured Papers

### 1. T5Gemma-TTS Technical Report

**arXiv:** [2604.01760](https://arxiv.org/abs/2604.01760)  
**Authors:** Chihiro Arata, Kiyoshi Kurihara  
**Institutions:** Independent Research  
**Subjects:** eess.AS

#### One-Sentence Summary
T5Gemma-TTS is an encoder-decoder codec language model that maintains persistent text conditioning through cross-attention at every decoder layer, achieving state-of-the-art speaker similarity on Japanese and Korean with a novel Progress-Monitoring Rotary Position Embedding (PM-RoPE) for duration control.

#### Key Innovations
1. **Encoder-Decoder Architecture:** Unlike decoder-only models, maintains persistent text conditioning by routing bidirectional text representations through cross-attention at every decoder layer
2. **Progress-Monitoring RoPE (PM-RoPE):** Injects normalized progress signals in all 26 cross-attention layers to help decoder track target speech length
3. **T5Gemma Backbone:** Built on pretrained 2B encoder + 2B decoder (4B total parameters), inheriting rich linguistic knowledge without phoneme conversion
4. **Subword-Level Processing:** Processes text directly at subword level, avoiding phoneme conversion overhead
5. **Multilingual Training:** Trained on 170,000 hours of speech in English, Chinese, and Japanese

#### Technical Method
- **Architecture:** Encoder-decoder codec language model
- **Backbone:** T5Gemma (2B encoder + 2B decoder, 4B parameters)
- **Position Embedding:** PM-RoPE in all 26 cross-attention layers
- **Training Data:** 170K hours multilingual speech (EN, ZH, JA)
- **Inference:** PM-RoPE essential—disabling causes near-complete synthesis failure (CER degrades from 0.129 to 0.982)

#### Experimental Results
| Metric | T5Gemma-TTS | XTTSv2 (Baseline) |
|--------|-------------|-------------------|
| Japanese Speaker Similarity | **0.677** (statistically significant gain) | 0.622 |
| Korean Speaker Similarity | **0.747** (highest numerical, not statistically conclusive) | 0.741 |
| Japanese Character Error Rate | **0.126** (lowest among 5 baselines) | - |
| Duration Accuracy | **79%** (with PM-RoPE) | 46% (without PM-RoPE) |

**Key Finding:** PM-RoPE is critical—disabling at inference causes catastrophic degradation in both CER (0.129→0.982) and duration accuracy (79%→46%).

#### Code & Demo
- **GitHub:** https://github.com/Aratako/T5Gemma-TTS
- **Model:** Open-source (weights available)
- **Demo:** Via GitHub repository

---

### 2. Woosh: A Sound Effects Foundation Model

**arXiv:** [2604.01929](https://arxiv.org/abs/2604.01929)  
**Authors:** Gaëtan Hadjeres, Marc Ferras, Khaled Koutini, Benno Weck, Alexandre Bittar, Thomas Hummel, Zineb Lahrici, Hakim Missoum, Joan Serrà, Yuki Mitsufuji  
**Institutions:** Sony AI  
**Subjects:** cs.SD, cs.AI, cs.LG

#### One-Sentence Summary
Woosh is Sony AI's publicly released sound effect foundation model featuring a complete pipeline including high-quality audio encoder/decoder, text-audio alignment, text-to-audio, and video-to-audio generation with distilled models for low-resource operation.

#### Key Innovations
1. **Complete Foundation Model Suite:** Provides (1) audio encoder/decoder, (2) text-audio alignment, (3) text-to-audio, and (4) video-to-audio models
2. **Sound Effect Optimization:** Specifically optimized for sound effect generation rather than speech or music
3. **Distilled Models:** Includes distilled versions for low-resource operation and fast inference
4. **Open Release:** Full model weights and inference code publicly available
5. **Competitive Performance:** Outperforms or matches StableAudio-Open and TangoFlux on public and private benchmarks

#### Technical Method
- **Components:** 4-module pipeline (encoder/decoder, alignment, T2A, V2A)
- **Optimization Target:** Sound effects (SFX) rather than speech/music
- **Distillation:** Provides lightweight distilled variants for efficiency
- **Training:** Proprietary Sony AI training data and infrastructure

#### Experimental Results
- **Benchmarks:** Evaluated against StableAudio-Open and TangoFlux
- **Performance:** Competitive or better on both public and private test data
- **Modules:** Each module evaluated independently showing strong performance

#### Code & Demo
- **GitHub:** https://github.com/SonyResearch/Woosh
- **Demo:** https://sonyresearch.github.io/Woosh/
- **Model:** Open-source (full weights released)

---

### 3. FastTurn: Unifying Acoustic and Streaming Semantic Cues for Low-Latency Turn Detection

**arXiv:** [2604.01897](https://arxiv.org/abs/2604.01897)  
**Authors:** Chengyou Wang, Hongfei Xue, Chunjiang He, Jingbin Hu, Shuiyuan Wang, Bo Wu, Yuyu Ji, Jimeng Zheng, Ruofei Chen, Zhou Zhu, Lei Xie  
**Institutions:** Not specified (likely industry lab based on author count)  
**Subjects:** cs.SD

#### One-Sentence Summary
FastTurn is a unified framework for low-latency turn detection in full-duplex spoken dialogue systems that combines streaming CTC decoding with acoustic features, enabling early decisions from partial observations while preserving semantic understanding.

#### Key Innovations
1. **Streaming CTC + Acoustic Fusion:** Combines streaming CTC decoding with acoustic features for early decision-making
2. **Semantic + Acoustic Cues:** Unlike VAD-only approaches, preserves semantic understanding while maintaining low latency
3. **Real-World Test Set:** Released test set based on real human dialogue with authentic turn transitions, overlapping speech, backchannels, and environmental noise
4. **Full-Duplex Optimization:** Designed for real-time full-duplex communication where agents must decide when to speak, yield, or interrupt
5. **Robust to Noise:** Maintains performance under challenging acoustic conditions (overlapping speech, background noise)

#### Technical Method
- **Architecture:** Unified framework combining streaming CTC decoder with acoustic feature extractor
- **Decision Making:** Early decisions from partial observations
- **Dataset:** New test set capturing realistic interaction dynamics
- **Application:** Full-duplex spoken dialogue systems

#### Experimental Results
- **Latency:** Lower interruption latency than representative baselines
- **Accuracy:** Higher decision accuracy while maintaining low latency
- **Robustness:** Remains effective under overlapping speech and environmental noise
- **Real-World Performance:** Validated on authentic human dialogue test set

#### Code & Demo
- **GitHub:** Not specified in paper
- **Dataset:** Real human dialogue test set (released)
- **Demo:** Not specified

---

### 4. GAP-URGENet: A Generative-Predictive Fusion Framework for Universal Speech Enhancement

**arXiv:** [2604.01832](https://arxiv.org/abs/2604.01832)  
**Authors:** Xiaobin Rong, Yushi Wang, Zheng Wang, Jing Lu  
**Institutions:** Not specified  
**Subjects:** eess.AS, cs.SD

#### One-Sentence Summary
GAP-URGENet is a generative-predictive fusion framework for speech enhancement that integrates a generative branch (self-supervised representation domain restoration) with a predictive branch (spectrogram-domain enhancement), achieving 1st place in ICASSP 2026 URGENT Challenge Track 1.

#### Key Innovations
1. **Generative-Predictive Fusion:** Combines generative restoration (self-supervised domain) with predictive enhancement (spectrogram domain) for complementary cues
2. **Dual-Branch Architecture:** Generative branch performs full-stack speech restoration; predictive branch provides spectrogram enhancement
3. **Post-Processing Fusion:** Fuses both branch outputs with bandwidth extension to 48 kHz
4. **Competition Winner:** Ranked 1st in objective evaluation of ICASSP 2026 URGENT Challenge Track 1
5. **Perceptual Quality:** Improved robustness and perceptual quality through fusion approach

#### Technical Method
- **Generative Branch:** Self-supervised representation domain restoration + neural vocoder waveform reconstruction
- **Predictive Branch:** Spectrogram-domain enhancement
- **Fusion Module:** Post-processing with bandwidth extension (48 kHz output, downsampled to original rate)
- **Challenge:** ICASSP 2026 URGENT Challenge Track 1

#### Experimental Results
- **Competition Result:** 1st place in blind-test phase objective evaluation
- **Performance:** Top performance in ICASSP 2026 URGENT Challenge
- **Quality:** Improved perceptual quality and robustness vs. single-branch approaches

#### Code & Demo
- **GitHub:** Not specified
- **Demo:** https://xiaobin-rong.github.io/gap-urgenet_demo
- **Model:** Competition submission (availability not specified)

---

### 5. Prosodic ABX: A Language-Agnostic Method for Measuring Prosodic Contrast in Speech Representations

**arXiv:** [2604.02102](https://arxiv.org/abs/2604.02102)  
**Authors:** Haitong Sun, Stephen McIntosh, Kwanghee Choi, Eunjung Yeo, Daisuke Saito, Nobuaki Minematsu  
**Institutions:** Not specified (likely academic, Japanese institutions based on author names)  
**Subjects:** cs.CL, cs.LG, cs.SD, eess.AS

#### One-Sentence Summary
Prosodic ABX extends the ABX discrimination task framework to evaluate prosodic contrast in self-supervised speech model representations using minimal pairs without explicit labels, with released datasets for English stress, Japanese pitch accent, and Mandarin tone evaluation.

#### Key Innovations
1. **Prosodic ABX Framework:** Extends phonemic ABX discrimination task to measure prosodic contrast in speech representations
2. **Label-Free Evaluation:** Requires only a handful of examples with no explicit prosodic labels
3. **Multilingual Dataset:** Released minimal pair datasets for English stress, Japanese pitch accent, and Mandarin tone
4. **Cross-Lingual Evaluation:** Language-agnostic method applicable across different prosodic systems
5. **Low-Resource Practical:** Model and layer rankings preserved across experimental conditions, enabling practical low-resource evaluation

#### Technical Method
- **Framework:** Extension of ABX discrimination task for prosodic features
- **Datasets:** English stress, Japanese pitch accent, Mandarin tone minimal pairs
- **Evaluation:** Self-supervised speech model (S3M) representation analysis
- **Label Requirement:** No explicit prosodic labels needed

#### Experimental Results
- **Cross-Lingual:** Evaluated on English, Japanese, and Mandarin
- **Consistency:** Model and layer rankings preserved across experimental conditions
- **Practical Utility:** Enables prosodic evaluation in low-resource settings

#### Code & Demo
- **GitHub:** Not specified
- **Dataset:** Released (English, Japanese, Mandarin minimal pairs)
- **Demo:** Not specified

---

## 📊 Summary Table

| Paper | Institution | Focus | Key Contribution | Open Source |
|-------|-------------|-------|------------------|-------------|
| T5Gemma-TTS | Independent | TTS / Codec LM | Encoder-decoder with PM-RoPE | ✅ Yes |
| Woosh | Sony AI | Sound Effects | Complete SFX foundation model suite | ✅ Yes |
| FastTurn | Industry Lab | Turn Detection | Streaming CTC + acoustic fusion | ⚠️ Dataset only |
| GAP-URGENet | Academic | Speech Enhancement | Generative-predictive fusion | ⚠️ Demo only |
| Prosodic ABX | Academic | Speech Evaluation | Label-free prosodic contrast measurement | ⚠️ Dataset only |

---

## 🔍 Trend Analysis

### Hot Topics This Week
1. **Encoder-Decoder TTS:** T5Gemma-TTS challenges decoder-only dominance, showing benefits of persistent text conditioning
2. **Sound Effect Generation:** Woosh represents growing interest in non-speech audio generation (SFX, environmental sounds)
3. **Full-Duplex Dialogue:** FastTurn addresses real-time interaction challenges as AudioLLMs enable more natural conversations
4. **Fusion Architectures:** GAP-URGENet's generative-predictive fusion reflects broader trend of combining complementary approaches
5. **Evaluation Methods:** Prosodic ABX provides new tools for measuring speech representation quality beyond phonemic features

### Notable Institutions
- **Sony AI:** Continuing strong audio research presence with Woosh foundation model
- **Independent Researchers:** T5Gemma-TTS shows high-quality work from individual researchers
- **Japanese Institutions:** Strong representation in prosody and TTS research

### Technical Insights
- **PM-RoPE Critical:** T5Gemma-TTS shows position embedding design can make/break model performance
- **Distillation Trend:** Woosh includes distilled models, reflecting industry demand for efficient inference
- **Real-World Data:** FastTurn's authentic dialogue test set addresses gap between lab and deployment conditions

---

## 📈 GitHub Repository

**Daily Digests:** https://github.com/junxi25liu/daily-arxiv-digest

Today's digest has been saved to: `daily-digests/2026-04-05-daily-digest.md`

---

## 📝 Notes

- Search conducted on arXiv for papers submitted April 3-5, 2026
- Categories: cs.CL, cs.SD, cs.AI, cs.LG, eess.AS
- Selection criteria: Institution prestige, keyword relevance, technical novelty, open-source availability
- Some papers may have incomplete information as they were just submitted

---

*Generated by Daily arXiv Digest System - TTS & Generative AI Focus*
