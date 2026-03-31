---
name: daily-arxiv-digest
description: |
  每日 arXiv 论文自动搜索 + 价值判断 + 总结 + GitHub 展示一体化技能。
  自动在每天早上 8 点执行，搜索热门论文，筛选有价值论文，生成创新点总结，
  并推送到 GitHub 仓库展示。
  
  支持自定义配置：
  - 搜索领域 (cs.AI, cs.LG, cs.CV, cs.CL 等)
  - GitHub 仓库信息
  - 筛选标准
  - 执行时间
---

# Daily arXiv Digest - 每日论文自动摘要技能

## 🎯 技能概述

这是一个**全自动**的每日论文处理技能，整合了：
1. **arXiv 论文搜索** - 自动搜索最新热门论文
2. **价值判断** - 筛选有创新价值的论文
3. **深度总结** - 生成创新点介绍和笔记
4. **GitHub 展示** - 自动推送到公开仓库

---

## ⏰ 定时任务

**执行时间**: 每天早上 8:00 (Asia/Shanghai)

**触发方式**: 
- 自动：cron 定时任务
- 手动：用户说"运行每日论文摘要"或"更新论文库"

---

## 🔄 完整工作流程

```
┌─────────────────────────────────────────────────────────┐
│  每天早上 8:00 自动触发                                    │
└─────────────────────────────────────────────────────────┘
                          ↓
┌─────────────────────────────────────────────────────────┐
│  第 1 步：搜索 arXiv 热门论文                                 │
│  - 搜索 CS.AI, CS.LG, CS.CV, CS.CL 等热门领域              │
│  - 获取过去 24 小时发布的论文                               │
│  - 按引用数、下载数排序                                    │
└─────────────────────────────────────────────────────────┘
                          ↓
┌─────────────────────────────────────────────────────────┐
│  第 2 步：价值判断筛选                                     │
│  - 判断标准：                                             │
│    ✓ 来自知名机构 (MIT, Stanford, Google, Meta 等)        │
│    ✓ 作者有 h-index > 20                                  │
│    ✓ 标题/摘要包含突破性关键词                            │
│    ✓ 与热门方向相关 (LLM, Diffusion, RL 等)               │
│  - 筛选出 3-5 篇最有价值的论文                              │
└─────────────────────────────────────────────────────────┘
                          ↓
┌─────────────────────────────────────────────────────────┐
│  第 3 步：深度阅读与总结                                   │
│  - 下载论文 LaTeX 源码                                    │
│  - 解析并读取完整内容                                     │
│  - 生成以下内容：                                         │
│    • 一句话总结                                          │
│    • 核心创新点 (3-5 条)                                   │
│    • 技术方法详解                                        │
│    • 实验结果摘要                                        │
│    • 代码/项目链接                                       │
│    • 个人评价/启发                                       │
└─────────────────────────────────────────────────────────┘
                          ↓
┌─────────────────────────────────────────────────────────┐
│  第 4 步：生成 Markdown 文档                                 │
│  - 创建今日论文摘要文件                                   │
│  - 格式：YYYY-MM-DD-daily-digest.md                      │
│  - 包含所有筛选论文的总结                                │
└─────────────────────────────────────────────────────────┘
                          ↓
┌─────────────────────────────────────────────────────────┐
│  第 5 步：推送到 GitHub 仓库                                │
│  - 克隆/更新本地仓库                                      │
│  - 添加新生成的文档                                       │
│  - 提交并推送                                            │
│  - 仓库：https://github.com/YOUR_USERNAME/daily-arxiv-digest │
└─────────────────────────────────────────────────────────┘
                          ↓
┌─────────────────────────────────────────────────────────┐
│  第 6 步：发送通知                                         │
│  - 告诉用户任务完成                                       │
│  - 提供 GitHub 仓库链接                                    │
│  - 列出今日推荐的论文标题                                │
└─────────────────────────────────────────────────────────┘
```

---

## 📋 详细执行步骤

### 第 1 步：搜索 arXiv 论文

