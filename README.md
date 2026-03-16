<p align="center">
  <h1 align="center">Claude Office Skills</h1>
</p>

<p align="center">
  <strong>Complete Document Processing Toolkit for Claude Code</strong>
  <br>
  <em>5 format skills, 3 cross-format workflows, 3 ready-to-use templates -- covering PDF, Word, Excel, and PowerPoint</em>
</p>

<p align="center">
  <a href="https://github.com/LeoLin990405/claude-office-skills/blob/main/LICENSE"><img src="https://img.shields.io/github/license/LeoLin990405/claude-office-skills?style=flat-square" alt="License"></a>
  <a href="https://github.com/LeoLin990405/claude-office-skills/stargazers"><img src="https://img.shields.io/github/stars/LeoLin990405/claude-office-skills?style=flat-square" alt="Stars"></a>
  <a href="https://github.com/LeoLin990405/claude-office-skills/issues"><img src="https://img.shields.io/github/issues/LeoLin990405/claude-office-skills?style=flat-square" alt="Issues"></a>
  <img src="https://img.shields.io/badge/Claude%20Code-Skill-8A2BE2?style=flat-square&logo=anthropic&logoColor=white" alt="Claude Code Skill">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/PDF-EC1C24?style=flat-square&logo=adobe&logoColor=white" alt="PDF">
  <img src="https://img.shields.io/badge/Word-2B579A?style=flat-square&logo=microsoftword&logoColor=white" alt="Word">
  <img src="https://img.shields.io/badge/Excel-217346?style=flat-square&logo=microsoftexcel&logoColor=white" alt="Excel">
  <img src="https://img.shields.io/badge/PowerPoint-B7472A?style=flat-square&logo=microsoftpowerpoint&logoColor=white" alt="PowerPoint">
</p>

<p align="center">
  <a href="#features">Features</a> &nbsp;|&nbsp;
  <a href="#quick-start">Quick Start</a> &nbsp;|&nbsp;
  <a href="#skills">Skills</a> &nbsp;|&nbsp;
  <a href="#workflows">Workflows</a> &nbsp;|&nbsp;
  <a href="#templates">Templates</a> &nbsp;|&nbsp;
  <a href="#contributing">Contributing</a>
</p>

---

