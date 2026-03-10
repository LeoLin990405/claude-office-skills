<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-Skill-blue?style=for-the-badge" alt="Claude Code Skill">
  <img src="https://img.shields.io/badge/Skills-5-green?style=for-the-badge" alt="Skills">
  <img src="https://img.shields.io/badge/Workflows-3-purple?style=for-the-badge" alt="Workflows">
  <img src="https://img.shields.io/badge/Templates-3-orange?style=for-the-badge" alt="Templates">
  <img src="https://img.shields.io/badge/Document-Toolkit-217346?style=for-the-badge" alt="Document Toolkit">
</p>

<h1 align="center">Document Toolkit</h1>

<p align="center">
  <strong>Complete Document Processing Toolkit for Claude Code</strong>
  <br>
  <em>5 format skills, 3 cross-format workflows, 3 ready-to-use templates — covering PDF, Word, Excel, and PowerPoint</em>
</p>

<p align="center">
  <a href="#-skills">Skills</a> •
  <a href="#-workflows">Workflows</a> •
  <a href="#-templates">Templates</a> •
  <a href="#-quick-start">Quick Start</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-CLI-8A2BE2?logo=anthropic&logoColor=white" alt="Claude Code">
  <img src="https://img.shields.io/badge/PDF-EC1C24?logo=adobe&logoColor=white" alt="PDF">
  <img src="https://img.shields.io/badge/Word-2B579A?logo=microsoftword&logoColor=white" alt="Word">
  <img src="https://img.shields.io/badge/Excel-217346?logo=microsoftexcel&logoColor=white" alt="Excel">
  <img src="https://img.shields.io/badge/PowerPoint-B7472A?logo=microsoftpowerpoint&logoColor=white" alt="PowerPoint">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</p>

**English** | [中文](#中文)

---

## Overview

**Document Toolkit** is a complete document processing toolkit organized by format and workflow. It provides 5 format-specific skills for creating, editing, and analyzing Office documents, plus cross-format workflows and ready-to-use templates.

### What Changed (v2.0)

| Before (v1) | After (v2) |
|-------------|------------|
| 5 standalone skills | **5 skills + routing layer** |
| No templates | **3 ready-to-use document templates** |
| Single-format focus | **3 cross-format workflows** |
| Flat skill list | **Intent-based routing with quick actions** |

---

## Skills

| Skill | Command | Description |
|-------|---------|-------------|
| `pdf` | `/pdf` | PDF manipulation — extract, create, merge, split, fill forms |
| `docx` | `/docx` | Word document processing — create, edit, format, styles |
| `xlsx` | `/xlsx` | Excel spreadsheets — formulas, charts, pivot tables, data validation |
| `pptx` | `/pptx` | PowerPoint presentations — slides, layouts, charts, animations |
| `doc-coauthoring` | `/doc-coauthoring` | Collaborative document editing and review workflows |

---

## Workflows

Cross-format workflow guides for multi-step document tasks:

| Workflow | Pipeline | Guide |
|----------|----------|-------|
| **Data to Presentation** | xlsx analysis → pptx slides | [data-to-presentation](workflows/data-to-presentation.md) |
| **Document Review Cycle** | docx draft → review → redline → final | [document-review-cycle](workflows/document-review-cycle.md) |
| **PDF Form Processing** | PDF form extraction → data processing → output | [pdf-form-processing](workflows/pdf-form-processing.md) |

---

## Templates

Ready-to-use document structure templates:

| Template | Use Case |
|----------|----------|
| [report-structure](templates/report-structure.md) | Business report (exec summary, analysis, recommendations, appendix) |
| [proposal-structure](templates/proposal-structure.md) | Business proposal (problem, solution, pricing, timeline) |
| [meeting-notes](templates/meeting-notes.md) | Meeting notes (attendees, agenda, discussion, decisions, actions) |

---

## Quick Start

### Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-office-skills.git
```

### Verify Installation

```bash
ls ~/.claude/skills/claude-office-skills/SKILL.md
```

### Usage

```bash
# The toolkit auto-routes based on your request:
"Create a business report"           → docx + report-structure template
"Write a proposal"                   → docx + proposal-structure template
"Merge these PDFs"                   → pdf skill
"Build slides from this data"        → data-to-presentation workflow
"Review and redline this doc"        → document-review-cycle workflow

# Or access skills directly:
/pdf                                 → PDF manipulation
/docx                                → Word documents
/xlsx                                → Excel spreadsheets
/pptx                                → PowerPoint presentations
/doc-coauthoring                     → Collaborative editing
```

---

## 中文

### 概述

**Document Toolkit** 是一个完整的文档处理工具集，按格式和工作流组织。提供 5 个格式专用技能、3 个跨格式工作流和 3 个即用模板。

### 技能

| 技能 | 命令 | 描述 |
|------|------|------|
| `pdf` | `/pdf` | PDF 操作 — 提取、创建、合并、拆分、填写表单 |
| `docx` | `/docx` | Word 文档处理 — 创建、编辑、格式、样式 |
| `xlsx` | `/xlsx` | Excel 电子表格 — 公式、图表、数据透视表、数据验证 |
| `pptx` | `/pptx` | PowerPoint 演示文稿 — 幻灯片、布局、图表、动画 |
| `doc-coauthoring` | `/doc-coauthoring` | 协作文档编辑和审阅工作流 |

### 工作流

| 工作流 | 流程 | 指南 |
|--------|------|------|
| **数据到演示** | xlsx 分析 → pptx 幻灯片 | [data-to-presentation](workflows/data-to-presentation.md) |
| **文档审阅周期** | docx 草稿 → 审阅 → 红线标注 → 定稿 | [document-review-cycle](workflows/document-review-cycle.md) |
| **PDF 表单处理** | PDF 表单提取 → 数据处理 → 输出 | [pdf-form-processing](workflows/pdf-form-processing.md) |

### 模板

| 模板 | 用途 |
|------|------|
| [report-structure](templates/report-structure.md) | 商业报告（摘要、分析、建议、附录） |
| [proposal-structure](templates/proposal-structure.md) | 商业提案（问题、方案、定价、时间线） |
| [meeting-notes](templates/meeting-notes.md) | 会议记录（参会人、议程、讨论、决定、行动项） |

### 安装

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-office-skills.git
```

---

## Contributors

- **Leo** ([@LeoLin990405](https://github.com/LeoLin990405)) - Project Lead
- **Claude** (Anthropic Claude Opus 4.6) - Content Generation

## License

MIT License - see [LICENSE](LICENSE) for details.

---

<p align="center">
  <sub>Built with collaboration between human and AI</sub>
</p>