**搜索策略**:
```
1. 使用 arXiv API 搜索过去 24 小时的论文
2. 分类别搜索：
   - cs.AI (人工智能)
   - cs.LG (机器学习)
   - cs.CV (计算机视觉)
   - cs.CL (计算语言学)
   - cs.RO (机器人学)
3. 按提交时间排序，获取最新论文
4. 每个类别获取 Top 20 论文
```

**API 示例**:
```
http://export.arxiv.org/api/query?
  search_query=cat:cs.AI+AND+submittedDate:[YYYYMMDD000000+TO+YYYYMMDD235959]
  &sortBy=submittedDate&sortOrder=descending
  &max_results=20
```

---

### 第 2 步：价值判断筛选

**筛选标准** (满足任意 2 项即可):

| 标准 | 说明 | 权重 |
|------|------|------|
| 🏛️ 知名机构 | MIT, Stanford, Berkeley, CMU, Google, Meta, Microsoft, OpenAI 等 | 高 |
| 👨‍🔬 知名作者 | h-index > 20, 或领域内知名研究者 | 高 |
| 🔥 热门方向 | LLM, Transformer, Diffusion, RLHF, Multimodal 等 | 中 |
| 📊 突破性词汇 | "First", "Novel", "Breakthrough", "State-of-the-art" | 中 |
| 🔗 代码可用 | 提供 GitHub 链接 | 低 |
| 📈 引用潜力 | 摘要质量高，问题定义清晰 | 中 |

**输出**: 筛选出 3-5 篇最有价值的论文

---

### 第 3 步：深度阅读与总结

**对每篇论文执行**:

1. **下载源码**
   ```
   URL: https://arxiv.org/src/{arxiv_id}
   保存到：~/.cache/daily-arxiv-digest/{arxiv_id}.tar.gz
   ```

2. **解压读取**
   ```
   解压到：~/.cache/daily-arxiv-digest/{arxiv_id}/
   找到 main.tex 或入口文件
   递归读取所有相关文件
   ```

3. **生成总结** (Markdown 格式)
   ```markdown
   ## {论文标题}
   
   **arXiv**: {arxiv_id}
   **作者**: {作者列表}
   **机构**: {机构列表}
   **代码**: {GitHub 链接}
   
   ### 📌 一句话总结
   {用一句话概括论文核心贡献}
   
   ### 💡 核心创新点
   1. {创新点 1}
   2. {创新点 2}
   3. {创新点 3}
   
   ### 🔧 技术方法
   {详细描述技术方法，包括关键公式/架构}
   
   ### 📊 实验结果
   - {主要实验结果 1}
   - {主要实验结果 2}
   
   ### 🤔 个人评价
   {评价论文的价值、局限性、可借鉴之处}
   
   ### 🔗 相关链接
   - [arXiv 页面](https://arxiv.org/abs/{arxiv_id})
   - [代码仓库]({code_url})
   ```

---

### 第 4 步：生成 Markdown 文档

**文件命名**: `YYYY-MM-DD-daily-digest.md`

**文件结构**:
```markdown
# Daily arXiv Digest - {日期}

> 自动生成的每日 arXiv 论文摘要

## 📅 {日期} 推荐论文

共推荐 {N} 篇论文

---

## 论文 1: {标题}

{完整总结}

---

## 论文 2: {标题}

{完整总结}

---

## 📊 今日统计

| 类别 | 数量 |
|------|------|
| 搜索论文总数 | XX |
| 筛选后推荐 | XX |
| 主要领域 | XX, XX |

---

## 🔗 相关链接

- [GitHub 仓库](https://github.com/YOUR_USERNAME/daily-arxiv-digest)
- [arXiv 今日论文](https://arxiv.org/list/recent)
```

**保存位置**: `./daily-digests/YYYY-MM-DD-daily-digest.md`

---

### 第 5 步：推送到 GitHub

**前提条件**:
- 用户已配置 GitHub token
- 仓库已创建 (公开)

**执行步骤**:
```bash
# 1. 克隆/更新仓库
git clone https://github.com/YOUR_USERNAME/daily-arxiv-digest.git
cd daily-arxiv-digest

# 2. 添加新文档
cp ~/.cache/daily-arxiv-digest/digests/YYYY-MM-DD-daily-digest.md ./daily-digests/

# 3. 更新 README (可选)
# 添加今日论文链接到 README

# 4. 提交并推送
git add .
git commit -m "docs: add daily digest for YYYY-MM-DD"
git push origin main
```

