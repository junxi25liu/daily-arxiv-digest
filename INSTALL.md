# Daily arXiv Digest Skill - 安装与配置指南

## ✅ 已完成内容

### 1. 技能文件创建

**位置**: `/home/admin/.openclaw/workspace/skills/daily-arxiv-digest/`

```
daily-arxiv-digest/
├── SKILL.md           # 技能执行指南 (9.3KB)
├── README.md          # 用户文档 (2.7KB)
└── INSTALL.md         # 本文件
```

### 2. Cron 定时任务设置

- **任务 ID**: `955c79bb-9b62-4fa9-82ae-fc777bdfe000`
- **名称**: 每日 arXiv 论文摘要
- **执行时间**: 每天早上 8:00 (Asia/Shanghai)
- **下次执行**: 明天早上 8 点
- **状态**: ✅ 已启用

---

## 📦 安装步骤

### 方式 1: 本地安装 (推荐)

```bash
# 1. 复制技能到 OpenClaw 技能目录
cp -r /home/admin/.openclaw/workspace/skills/daily-arxiv-digest \
      ~/.agents/skills/

# 2. 验证安装
ls -la ~/.agents/skills/daily-arxiv-digest/
```

### 方式 2: 使用 Skills CLI

```bash
# 先将技能发布到 GitHub
cd /home/admin/.openclaw/workspace/skills/daily-arxiv-digest
git remote add origin https://github.com/YOUR_USERNAME/daily-arxiv-digest-skill.git
git push -u origin main

# 然后安装
npx skills add YOUR_USERNAME/daily-arxiv-digest-skill -g -y
```

---

## 🔧 配置 GitHub

### 1. 创建展示仓库

访问 https://github.com/new 创建：
- **Repository name**: `daily-arxiv-digest`
- **Description**: Daily arXiv Paper Digest - 每日论文自动摘要
- **Public**: ✅
- **Initialize**: ❌

### 2. 生成 GitHub Token

访问 https://github.com/settings/tokens:
- 点击 **Generate new token (classic)**
- Note: `Daily arXiv Digest`
- 勾选 **repo** (全部权限)
- 点击 **Generate token**
- 复制 token (只显示一次!)

### 3. 配置环境变量

编辑 `~/.bashrc` 或 `~/.zshrc`:

```bash
# GitHub 配置
export GITHUB_TOKEN="ghp_xxxxxxxxxxxxxxxxxxxx"
export GITHUB_USERNAME="your-username"
export GITHUB_REPO="daily-arxiv-digest"
```

使配置生效:

```bash
source ~/.bashrc  # 或 source ~/.zshrc
```

### 4. 验证配置

```bash
# 测试 GitHub API
curl -H "Authorization: token $GITHUB_TOKEN" \
     https://api.github.com/user
```

---

## 🚀 测试技能

### 手动触发

```
用户：运行每日论文摘要

AI: 🤖 开始执行每日论文摘要任务...

📡 第 1 步：搜索 arXiv 热门论文
   - 搜索 cs.AI, cs.LG, cs.CV, cs.CL
   - 找到 XX 篇新论文

🔍 第 2 步：价值判断筛选
   - 筛选出 X 篇推荐论文

📖 第 3 步：深度阅读与总结
   - 正在下载论文...
   - 正在生成总结...

📄 第 4 步：生成 Markdown 文档

🚀 第 5 步：推送到 GitHub
   - 推送成功！

📬 第 6 步：发送通知

✅ 任务完成！
```

### 检查定时任务

```bash
# 查看 cron 任务状态
openclaw cron list

# 应该看到:
# ✓ 每日 arXiv 论文摘要 - 每天 08:00 执行
```

### 手动运行 cron 任务

```bash
# 立即执行一次测试
openclaw cron run 955c79bb-9b62-4fa9-82ae-fc777bdfe000
```

---

## 📊 预期输出

### GitHub 仓库结构

