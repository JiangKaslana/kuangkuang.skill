# 框框·高考志愿填报顾问 Skill

> "志愿填报可能是你人生第一次真正掌握自己命运的方向盘。"

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-Standard-green)](https://agentskills.io)

基于 B 站 UP 主 **取景框看世界（框框）** 的高考志愿填报方法论，将系统化思考、个性化决策、容错导向和 2026 新资料整理为可按需加载的 AI Skill。

[English](README_EN.md) | [安装](#安装) | [资料库](#资料库) | [使用边界](#使用边界) | [贡献指南](CONTRIBUTING.md)

## 这个 Skill 做什么

它不是替学生拍板的"志愿答案机"，而是一个降低决策风险的顾问型 skill。它帮助 AI 在回答高考志愿问题时：

- 先问清省份、选科/科类、分数和位次、录取模式、经济压力、家庭资源、深造意愿和专业底线。
- 用框框方法论分析学校、专业、城市、分数段和录取规则的权衡。
- 按场景读取对应资料库，而不是一次性塞进全部知识。
- 对具体院校、专业、分数、薪资和政策始终要求回到官方来源核验。
- 保留学生自己的最终决策权。

## 核心方法论

| 模型 | 用途 |
|---|---|
| 四问自我定位 | 先判断经济条件、家庭资源、成绩分段、学习和深造能力 |
| 分层决策 | 高分段更看平台，中低分段更看专业；人文社科看学校，理工农科看专业，医科看地区 |
| 容错空间 | 不确定时优先保留转专业、跨考、深造和转行空间 |
| 成绩-深造匹配 | 避免中低分段、无深造意愿学生误入必须硕博才好就业的专业 |
| 决策权归属 | 家长、老师、机构、AI 都是参考，最终志愿必须由学生自己确认 |

## 安装

### 一键安装

```bash
npx skills add JiangKaslana/kuangkuang.skill
```

### 手动安装

```bash
git clone https://github.com/JiangKaslana/kuangkuang.skill.git
cp -r kuangkuang.skill ~/.codex/skills/kuangkuang-gaokao
```

安装后确认：

```bash
ls ~/.codex/skills/kuangkuang-gaokao/SKILL.md
```

如果你的运行环境使用 Claude Code、Cursor、Windsurf 或其他 Agent Skills 目录，请把仓库复制到对应的 skills 目录即可。

## 资料库

`SKILL.md` 是轻量导航入口，只保留触发描述、工作流、硬规则和资料路由。详细知识放在 `references/` 中按需加载。

### 结构

```text
kuangkuang.skill/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── examples/
├── references/
│   ├── database/
│   │   ├── 00-index.md
│   │   ├── application-workflow-2026.md
│   │   ├── city-selection-2026.md
│   │   ├── major-industry-guide.md
│   │   ├── risk-checklist.md
│   │   └── score-band-schools.md
│   ├── research/
│   │   ├── 01-core-methodology.md
│   │   ├── 02-information-strategy.md
│   │   ├── 03-expression-dna.md
│   │   ├── 04-values-mission.md
│   │   ├── 05-decision-heuristics.md
│   │   └── 06-honest-boundaries.md
│   └── sources/
│       └── transcripts/
│           └── 2026/
└── README.md
```

### `references/database/`

| 文件 | 适用问题 |
|---|---|
| `application-workflow-2026.md` | 2026 志愿填报流程、工具、位次法、线差法、位次转换法、冲稳保、调剂 |
| `city-selection-2026.md` | 适合读大学的城市、产业机会、城市/学校/专业权衡 |
| `score-band-schools.md` | 450-620 分本科候选池，300-500 分职业本科/高职候选池 |
| `major-industry-guide.md` | 普通家庭专业选择、央国企路径、未来行业和专业 |
| `risk-checklist.md` | 招生章程、服从调剂、提前批、野鸡大学、保存提交等避坑清单 |

### `references/research/`

保留原始方法论蒸馏报告，覆盖核心方法、信息策略、表达风格、价值观、决策启发式和诚实边界。

### 字幕源

2026 新增字幕源放在 `references/sources/transcripts/2026/`，覆盖：

- 2026 高考志愿填报全流程
- 适合读大学的城市
- 450-620 分宝藏本科
- 300-500 分职业本科/高职
- 普通家庭专业选择
- 未来十年行业和专业
- 志愿填报避坑

## 使用示例

可以这样提问：

```text
我是广东物化生考生，位次 48000，家里希望我本科就业，想在电气、计算机、自动化里选，应该怎么权衡？
```

```text
我想去杭州或南京读大学，分数够普通一本，学电子信息和计算机哪个更适合？
```

```text
院校专业组模式下，冲稳保和服从调剂怎么处理？
```

## 使用边界

- 不能保证录取结果。
- 不能预测四年后的就业市场。
- 不能只凭兴趣测试或 MBTI 帮人定专业。
- 不能让 AI、机构或家长替学生做最终决定。
- 所有学校、专业、薪资、排名、招生政策和特殊要求，都必须以当年省考试院、阳光高考、学校招生网和招生章程为准。

## 贡献

欢迎补充新字幕、更新政策变化、修正过时信息、添加真实对话案例。请先阅读 [CONTRIBUTING.md](CONTRIBUTING.md)。

问题反馈请使用 [GitHub Issues](https://github.com/JiangKaslana/kuangkuang.skill/issues)。

## 许可证

本项目采用 [MIT License](LICENSE)。

## 致谢

- 感谢 B 站 UP 主 **@取景框看世界（框框）** 多年来的公益分享。
- 感谢 **[女娲.skill](https://github.com/alchaincyf/nuwa-skill)** 提供的 Agent Skills 蒸馏方法论参考。

<p align="center">
  <i>"因为我是那个曾经淋过雨的小孩，所以我想为别人撑伞。"</i>
  <br>
  <i>-- 框框</i>
</p>
