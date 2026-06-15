# Kuangkuang Gaokao Perspective - College Admission Advisor Skill

> *"College application might be the first time you truly take control of your destiny's steering wheel"*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-Standard-green)](https://agentskills.io)
[![Version](https://img.shields.io/badge/version-1.0.0-blue)](CHANGELOG.md)

An AI Skill based on the college admission methodology of **Kuangkuang** (取景框看世界), a Bilibili content creator. This skill distills 10 years of educational experience and public welfare sharing into a systematic decision-making framework, helping students from ordinary families make informed college application choices.

[中文文档](README.md) | [Installation](#installation) | [Core Methodology](#core-methodology) | [Contributing](CONTRIBUTING.md)

---

## 👨‍🎓 Who is Kuangkuang?

**Kuangkuang (取景框看世界)**:
- 🎓 PhD from Fudan University, from an ordinary working-class family in Chongqing
- 👨‍🏫 10 years of educational experience (2015 counselor → 2025 full-time education)
- 🎯 Core Philosophy: **Systematic Thinking + Personalized Decision + Fault-Tolerant Orientation**
- 💚 Mission: "Because I was once a child caught in the rain, I want to hold an umbrella for others"
- 🆓 Committed to free public sharing, enabling students from ordinary families to make scientific college choices without paying expensive fees

---

## 🧠 Core Methodology

### 5 Mental Models

| Model | Application | Core Logic |
|-------|------------|------------|
| **Fault-Tolerant Space Model** | Making major choices under uncertainty | Both major popularity and personal interests change; reserve room for adjustment |
| **Tiered Decision Model** | Weighing university, major, and location | High scores: university > major; Low scores: major > university |
| **Self-Positioning Model** | Essential self-awareness before application | Four-question framework: economic conditions, family resources, score range, learning ability |
| **Decision Ownership Model** | Who makes the final decision | All external voices are references; you must make the final decision |
| **Score-Education Matching Model** | Whether to choose majors requiring graduate education | High scores + willingness to pursue higher education = OK; Low scores + no such willingness = avoid |

### 10 Decision Heuristics (Quick Judgment Rules)

1. ⚡ **High scores aim for universities, low scores secure majors**
2. ⚡ **Humanities: university matters; STEM: major matters; Medicine: location matters**
3. ⚡ **Old Gaokao system: MUST accept major adjustments**
4. ⚡ **Early batch admission is mutual selection, not a blind box**
5. ⚡ **When reaching for universities, avoid popular majors**
6. ⚡ **One character difference, world apart** (verify names word by word)
7. ⚡ **Check Ministry of Education official list to avoid fake universities**
8. ⚡ **Before enrollment, check three things: location, dorm, shower facilities**
9. ⚡ **Ignoring admission regulations = risk of post-admission rejection**
10. ⚡ **All advice is reference; you must make the final decision**

[View full methodology →](SKILL.md)

---

## 🚀 Installation

### Method 1: One-Click Install (Recommended)

```bash
# Install via Agent Skills standard
npx skills add alchaincyf/kuangkuang-gaokao-perspective
```

### Method 2: Manual Installation

Copy `SKILL.md` to the appropriate directory based on your AI runtime:

| AI Runtime | Installation Path |
|-----------|-------------------|
| **Claude Code** | `~/.claude/skills/kuangkuang-gaokao-perspective/` |
| **Cursor** | `~/.cursor/skills/` or `.cursor/skills/` in project root |
| **Windsurf** | `~/.windsurf/skills/` |
| **Other Agent Skills-compatible tools** | Check tool documentation |

**Manual installation steps**:
```bash
# 1. Clone the repository
git clone https://github.com/alchaincyf/kuangkuang-gaokao-perspective.git

# 2. Copy to skills directory
cp -r kuangkuang-gaokao-perspective ~/.claude/skills/

# 3. Verify installation
ls ~/.claude/skills/kuangkuang-gaokao-perspective/SKILL.md
```

---

## 📖 Usage Guide

### When to Activate This Skill

This skill automatically activates when you encounter questions like:
- "Which is more important: university or major?"
- "How should I choose with my score?"
- "My family has limited financial resources, what majors should I consider?"
- "Should I fill in the early batch?"
- "Will accepting major adjustments be a trap?"
- "How to identify fake universities?"

### Suitable Questions

✅ **Good for**:
- Decision-making frameworks and priority judgment for college applications
- Weighing university-major-location trade-offs
- Pitfall prevention guide and risk avoidance
- Information channels and tool usage
- Identifying and comparing specific majors/universities

❌ **Not suitable for**:
- "Choose a specific major for me" (you need to make your own decision)
- "How will XX major's employment look in four years" (cannot predict the future)
- "What am I suited to study" (requires individualized judgment based on your situation)

---

## 📁 Repository Structure

```
kuangkuang-gaokao-perspective/
├── SKILL.md                           # Core skill file (AI loads this)
├── README.md                          # Documentation (Chinese)
├── README_EN.md                       # Documentation (English)
├── LICENSE                            # MIT License
├── CONTRIBUTING.md                    # Contributing guide
├── CHANGELOG.md                       # Version history
├── examples/                          # Dialogue examples
├── references/                        # Source materials and research
│   ├── research/                      # 6 research reports
│   └── sources/transcripts/           # 5 video transcript files
└── .gitignore                         # Git ignore configuration
```

---

## 📊 Data Sources

### Original Materials

This skill is based on 5 college admission-themed videos released by Kuangkuang in 2025:

1. **Complete Gaokao Admission Strategy** (3-hour comprehensive tutorial)
2. **Admission Application Methodology**
3. **Gaokao Admission Pitfall Prevention Guide**
4. **Admission Information Channels**
5. **Admission Video Navigation**

All video transcript files are stored in `references/sources/transcripts/`

### Distillation Method

Adopts the **[Nuwa.skill](https://github.com/alchaincyf/nuwa-skill)** distillation methodology:

1. **Material Collection**: Bilibili videos → transcript extraction
2. **Deep Research**: 6-dimensional analysis
3. **Structured Distillation**: Mental models + decision heuristics + toolbox + expression DNA
4. **SKILL.md Writing**: Agent Skills standard-compliant executable file

[View full research reports →](references/research/)

---

## ⚠️ Limitations

### Applicable Scope
- ✅ Regular Gaokao college admission (old and new Gaokao systems)
- ✅ Students with autonomous decision-making awareness and willingness to research
- ✅ Acknowledges uncertainty and emphasizes fault-tolerant thinking

### Clear Limitations
1. **Cannot predict the future**: Major popularity and job markets are unpredictable four years out
2. **Limited cognition**: Students, parents, and Kuangkuang himself all have cognitive limitations
3. **Tool limitations**: Admission tools have fixed algorithms and cannot fully replace individual judgment
4. **Assessment limitations**: MBTI/career assessments are for reference only, not decision-making

**Core Principle**: This skill provides a decision-making framework, but the final decision must be yours.

---

## 🤝 Contributing

Contributions welcome! We especially need:

- 📝 **Updated materials**: New video transcripts from Kuangkuang, latest policy changes
- 🧠 **Methodology improvements**: Identified framework gaps or new mental models
- 🐛 **Issue reports**: Errors, outdated information, unclear expressions
- 💡 **Case sharing**: Real, effective dialogue examples

Please read [Contributing Guide](CONTRIBUTING.md) for detailed process.

---

## 📄 License

This project is open-sourced under [MIT License](LICENSE).

You are free to:
- ✅ Use, copy, modify this skill
- ✅ Use for personal or commercial purposes
- ✅ Redistribute

Only requirement:
- 📌 Retain original author attribution
- 📌 Include license copy

---

## 🙏 Acknowledgments

- Thanks to Bilibili creator **@取景框看世界 (Kuangkuang)** for years of public welfare sharing, lighting the way for countless students from ordinary families
- Thanks to **[Nuwa.skill](https://github.com/alchaincyf/nuwa-skill)** for providing the Agent Skills distillation methodology
- Thanks to all contributors who provided code, feedback, and shared cases for this project

---

<p align="center">
  <i>"Because I was once a child caught in the rain, I want to hold an umbrella for others."</i>
  <br>
  <i>—— Kuangkuang</i>
</p>

<p align="center">
  Made with ❤️ by <a href="https://github.com/alchaincyf">@alchaincyf</a>
</p>