```
daily-arxiv-digest/
├── README.md              # 项目说明 + 最新论文链接
├── daily-digests/         # 每日摘要
│   ├── 2026-03-31-daily-digest.md
│   ├── 2026-04-01-daily-digest.md
│   └── ...
└── best-papers/           # 月度精选
    └── 2026-03-best-papers.md
```

### 每日摘要格式

```markdown
# Daily arXiv Digest - 2026-03-31

> 自动生成的每日 arXiv 论文摘要

## 📅 2026-03-31 推荐论文

共推荐 3 篇论文

---

## 论文 1: Attention Is All You Need v2

**arXiv**: 2603.12345
**作者**: John Smith, Jane Doe
**机构**: Google Research
**代码**: https://github.com/google/attention-v2

### 📌 一句话总结
提出了改进的注意力机制...

### 💡 核心创新点
1. ...
2. ...
3. ...

### 🔧 技术方法
...

### 📊 实验结果
...

### 🤔 个人评价
...
```

---

## ⚠️ 故障排查

### 问题 1: 技能未找到

```bash
# 检查技能是否安装
ls -la ~/.agents/skills/daily-arxiv-digest/

# 如果没有，手动复制
cp -r /home/admin/.openclaw/workspace/skills/daily-arxiv-digest \
      ~/.agents/skills/
```

### 问题 2: GitHub 推送失败

```bash
# 检查 token 是否有效
curl -H "Authorization: token $GITHUB_TOKEN" \
     https://api.github.com/user

# 检查仓库是否存在
curl -H "Authorization: token $GITHUB_TOKEN" \
     https://api.github.com/repos/$GITHUB_USERNAME/$GITHUB_REPO
```

### 问题 3: arXiv API 失败

```bash
# 测试 arXiv API
curl "http://export.arxiv.org/api/query?search_query=cat:cs.AI&max_results=1"

# 如果失败，检查网络连接
ping arxiv.org
```

### 问题 4: 定时任务未执行

```bash
# 查看 cron 任务状态
openclaw cron status

# 查看任务历史
openclaw cron runs 955c79bb-9b62-4fa9-82ae-fc777bdfe000

# 重新启用任务
openclaw cron update 955c79bb-9b62-4fa9-82ae-fc777bdfe000 --enabled=true
```

---

## 📝 自定义配置

### 修改执行时间

编辑 cron 任务：

```bash
openclaw cron update 955c79bb-9b62-4fa9-82ae-fc777bdfe000 \
  --schedule="0 9 * * *"  # 改为每天早上 9 点
```

### 修改搜索领域

编辑 `SKILL.md`，修改搜索分类：

```markdown
搜索分类:
- cs.AI (人工智能)
- cs.LG (机器学习)
- cs.CV (计算机视觉)
- cs.CL (自然语言处理)
- cs.RO (机器人学)  # 添加这个
```

### 修改推荐数量

在 `SKILL.md` 中修改：

```markdown
筛选出 3-5 篇最有价值的论文
# 改为
筛选出 5-10 篇最有价值的论文
```

---

## 📞 获取帮助

### 查看技能文档

```bash
cat ~/.agents/skills/daily-arxiv-digest/SKILL.md
```

### 查看 cron 任务

```bash
openclaw cron list
openclaw cron status
```

### 查看执行日志

```bash
# 查看最近的执行记录
openclaw cron runs 955c79bb-9b62-4fa9-82ae-fc777bdfe000
```

---

## 🎉 完成！

现在你已经完成了所有配置：

- ✅ 技能文件已创建
- ✅ Cron 定时任务已设置 (每天早上 8 点)
- ✅ GitHub 仓库待创建
- ✅ 环境变量待配置

**下一步**:
1. 创建 GitHub 仓库
2. 配置环境变量
3. 手动测试一次
4. 等待明天早上 8 点自动执行！

---

**最后更新**: 2026-03-31  
**版本**: 1.0.0