**仓库结构**:
```
daily-arxiv-digest/
├── README.md              # 项目说明 + 今日论文链接
├── daily-digests/         # 每日摘要
│   ├── 2026-03-31-daily-digest.md
│   ├── 2026-04-01-daily-digest.md
│   └── ...
├── best-papers/           # 精选论文 (月度/年度)
└── .github/
    └── workflows/         # GitHub Actions (可选)
```

---

### 第 6 步：发送通知

**通知内容**:
```
✅ 今日论文摘要已完成！

📅 日期：2026-03-31
📝 推荐论文：3 篇
🔗 GitHub: https://github.com/YOUR_USERNAME/daily-arxiv-digest

今日推荐:
1. {论文标题 1}
2. {论文标题 2}
3. {论文标题 3}

点击查看完整摘要 👆
```

---

## 🔧 配置要求

### 方式 1: 使用配置文件 (推荐)

**位置**: `~/.agents/skills/daily-arxiv-digest/config.json`

首次使用时复制示例配置：

```bash
cp ~/.agents/skills/daily-arxiv-digest/config.example.json \
   ~/.agents/skills/daily-arxiv-digest/config.json
```

然后编辑 `config.json` 自定义你的配置。

### 方式 2: 环境变量

| 配置项 | 说明 | 示例 |
|--------|------|------|
| `GITHUB_TOKEN` | GitHub API token | `ghp_xxxxxxxxxxxx` |
| `GITHUB_USERNAME` | GitHub 用户名 | `your-username` |
| `GITHUB_REPO` | 仓库名称 | `daily-arxiv-digest` |

### 配置文件详解

```json
{
  "search": {
    "categories": ["cs.AI", "cs.LG", "cs.CV", "cs.CL"],
    "timeRange": "24h",
    "maxResults": 20
  },
  "filter": {
    "minPapers": 3,
    "maxPapers": 5,
    "institutions": ["MIT", "Stanford", "Google", "Meta"],
    "hotKeywords": ["LLM", "Transformer", "Diffusion"],
    "minHIndex": 20
  },
  "github": {
    "token_env": "GITHUB_TOKEN",
    "username_env": "GITHUB_USERNAME",
    "repo_env": "GITHUB_REPO",
    "branch": "main",
    "digests_dir": "daily-digests",
    "auto_push": true
  },
  "schedule": {
    "enabled": true,
    "timezone": "Asia/Shanghai",
    "cron": "0 8 * * *"
  }
}
```

### 配置项说明

#### 搜索配置 (search)

| 字段 | 说明 | 默认值 |
|------|------|--------|
| `categories` | arXiv 分类列表 | `["cs.AI", "cs.LG", "cs.CV", "cs.CL"]` |
| `timeRange` | 搜索时间范围 | `"24h"` |
| `maxResults` | 每个分类获取论文数 | `20` |
| `sortBy` | 排序方式 | `"submittedDate"` |

**常用 arXiv 分类**:
- `cs.AI` - 人工智能
- `cs.LG` - 机器学习
- `cs.CV` - 计算机视觉
- `cs.CL` - 计算语言学
- `cs.RO` - 机器人学
- `cs.SD` - 语音
- `cs.NE` - 神经网络
- `stat.ML` - 统计机器学习

#### 筛选配置 (filter)

| 字段 | 说明 | 默认值 |
|------|------|--------|
| `minPapers` | 最少推荐论文数 | `3` |
| `maxPapers` | 最多推荐论文数 | `5` |
| `institutions` | 优先机构列表 | 见配置文件 |
| `hotKeywords` | 热门关键词 | 见配置文件 |
| `minHIndex` | 最小 h-index | `20` |

#### GitHub 配置 (github)