**English** | [中文](#中文)

## Features

| Feature | Description |
|---------|-------------|
| **PDF Processing** | Extract text, create PDFs, merge/split documents, fill & read forms |
| **Word Documents** | Create, edit, format `.docx` files with full OOXML schema support |
| **Excel Spreadsheets** | Formulas, charts, pivot tables, data validation, recalculation |
| **PowerPoint Presentations** | Slides, layouts, charts, animations, HTML-to-PPTX conversion |
| **Document Co-authoring** | Collaborative editing, review cycles, redlining workflows |
| **Cross-format Workflows** | Data-to-presentation pipeline, document review cycle, PDF form processing |
| **Ready-to-use Templates** | Business report, proposal, and meeting notes structures |
| **Intent-based Routing** | Auto-detects document type and routes to the right skill |

## Quick Start

### Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-office-skills.git
```

### Verify

```bash
ls ~/.claude/skills/claude-office-skills/SKILL.md
```

### Usage

The toolkit auto-routes based on your request, or you can invoke skills directly:

```
# Auto-routed examples
"Create a business report"           -> docx + report-structure template
"Merge these PDFs"                   -> pdf skill
"Build slides from this data"        -> data-to-presentation workflow

# Direct skill commands
/pdf                                 -> PDF manipulation
/docx                                -> Word documents
/xlsx                                -> Excel spreadsheets
/pptx                                -> PowerPoint presentations
/doc-coauthoring                     -> Collaborative editing
```

## Skills

| Skill | Command | Description |
|-------|---------|-------------|
| `pdf` | `/pdf` | PDF manipulation -- extract, create, merge, split, fill forms |
| `docx` | `/docx` | Word document processing -- create, edit, format, styles |
| `xlsx` | `/xlsx` | Excel spreadsheets -- formulas, charts, pivot tables, data validation |
| `pptx` | `/pptx` | PowerPoint presentations -- slides, layouts, charts, animations |
| `doc-coauthoring` | `/doc-coauthoring` | Collaborative document editing and review workflows |

## Workflows

Cross-format workflow guides for multi-step document tasks:

| Workflow | Pipeline | Guide |
|----------|----------|-------|
| **Data to Presentation** | xlsx analysis -> pptx slides | [data-to-presentation](workflows/data-to-presentation.md) |
| **Document Review Cycle** | docx draft -> review -> redline -> final | [document-review-cycle](workflows/document-review-cycle.md) |
| **PDF Form Processing** | PDF form extraction -> data processing -> output | [pdf-form-processing](workflows/pdf-form-processing.md) |

## Templates

Ready-to-use document structure templates:

| Template | Use Case |
|----------|----------|
| [report-structure](templates/report-structure.md) | Business report (exec summary, analysis, recommendations, appendix) |
| [proposal-structure](templates/proposal-structure.md) | Business proposal (problem, solution, pricing, timeline) |
| [meeting-notes](templates/meeting-notes.md) | Meeting notes (attendees, agenda, discussion, decisions, actions) |

## Project Structure

```
claude-office-skills/
├── SKILL.md                          # Skill index (entry point for Claude Code)
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── CHANGELOG.md
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.yml
│   │   ├── feature_request.yml
│   │   └── config.yml
│   ├── PULL_REQUEST_TEMPLATE.md
│   └── workflows/
│       └── claude-review.yml
├── skills/
│   ├── pdf/                          # PDF manipulation toolkit
│   │   ├── SKILL.md
│   │   ├── reference.md
│   │   ├── forms.md
│   │   └── scripts/                  # Python helpers (form fill, extract, validate)
│   ├── docx/                         # Word document processing
│   │   ├── SKILL.md
│   │   ├── docx-js.md
│   │   ├── ooxml.md
│   │   ├── ooxml/schemas/            # ISO-IEC 29500 & Microsoft OOXML schemas
│   │   ├── ooxml/scripts/            # Pack, unpack, validate utilities
│   │   └── scripts/                  # Document helpers & XML templates
│   ├── xlsx/                         # Excel spreadsheet processing
│   │   ├── SKILL.md
│   │   └── recalc.py
│   ├── pptx/                         # PowerPoint presentations
│   │   ├── SKILL.md
│   │   ├── html2pptx.md
│   │   ├── ooxml.md
│   │   ├── ooxml/schemas/            # OOXML schemas for presentations
│   │   ├── ooxml/scripts/            # Pack, unpack, validate utilities
│   │   └── scripts/                  # HTML2PPTX, inventory, rearrange, replace
│   └── doc-coauthoring/              # Collaborative editing workflow
│       └── SKILL.md
├── workflows/                        # Cross-format workflow guides
│   ├── data-to-presentation.md
│   ├── document-review-cycle.md
│   └── pdf-form-processing.md
└── templates/                        # Document structure templates
    ├── report-structure.md
    ├── proposal-structure.md
    └── meeting-notes.md
```

## Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to submit issues, feature requests, and pull requests.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---

## 中文

### 概述

**Claude Office Skills** 是一个完整的文档处理工具集，按格式和工作流组织。提供 5 个格式专用技能、3 个跨格式工作流和 3 个即用模板。

### 技能

| 技能 | 命令 | 描述 |
|------|------|------|
| `pdf` | `/pdf` | PDF 操作 -- 提取、创建、合并、拆分、填写表单 |
| `docx` | `/docx` | Word 文档处理 -- 创建、编辑、格式、样式 |
| `xlsx` | `/xlsx` | Excel 电子表格 -- 公式、图表、数据透视表、数据验证 |
| `pptx` | `/pptx` | PowerPoint 演示文稿 -- 幻灯片、布局、图表、动画 |
| `doc-coauthoring` | `/doc-coauthoring` | 协作文档编辑和审阅工作流 |

### 工作流

| 工作流 | 流程 | 指南 |
|--------|------|------|
| **数据到演示** | xlsx 分析 -> pptx 幻灯片 | [data-to-presentation](workflows/data-to-presentation.md) |
| **文档审阅周期** | docx 草稿 -> 审阅 -> 红线标注 -> 定稿 | [document-review-cycle](workflows/document-review-cycle.md) |
| **PDF 表单处理** | PDF 表单提取 -> 数据处理 -> 输出 | [pdf-form-processing](workflows/pdf-form-processing.md) |

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

<p align="center">
  <sub>Built with collaboration between human and AI</sub>
</p>
