# Thought Sprout 🌱

> Transform your fragmented notes into a coherent, insightful narrative.

A Claude Code skill that analyzes a collection of user notes to generate a "sprout report" — a literary and philosophical exploration of your own thoughts.

## Overview

Thought Sprout transforms raw, fragmented notes into a polished narrative report. It:
- Analyzes 3-5 notes from a recent period (default: last 3 days)
- Identifies underlying themes and patterns
- Expands each note into a compelling story with historical context
- Delivers a cohesive "Aha!" moment for each insight

## How It Works

The skill follows a 6-step workflow:

1. **Note Aggregation** — Gather recent notes, filter for depth
2. **Thematic Analysis** — Identify patterns and generate a poetic opening
3. **Story-Driven Expansion** — Each note becomes:
   - 🌱 **Seed** — Connecting ideas to larger concepts
   - 📖 **Story** — Historical/scientific context
   - ✨ **Aha Moment** — A distilled insight
4. **Golden Quote Resonance** (Optional) — Multi-perspective quote expansion
5. **Report Assembly** — Compile into a cohesive document
6. **Quality Control** — Verify coherence and accuracy

## Installation

```bash
# Clone this repository into your Claude Code skills directory
cd ~/.claude/skills
git clone https://github.com/violin86318/thought-sprout.git
```

## Usage

Once installed, invoke the skill by:

- Asking to "sprout my thoughts"
- Requesting a "sprout report" from your recent notes
- Explicitly triggering deeper analysis of your notes

## Advanced: Save Reports to Custom Folder

After installing the skill locally, you can ask Claude to modify the skill itself to automatically save generated sprout reports to a specified folder:

1. **Tell Claude your desired output folder:**
   ```
   "Please modify the thought-sprout skill to save all generated sprout reports to ~/Documents/SproutReports"
   ```

2. **Claude will then:**
   - Update the skill's prompt templates to include the save path
   - Add automatic file creation when generating reports
   - Commit the changes back to this repository

3. **Example conversation:**
   ```
   You: 每次生成发芽报告后，自动保存到 ~/Documents/我的思考笔记 文件夹

   Claude: 我来修改 skill，让它在生成报告后自动保存...
   [Claude edits the skill files and commits changes]
   ```

## Project Structure

```
thought-sprout/
├── SKILL.md              # Skill metadata and documentation
├── README.md             # English documentation
├── README_CN.md          # 中文文档
├── references/
│   ├── system_prompt.md          # Core persona and principles
│   ├── opening_prompt.md         # Poetic opening generation
│   ├── expansion_prompt.md       # Story-driven expansion
│   ├── story_search.md           # Research strategy
│   ├── quality_checklist.md      # QC guidelines
│   └── CLAUDE.md                 # Skill memory context
└── templates/            # (Reserved for future use)
```

## Core Principles

- **Literary over academic** — Narrative style, not theoretical
- **Stories over facts** — Dramatic context matters
- **Warm and philosophical** — Encouraging tone
- **Verifiable accuracy** — All facts checked

## License

MIT

---

Made with ❤️ by [violin86318](https://github.com/violin86318)