| 字段 | 说明 | 默认值 |
|------|------|--------|
| `token_env` | Token 环境变量名 | `"GITHUB_TOKEN"` |
| `username_env` | 用户名环境变量名 | `"GITHUB_USERNAME"` |
| `repo_env` | 仓库环境变量名 | `"GITHUB_REPO"` |
| `branch` | 分支名 | `"main"` |
| `digests_dir` | 摘要目录 | `"daily-digests"` |
| `best_papers_dir` | 精选目录 | `"best-papers"` |
| `auto_push` | 自动推送 | `true` |

#### 输出配置 (output)

| 字段 | 说明 | 默认值 |
|------|------|--------|
| `cache_dir` | 缓存目录 | `"~/.cache/daily-arxiv-digest"` |
| `digests_dir` | 输出目录 | `"./daily-digests"` |
| `include_abstract` | 包含摘要 | `true` |
| `include_code_link` | 包含代码链接 | `true` |
| `include_pdf_link` | 包含 PDF 链接 | `true` |

#### 定时配置 (schedule)

| 字段 | 说明 | 默认值 |
|------|------|--------|
| `enabled` | 启用定时任务 | `true` |
| `timezone` | 时区 | `"Asia/Shanghai"` |
| `cron` | Cron 表达式 | `"0 8 * * *"` |
| `retry_count` | 失败重试次数 | `3` |

#### 通知配置 (notification)

| 字段 | 说明 | 默认值 |
|------|------|--------|
| `enabled` | 启用通知 | `true` |
| `on_success` | 成功时通知 | `true` |
| `on_failure` | 失败时通知 | `true` |
| `include_paper_titles` | 包含论文标题 | `true` |
| `include_github_link` | 包含 GitHub 链接 | `true` |

---

## 📦 依赖工具

| 工具 | 用途 |
|------|------|
| `curl` | 调用 arXiv API |
| `tar` | 解压论文源码 |
| `git` | 推送到 GitHub |
| `grep/sed` | 文本处理 |

---

## 🚀 首次使用指南

### 1. 创建 GitHub 仓库

```bash
# 访问 https://github.com/new
# 仓库名：daily-arxiv-digest
# 可见性：Public
# 不要初始化 README
```

### 2. 配置 GitHub Token

```bash
# 访问 https://github.com/settings/tokens
# 生成 classic token
# 勾选 repo 权限
# 保存 token
```

### 3. 设置定时任务

使用 cron 设置每天早上 8 点执行：

```bash
# 编辑 crontab
crontab -e

# 添加以下行
0 8 * * * /path/to/openclaw -c "运行每日论文摘要"
```

或使用 OpenClaw 的 cron 功能：

```
设置每日早上 8 点的定时任务，执行"运行每日论文摘要"
```

### 4. 手动测试

```
用户：运行每日论文摘要

AI: 开始执行每日论文摘要任务...
[执行各个步骤...]
✅ 完成！
```

---

## ⚠️ 注意事项

1. **API 限制**: arXiv API 有请求频率限制，建议添加延迟
2. **存储空间**: 论文源码会缓存到本地，定期清理旧文件
3. **Token 安全**: GitHub token 要妥善保管，不要泄露
4. **错误处理**: 如果某篇论文下载失败，跳过并继续处理其他论文
5. **周末/假期**: 可选择周末不执行，或减少推荐数量

---

## 📊 成功标准

任务完成后应满足：

- ✅ 搜索了至少 50 篇论文
- ✅ 筛选出 3-5 篇有价值论文
- ✅ 为每篇论文生成详细总结
- ✅ 成功推送到 GitHub 仓库
- ✅ 用户收到完成通知

---

## 🔄 错误处理

| 错误 | 处理方式 |
|------|----------|
| arXiv API 失败 | 重试 3 次，仍失败则跳过 |
| 论文下载失败 | 记录日志，跳过该论文 |
| GitHub 推送失败 | 保存本地，通知用户手动推送 |
| 无有价值论文 | 发送通知说明今日无推荐 |

---

## 💡 优化建议

1. **智能筛选**: 根据用户历史偏好调整筛选标准
2. **多领域支持**: 支持用户自定义关注的领域
3. **论文追踪**: 追踪已推荐论文的后续引用/更新
4. **周报/月报**: 自动生成周度/月度精选
5. **RSS 订阅**: 提供 RSS feed 订阅功能

---

## 📝 示例输出

