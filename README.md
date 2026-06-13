[README.md](https://github.com/user-attachments/files/28917280/README.md)
# Claude Prompt Skills

> 提示词优化专家 — 57 种专业框架，把模糊的 prompt 改成清晰、可执行的版本。

## 这是什么

一个 Claude Code 技能，当你写不好 prompt、AI 回答不满意、或需要为特定任务设计高质量提示词时，它会自动匹配最合适的框架，帮你生成优化版本。

## 核心能力

| 能力 | 说明 |
|------|------|
| **诊断现有 prompt** | 分析问题：目标不清、缺约束、受众不明、格式模糊 |
| **智能匹配框架** | 按复杂度（简单/中等/复杂）和领域（营销、教育、决策等）推荐 |
| **追问补全** | 关键信息缺失时先问再写，不瞎猜 |
| **即插即用** | 输出可直接复制使用的优化 prompt，附带选择理由 |

## 触发方式

在 Claude Code 中输入以下任意关键词即自动激活：

```
提示词 / prompt / 优化提示 / 帮我改改 / 这个回答不好 / 不是我想要的 / 写个提示模板
```

示例：

```
帮我优化提示词，我想让 AI 帮我写营销文案
```

## 安装

### 方式一：Git 克隆（推荐）

```bash
git clone https://github.com/YOUR_USERNAME/claude-prompt-skills.git ~/.claude/skills/claude-prompt-skills
```

### 方式二：手动安装

1. 下载本仓库
2. 放到 Claude Code skills 目录：

| 系统 | 路径 |
|------|------|
| Windows | `C:\Users\<用户名>\.claude\skills\claude-prompt-skills\` |
| macOS / Linux | `~/.claude/skills/claude-prompt-skills/` |

3. 确认目录结构：

```
claude-prompt-skills/
├── SKILL.md                           # 技能定义（必需）
├── README.md                          # 本文件
├── references/
│   ├── Frameworks_Summary.md          # 57 个框架总览
│   └── frameworks/                    # 框架详细文档
│       ├── 01_RACEF_Framework.md
│       ├── 02_CRISPE_Framework.md
│       ├── ...
│       └── 57_RASCEF_Framework.md
└── evals/
    └── evals.json
```

### 验证安装

重启 Claude Code，运行：

```
/claude-prompt-skills 帮我写一个推广新产品的提示词
```

看到框架推荐 + 优化后的 prompt = 安装成功。

## 使用效果

**你输入：**
> 帮我优化提示词，我想让 AI 帮我写营销文案

**它输出：**

```
🎯 选定框架：BAB (Before-After-Bridge)
选择原因：BAB 专为营销场景设计，通过"痛点→愿景→方案"结构打动受众。

✨ 优化后的提示词：
[可直接复制的完整 prompt]

📝 优化说明：
- Before：补充了目标受众画像和当前痛点
- After：明确了期望的转化效果
- Bridge：加入了产品差异化卖点

💡 变体建议：
- 试试 SPEAR 框架，适合更长的说服性内容
- 用 Challenge-Solution-Benefit 结构做案例研究
```

## 包含的 57 个框架

按领域速查：

| 领域 | 推荐框架 |
|------|----------|
| 营销内容 | BAB、SPEAR、Challenge-Solution-Benefit、BLOG、PROMPT、RHODES |
| 决策分析 | RICE、Pros and Cons、Six Thinking Hats、Tree of Thought、PAUSE、What If |
| 教育培训 | Bloom's Taxonomy、ELI5、Socratic Method、PEE、Hamburger Model |
| 产品开发 | SCAMPER、HMW、CIDI、RELIC、3Cs Model |
| AI 对话/助手 | COAST、ROSES、TRACE、RACE、RASCEF |
| 写作创作 | BLOG、4S Method、Hamburger Model、Few-shot、RHODES、Chain of Destiny |
| 图像生成 | Atomic Prompting |
| 快速简单任务 | Zero-shot、ERA、TAG、APE、RTF |
| 复杂推理 | Chain of Thought、Tree of Thought |

完整框架列表见 [references/Frameworks_Summary.md](references/Frameworks_Summary.md)。

## 许可证

MIT
