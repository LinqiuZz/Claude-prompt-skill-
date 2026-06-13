---
  Claude Prompt Skills

  提示词优化专家 — 内置 57 种专业框架，帮你把模糊的 prompt 改成清晰、可执行的版本。

  功能

  - 诊断现有 prompt — 分析问题（目标不清、缺约束、受众不明等）
  - 智能匹配框架 — 按复杂度和领域自动推荐最合适的框架
  - 追问补全 — 信息不足时先问再写
  - 即插即用 — 输出可直接复制使用的优化 prompt

  适用场景

  ┌──────────────────────┬──────────┐
  │       你说的话       │ 触发优化 │
  ├──────────────────────┼──────────┤
  │ "帮我优化这个提示词" │ ✅       │
  ├──────────────────────┼──────────┤
  │ "这个 prompt 不好用" │ ✅       │
  ├──────────────────────┼──────────┤
  │ "写个提示模板"       │ ✅       │
  ├──────────────────────┼──────────┤
  │ "不是我想要的回答"   │ ✅       │
  └──────────────────────┴──────────┘

  安装

  方式一：克隆到 Claude Code skills 目录（推荐）

  git clone https://github.com/YOUR_USERNAME/claude-prompt-skills.git ~/.claude/skills/claude-prompt-skills

  方式二：手动安装

  1. 下载本仓库
  2. 复制整个文件夹到：
    - Windows: C:\Users\<你的用户名>\.claude\skills\claude-prompt-skills\
    - macOS/Linux: ~/.claude/skills/claude-prompt-skills/
  3. 确保目录结构如下：

  ~/.claude/skills/claude-prompt-skills/
  ├── SKILL.md                          # 技能定义
  ├── references/
  │   ├── Frameworks_Summary.md         # 框架总览
  │   └── frameworks/                   # 57 个框架详细文件
  │       ├── 01_RACEF_Framework.md
  │       ├── 02_CRISPE_Framework.md
  │       └── ...
  └── evals/
      └── evals.json

  验证安装

  重启 Claude Code，输入：

  /claude-prompt-skills 帮我优化这个提示词：写一篇关于AI的文章

  如果返回框架推荐和优化后的 prompt，说明安装成功。

  使用示例

  用户：帮我优化提示词，我想让 AI 帮我写营销文案

  Claude：
  🎯 选定框架：BAB (Before-After-Bridge)
  选择原因：BAB 框架专为营销场景设计，通过"痛点→愿景→方案"结构打动受众。

  ✨ 优化后的提示词：
  [生成的优化 prompt]

  📝 优化说明：
  - Before：补充了目标受众画像和当前痛点
  - After：明确了期望的转化效果
  - Bridge：加入了产品差异化卖点

  包含的 57 个框架

  覆盖营销、决策分析、教育、产品开发、AI 对话、写作创作、图像生成等领域。详见 references/Frameworks_Summary.md。