### 用户触发
```
用户：运行每日论文摘要
```

### AI 执行
```
🤖 开始执行每日论文摘要任务...

📡 第 1 步：搜索 arXiv 热门论文
   - 搜索 cs.AI, cs.LG, cs.CV, cs.CL
   - 找到 87 篇新论文

🔍 第 2 步：价值判断筛选
   - 知名机构论文：23 篇
   - 热门方向论文：45 篇
   - 筛选出 4 篇推荐论文

📖 第 3 步：深度阅读与总结
   - 正在下载论文 1/4...
   - 正在生成总结...
   - 完成 4 篇论文总结

📄 第 4 步：生成 Markdown 文档
   - 创建 2026-03-31-daily-digest.md

🚀 第 5 步：推送到 GitHub
   - 克隆仓库...
   - 添加文档...
   - 提交并推送...
   - ✅ 推送成功！

📬 第 6 步：发送通知
   - 通知已发送

✅ 任务完成！

今日推荐:
1. "Attention Is All You Need v2" - Google
2. "Diffusion Models Beat GANs" - MIT
3. "RLHF for Code Generation" - Stanford
4. "Multimodal LLM Survey" - Meta

🔗 查看完整摘要:
https://github.com/your-username/daily-arxiv-digest
```

---

## 🎯 技能边界

**本技能负责**:
- ✅ arXiv 论文搜索
- ✅ 论文价值判断
- ✅ 论文下载与解析
- ✅ 生成创新点总结
- ✅ 推送到 GitHub

**本技能不负责**:
- ❌ PDF 格式转换
- ❌ 论文代码复现
- ❌ 实验验证
- ❌ 同行评审

---

## 📞 故障排查

如果任务失败，检查：

1. **网络连接**: 是否能访问 arxiv.org
2. **GitHub Token**: 是否有效，权限是否足够
3. **磁盘空间**: 缓存目录是否有足够空间
4. **Git 配置**: 是否正确配置用户信息
5. **日志文件**: 查看执行日志定位问题

---

**技能版本**: 1.0.0  
**最后更新**: 2026-03-31  
**作者**: Liu  
**许可**: MIT

---

## 📝 配置使用指南

### 首次配置

1. **复制配置文件**
```bash
cp ~/.agents/skills/daily-arxiv-digest/config.example.json \
   ~/.agents/skills/daily-arxiv-digest/config.json
```

2. **编辑配置文件**
```bash
nano ~/.agents/skills/daily-arxiv-digest/config.json
```

3. **修改搜索方向**
```json
{
  "search": {
    "categories": [
      "cs.AI",      // 人工智能
      "cs.LG",      // 机器学习
      "cs.CV",      // 计算机视觉
      "cs.CL"       // 自然语言处理
    ]
  }
}
```

4. **修改 GitHub 仓库**
```json
{
  "github": {
    "username_env": "GITHUB_USERNAME",
    "repo_env": "MY_PAPER_REPO"  // 自定义仓库名
  }
}
```

```bash
# 设置环境变量
export MY_PAPER_REPO="my-daily-papers"
```

5. **修改执行时间**
```json
{
  "schedule": {
    "cron": "0 9 * * *"  // 改为每天早上 9 点
  }
}
```

### 常用配置组合

#### 只关注 LLM 相关
```json
{
  "search": {
    "categories": ["cs.CL", "cs.AI"]
  },
  "filter": {
    "hotKeywords": ["LLM", "Language Model", "Transformer", "GPT"]
  }
}
```

#### 只关注顶级机构
```json
{
  "filter": {
    "institutions": ["MIT", "Stanford", "Berkeley", "Google", "OpenAI"]
  }
}
```

#### 增加推荐数量
```json
{
  "filter": {
    "minPapers": 5,
    "maxPapers": 10
  }
}
```

### 验证配置

```bash
# 检查配置文件语法
cat ~/.agents/skills/daily-arxiv-digest/config.json | python -m json.tool

# 查看当前配置
cat ~/.agents/skills/daily-arxiv-digest/config.json
```

---

**技能版本**: 1.1.0 (支持配置)  
**最后更新**: 2026-03-31  
**作者**: Liu  
**许可**: MIT
