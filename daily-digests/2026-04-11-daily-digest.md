# Daily arXiv Digest - 2026-04-11

**Date**: April 11, 2026 (Saturday)  
**Focus Areas**: Text-to-Speech, Audio Generation, Generative Models, Text-to-Audio-Video  
**Time Range**: Past 48 hours (April 9-11, 2026)  
**Total Papers Selected**: 4

---

## 📄 Paper 1: AVGen-Bench: A Task-Driven Benchmark for Multi-Granular Evaluation of Text-to-Audio-Video Generation

**arXiv**: [2604.08540](https://arxiv.org/abs/2604.08540)  
**PDF**: [https://arxiv.org/pdf/2604.08540](https://arxiv.org/pdf/2604.08540)  
**Authors**: Ziwei Zhou, Zeyuan Lai, Rui Wang, Yifan Yang, Zhen Xing, Yuqing Yang, Qi Dai, Lili Qiu, Chong Luo  
**Institution**: Microsoft Research  
**Categories**: cs.CV, cs.AI, cs.CL  
**Published**: April 9, 2026  
**Code/Resources**: [http://aka.ms/avgenbench](http://aka.ms/avgenbench)

### 📝 One-Sentence Summary

AVGen-Bench introduces the first task-driven benchmark for Text-to-Audio-Video (T2AV) generation with 11 real-world categories and a multi-granular evaluation framework combining specialist models with MLLMs, revealing a significant gap between audio-visual aesthetics and semantic reliability in current T2AV systems.

### ✨ Core Innovations (3-5 points)

- **Task-Driven Benchmark Design**: Features high-quality prompts across 11 real-world categories, moving beyond isolated audio/video evaluation to capture fine-grained joint correctness required by realistic prompts
- **Multi-Granular Evaluation Framework**: Combines lightweight specialist models with Multimodal Large Language Models (MLLMs) to enable evaluation from perceptual quality to fine-grained semantic controllability
- **Comprehensive Failure Mode Analysis**: Reveals persistent failures in text rendering, speech coherence, physical reasoning, and a universal breakdown in musical pitch control across current T2AV systems
- **Aesthetic-Semantic Gap Discovery**: Exposes a pronounced gap between strong audio-visual aesthetics and weak semantic reliability, highlighting a critical challenge for the field

### 🔬 Technical Method Details

**Evaluation Framework Architecture**:
1. **Specialist Models Layer**: Lightweight models for specific quality metrics (perceptual quality, audio-video synchronization, technical artifacts)
2. **MLLM Layer**: Multimodal Large Language Models for fine-grained semantic evaluation and controllability assessment
3. **Task-Driven Prompts**: 11 real-world categories designed to test practical T2AV generation capabilities

**Key Evaluation Dimensions**:
- Perceptual quality (audio and video separately)
- Audio-video synchronization
- Semantic correctness (joint audio-video understanding)
- Text rendering accuracy
- Speech coherence
- Physical reasoning
- Musical pitch control

**Benchmark Categories**: 11 real-world categories covering diverse T2AV use cases (specific categories detailed in full paper)

### 📊 Experimental Results Summary

**Key Findings**:
- **Aesthetic-Semantic Gap**: Current T2AV models achieve strong audio-visual aesthetics but fail significantly on semantic reliability tasks
- **Text Rendering**: Persistent failures in generating correct text within video content
- **Speech Coherence**: Models struggle to maintain coherent speech patterns in generated audio
- **Physical Reasoning**: Significant gaps in understanding and representing physical interactions
- **Musical Pitch Control**: Universal breakdown observed across all evaluated models - no model successfully maintains accurate musical pitch

**Implications**: The benchmark reveals that while T2AV generation has made progress in surface-level quality, fundamental semantic understanding and controllability remain major challenges requiring focused research attention.

---

## 📄 Paper 2: CapTalk: Unified Voice Design for Single-Utterance and Dialogue Speech Generation

**arXiv**: [2604.08363](https://arxiv.org/abs/2604.08363)  
**PDF**: [https://arxiv.org/pdf/2604.08363](https://arxiv.org/pdf/2604.08363)  
**Authors**: Xiaosu Su, Zihan Sun, Peilei Jia, Jun Gao  
**Institution**: Academic  
**Categories**: cs.SD, cs.AI  
**Published**: April 9, 2026  
**Audio Samples**: [https://anonymous.4open.science/api/repo/Captalk-D601/file/index.html](https://anonymous.4open.science/api/repo/Captalk-D601/file/index.html)

### 📝 One-Sentence Summary

CapTalk proposes the first unified caption-conditioned text-audio autoregressive framework for both single-utterance and dialogue voice design, extending voice design from natural language descriptions to conversational settings with turn-level expressive control.

### ✨ Core Innovations (3-5 points)

- **Dialogue Voice Design Extension**: First work to extend voice design from single-utterance generation to multi-turn dialogue settings, enabling better target speaker modeling and turn-level expressive control
- **Unified Caption-Conditioned Framework**: Uses utterance-level captions for single-utterance voice design and speaker-level captions for dialogue speaker modeling within a single architecture
- **CoT Control Sequence**: Introduces Chain-of-Thought control sequences in dialogue to explicitly plan turn-level dynamic attributes
- **Hierarchical Variational Conditioning Module**: Novel module with utterance-level speaker encoder that balances stable timbre preservation with context-adaptive expression
- **Comprehensive Evaluation Protocol**: First evaluation protocol covering both single-utterance and dialogue voice design settings

### 🔬 Technical Method Details

**Architecture Components**:

1. **Caption-Conditioned Text-Audio Autoregressive Framework**:
   - Accepts natural language descriptions as input (no reference audio required)
   - Generates speech with target timbre and speaking style
   - Unified architecture handles both single-utterance and dialogue modes

2. **Caption Strategy**:
   - **Single-Utterance Mode**: Uses utterance-level captions describing target voice characteristics
   - **Dialogue Mode**: Uses speaker-level captions for consistent speaker modeling across turns

3. **CoT Control Sequence**:
   - Explicitly plans turn-level dynamic attributes (emotion, emphasis, pacing)
   - Enables fine-grained control over expressive variations in dialogue

4. **Hierarchical Variational Conditioning Module**:
   - **Utterance-Level Speaker Encoder**: Extracts stable timbre representations
   - **Variational Conditioning**: Balances timbre stability with expression adaptivity
   - **Context Integration**: Incorporates surrounding dialogue context for appropriate expression

**Training Strategy**:
- Multi-task learning across single-utterance and dialogue scenarios
- Joint optimization of timbre preservation and expression adaptation objectives

### 📊 Experimental Results Summary

**Single-Utterance Voice Design**:
- Achieves **state-of-the-art performance** on single-utterance voice design benchmark
- Outperforms reference-audio-based methods in timbre accuracy and naturalness

**Dialogue Voice Design**:
- **Better Expression Controllability**: More precise control over turn-level emotional and prosodic variations
- **Improved Contextual Appropriateness**: Expressions better match dialogue context and conversational flow
- **Timbre Consistency**: Maintains stable speaker identity across multiple turns while adapting expression

**Key Metrics**:
- MOS (Mean Opinion Score): Significant improvements over baselines
- Speaker Similarity: High consistency across dialogue turns
- Expression Appropriateness: Better alignment with intended emotional states

---

## 📄 Paper 3: A Novel Automatic Framework for Speaker Drift Detection in Synthesized Speech

**arXiv**: [2604.06327](https://arxiv.org/abs/2604.06327)  
**PDF**: [https://arxiv.org/pdf/2604.06327](https://arxiv.org/pdf/2604.06327)  
**Authors**: Jia-Hong Huang, Seulgi Kim, Yi Chieh Liu, Yixian Shen, Hongyi Zhu, Prayag Tiwari, Stevan Rudinac, Evangelos Kanoulas  
**Institution**: Academic  
**Categories**: cs.SD, cs.AI  
**Published**: April 7, 2026  
**Conference**: IEEE ICASSP 2026 (Accepted)

### 📝 One-Sentence Summary

This work introduces the first automatic framework for detecting speaker drift in diffusion-based TTS by formulating it as a binary classification task over utterance-level speaker consistency, combining cosine similarity analysis with LLM-based perceptual reasoning.

### ✨ Core Innovations (3-5 points)

- **First Automatic Speaker Drift Detection Framework**: Addresses the underexplored problem of speaker drift - subtle, gradual shifts in perceived speaker identity within a single utterance in diffusion-based TTS
- **Binary Classification Formulation**: Formulates speaker drift detection as utterance-level speaker consistency classification task
- **Cosine Similarity Analysis**: Computes cosine similarity across overlapping segments of synthesized speech with theoretical guarantees for cosine-based drift detection
- **LLM-Based Perceptual Reasoning**: Prompts large language models with structured speaker embedding representations to assess drift perceptually
- **Geometric Clustering Discovery**: Demonstrates that speaker embeddings exhibit meaningful geometric clustering on the unit sphere
- **Human-Validated Benchmark**: Constructs high-quality synthetic benchmark with human-validated speaker drift annotations for evaluation

### 🔬 Technical Method Details

**Detection Pipeline**:

1. **Segment Extraction**:
   - Divides synthesized speech utterance into overlapping segments
   - Ensures temporal coverage for drift detection across entire utterance

2. **Speaker Embedding Computation**:
   - Extracts speaker embeddings for each segment using pre-trained speaker verification model
   - Embeddings lie on unit sphere in high-dimensional space

3. **Cosine Similarity Analysis**:
   - Computes pairwise cosine similarity between segment embeddings
   - **Theoretical Guarantee**: Proves that cosine similarity provides reliable drift indicator under geometric assumptions
   - Low similarity between segments indicates potential speaker drift

4. **LLM-Based Assessment**:
   - Structures embedding representations as input prompts for LLMs
   - LLM analyzes embedding patterns to classify presence/absence of drift
   - Leverages LLM's reasoning capabilities for perceptual judgment

5. **Binary Classification**:
   - Final output: drift detected (1) or not detected (0)
   - Threshold optimization based on human validation data

**Theoretical Foundation**:
- Proves speaker embeddings cluster meaningfully on unit sphere
- Establishes geometric conditions under which cosine similarity reliably indicates drift
- Provides bounds on detection accuracy given embedding quality

**Benchmark Construction**:
- Synthetic speech generated using multiple state-of-the-art diffusion TTS models
- Human annotators validate presence/absence of speaker drift
- High-quality annotations enable reliable evaluation

### 📊 Experimental Results Summary

**LLM Evaluation**:
- Multiple state-of-the-art LLMs tested on embedding-to-reasoning pipeline
- All LLMs confirm viability of the approach
- Consistent performance across different LLM architectures

**Detection Performance**:
- High accuracy in detecting speaker drift instances
- Strong correlation with human judgments
- Effective across different TTS models and speaker types

**Geometric Analysis**:
- Speaker embeddings show clear clustering patterns on unit sphere
- Drift instances correspond to measurable trajectory deviations in embedding space
- Cosine similarity thresholds effectively separate drift vs. non-drift cases

**Research Impact**:
- Establishes speaker drift as standalone research problem in TTS quality assessment
- Bridges geometric signal analysis with LLM-based perceptual reasoning
- Provides foundation for future work on drift mitigation and TTS quality improvement

---

## 📄 Paper 4: Towards Real-Time Human-AI Musical Co-Performance: Accompaniment Generation with Latent Diffusion Models and MAX/MSP

**arXiv**: [2604.07612](https://arxiv.org/abs/2604.07612)  
**PDF**: [https://arxiv.org/pdf/2604.07612](https://arxiv.org/pdf/2604.07612)  
**Authors**: Academic (12 pages, 6 figures)  
**Institution**: Academic  
**Categories**: cs.SD, cs.AI  
**Published**: April 8, 2026

### 📝 One-Sentence Summary

This work presents a framework for real-time human-AI musical co-performance using latent diffusion models for accompaniment generation, achieving real-time operation through consistency distillation (5.4x speedup) while exposing fundamental trade-offs between latency, look-ahead depth, and generation quality.

### ✨ Core Innovations (3-5 points)

- **Real-Time Human-AI Co-Performance Framework**: First system combining MAX/MSP real-time audio environment with Python-based latent diffusion model for live musical accompaniment
- **OSC/UDP Communication Architecture**: Bridges MAX/MSP front-end (real-time audio I/O, buffering, playback) with Python inference server via OSC/UDP messaging
- **Sliding-Window Look-Ahead Protocol**: Formulates accompaniment generation as prediction of future audio from partial context with controlled look-ahead window
- **Consistency Distillation for Latency Reduction**: Applies consistency distillation to diffusion model, achieving 5.4x reduction in sampling time for real-time operation
- **Latency-Quality Trade-off Analysis**: Comprehensive evaluation exposing fundamental trade-off between model latency, look-ahead depth, and generation quality

### 🔬 Technical Method Details

**System Architecture**:

1. **MAX/MSP Front-End**:
   - Real-time audio input capture from live performance
   - Audio buffering and context management
   - Playback of generated accompaniment
   - OSC/UDP message handling for model communication

2. **Python Inference Server**:
   - Runs latent diffusion model for accompaniment generation
   - Receives context audio via OSC/UDP
   - Generates accompaniment conditioned on live input
   - Returns generated audio to MAX/MSP

3. **Communication Protocol**:
   - OSC (Open Sound Control) for low-latency messaging
   - UDP transport for minimal overhead
   - Synchronized timing for real-time performance

**Generation Protocol**:

1. **Sliding-Window Look-Ahead**:
   - Context window: Recent audio from live performance (e.g., 2-4 seconds)
   - Look-ahead window: Future audio to generate (e.g., 1-2 seconds)
   - Sliding mechanism: Continuous update as performance progresses

2. **Latent Diffusion Model**:
   - Operates in compressed latent space for efficiency
   - Conditions on context audio for coherent accompaniment
   - Generates future audio matching musical style and structure

3. **Consistency Distillation**:
   - Trains student model to match multi-step diffusion output in fewer steps
   - Reduces sampling iterations from typical 50-100 to 4-8 steps
   - Achieves 5.4x speedup while maintaining quality

**Latency Management**:
- Total system latency = audio I/O + communication + inference + playback
- Target: <100ms for acceptable real-time performance
- Consistency distillation critical for meeting latency budget

### 📊 Experimental Results Summary

**Latency Performance**:
- **Consistency Distillation Speedup**: 5.4x reduction in sampling time
- **Real-Time Operation**: Both original and distilled models achieve real-time performance
- **System Latency**: Within acceptable bounds for live performance (<100ms)

**Quality Evaluation**:

1. **Musical Coherence**:
   - Strong performance in Retrospective regime (looking back at context)
   - Generated accompaniment maintains musical consistency with input

2. **Beat Alignment**:
   - Accurate synchronization with live performance tempo
   - Maintains rhythmic coherence across generation windows

3. **Audio Quality**:
   - High fidelity in generated accompaniment
   - Minimal artifacts from diffusion process

**Look-Ahead Trade-off**:
- **Retrospective Regime**: Strong performance when relying on past context
- **Look-Ahead Degradation**: Quality degrades gracefully as look-ahead increases
- **Fundamental Trade-off**: Longer look-ahead provides more planning time but increases latency and uncertainty

**Key Insight**: The work demonstrates feasibility of diffusion-based real-time accompaniment while clearly characterizing the inherent tension between latency constraints and generation quality - a fundamental consideration for any real-time generative music system.

---

## 📈 Summary Statistics

| Metric | Value |
|--------|-------|
| Total Papers Reviewed | ~50+ |
| Papers Selected | 4 |
| Date Range | April 7-9, 2026 |
| Primary Categories | cs.SD, cs.AI, cs.CV, cs.CL |
| Key Themes | T2AV Evaluation, Voice Design, Speaker Drift, Real-Time Music Generation |
| Institutions Represented | Microsoft Research, Academic (multiple) |
| Conference Acceptances | ICASSP 2026 (1 paper) |

## 🎯 Focus Area Coverage

- ✅ **Text-to-Speech**: CapTalk (voice design), Speaker Drift Detection (TTS quality)
- ✅ **Audio Generation**: Real-Time Music Co-Performance (diffusion-based)
- ✅ **Generative Models**: All papers (diffusion, autoregressive, latent space models)
- ✅ **Text-to-Audio-Video**: AVGen-Bench (evaluation framework)
- ✅ **Speech Synthesis**: CapTalk, Speaker Drift Detection
- ✅ **Diffusion Models**: Speaker Drift Detection (diffusion TTS), Real-Time Music (latent diffusion)

## 🔗 Quick Links

- **AVGen-Bench Code**: [http://aka.ms/avgenbench](http://aka.ms/avgenbench)
- **CapTalk Audio Samples**: [Anonymous Demo](https://anonymous.4open.science/api/repo/Captalk-D601/file/index.html)
- **Speaker Drift Paper**: [arXiv:2604.06327](https://arxiv.org/abs/2604.06327) (ICASSP 2026)
- **Real-Time Music Paper**: [arXiv:2604.07612](https://arxiv.org/abs/2604.07612)

---

*Generated by Daily arXiv Digest - Text-to-Audio, Text-to-Speech & Generative Model*  
*Next digest: April 12, 2026 (Sunday)*
