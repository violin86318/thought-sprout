# Thought Sprout 🌱

> 将你碎片化的笔记转化为连贯、深刻的叙事。

这是一个 Claude Code 技能，分析用户的笔记集合并生成"发芽报告"（Sprout Report）——对你思想的文学和哲学探索。

## 概述

Thought Sprout 将原始、碎片化的笔记转化为精炼的叙事报告。它可以：
- 分析最近一段时间（默认：最近3天）的3-5条笔记
- 识别潜在的主题和模式
- 将每条笔记扩展为带有历史背景的精彩故事
- 为每个洞察提供连贯的"顿悟时刻"

## 工作原理

该技能遵循6步工作流程：

1. **笔记聚合** — 收集最近笔记，筛选有深度的内容
2. **主题分析** — 识别模式，生成诗意开篇
3. **故事驱动扩展** — 每条笔记变为：
   - 🌱 **种子** — 将想法连接到更大的概念
   - 📖 **故事** — 历史/科学背景
   - ✨ **顿悟** — 提炼的核心洞察
4. **金句共鸣**（可选）— 多视角引用扩展
5. **报告组装** — 编译成连贯文档
6. **质量控制** — 验证连贯性和准确性

## 安装

```bash
# 将此仓库克隆到你的 Claude Code 技能目录
cd ~/.claude/skills
git clone https://github.com/violin86318/thought-sprout.git
```

## 使用方法

安装后，通过以下方式调用技能：

- 要求"发芽我的想法"
- 请求从最近笔记生成"发芽报告"
- 明确触发对笔记的深度分析

## 高级功能：自动保存报告到指定文件夹

本地安装技能后，你可以让 Claude 修改技能本身，将生成的发芽报告自动保存到指定文件夹：

1. **告诉 Claude 你想要的输出文件夹：**
   ```
   "请修改 thought-sprout 技能，将所有生成的发芽报告保存到 ~/Documents/SproutReports"
   ```

2. **Claude 将会：**
   - 更新技能的提示模板，包含保存路径
   - 在生成报告时添加自动创建文件的功能
   - 将更改提交回此仓库

3. **对话示例：**
   ```
   你: 每次生成发芽报告后，自动保存到 ~/Documents/我的思考笔记 文件夹

   Claude: 我来修改 skill，让它在生成报告后自动保存...
   [Claude 编辑技能文件并提交更改]
   ```

4. **中英文皆可：**
   ```
   You: Save sprout reports to ~/Documents/MyNotes folder

   Claude: I'll modify the skill to automatically save reports...
   ```

## 项目结构

```
thought-sprout/
├── SKILL.md              # 技能元数据和文档
├── README.md             # 英文文档
├── README_CN.md          # 中文文档
├── references/
│   ├── system_prompt.md          # 核心人设和原则
│   ├── opening_prompt.md         # 诗意开篇生成
│   ├── expansion_prompt.md       # 故事驱动扩展
│   ├── story_search.md           # 研究策略
│   ├── quality_checklist.md      # 质量检查指南
│   └── CLAUDE.md                 # 技能记忆上下文
└── templates/            # （保留供未来使用）
```

## 核心原则

- **文学性胜于学术性** — 叙事风格，而非理论化
- **故事胜于事实** — 戏剧性背景很重要
- **温暖而富有哲学性** — 鼓励性的语调
- **可验证的准确性** — 所有事实都经过核对

## 许可证

MIT

---

由 [violin86318](https://github.com/violin86318) 用 ❤️ 制作
