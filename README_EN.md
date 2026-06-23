# Kuangkuang Gaokao Application Advisor Skill

> "Gaokao application may be the first time you truly hold the steering wheel of your own life."

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-Standard-green)](https://agentskills.io)

An Agent Skill based on the gaokao application methodology of **取景框看世界 / Kuangkuang**. It turns decision frameworks, risk checks, city/major/school tradeoffs, and 2026 subtitle-derived references into a progressively loaded advisor skill.

[中文](README.md) | [Installation](#installation) | [Reference Database](#reference-database) | [Boundaries](#boundaries) | [Contributing](CONTRIBUTING.md)

## What This Skill Does

This skill is not an "answer machine" that chooses applications for students. It helps an AI:

- Ask for high-impact facts first: province, subject selection, score/rank, admission mode, financial pressure, family resources, deep-study willingness, and major bottom line.
- Analyze school, major, city, score-band, and admission-rule tradeoffs with Kuangkuang's risk-aware framework.
- Load only the reference file needed for the current question.
- Treat school, major, score, salary, ranking, and policy claims as leads that require official verification.
- Keep the student's final decision ownership intact.

## Core Models

| Model | Purpose |
|---|---|
| Four self-positioning questions | Check finances, usable family resources, score tier, and learning/deep-study capacity |
| Layered decisions | High score often values platform; middle/low score often values major; humanities value school network; engineering values major fit; medicine is region-bound |
| Error-tolerance space | Prefer choices that preserve transfer, cross-exam, postgraduate, and career-pivot options |
| Score-depth match | Avoid majors that require master's/PhD outcomes when the student cannot support that path |
| Decision ownership | Parents, teachers, agencies, and AI are references; the student must own the final list |

## Installation

### One-command install

```bash
npx skills add JiangKaslana/kuangkuang.skill
```

### Manual install

```bash
git clone https://github.com/JiangKaslana/kuangkuang.skill.git
cp -r kuangkuang.skill ~/.codex/skills/kuangkuang-gaokao
```

Verify:

```bash
ls ~/.codex/skills/kuangkuang-gaokao/SKILL.md
```

For Claude Code, Cursor, Windsurf, or other Agent Skills runtimes, copy the repository into the relevant skills directory.

## Reference Database

`SKILL.md` is now a lightweight navigation entry. It keeps triggering metadata, workflow, hard rules, and routing instructions. Detailed knowledge lives under `references/`.

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

### Database Files

| File | Use for |
|---|---|
| `application-workflow-2026.md` | 2026 application workflow, tools, rank method, line-difference method, rank-conversion method, safety strategy, adjustment rules |
| `city-selection-2026.md` | University city choice, industry opportunities, city/school/major tradeoffs |
| `score-band-schools.md` | 450-620 undergraduate candidates and 300-500 vocational college candidates |
| `major-industry-guide.md` | Ordinary-family major choice, SOE/public-sector paths, future industries and majors |
| `risk-checklist.md` | Admission charter, adjustment, early batch, fake universities, final submission checks |

### Research Files

`references/research/` keeps the original distilled methodology: core models, information strategy, expression style, values, heuristics, and honest boundaries.

### Transcript Sources

New 2026 subtitle sources are archived in `references/sources/transcripts/2026/`, covering:

- Full 2026 gaokao application workflow
- Best cities for university study
- 450-620 score-band undergraduate schools
- 300-500 score-band vocational schools
- Major choice for ordinary families
- Future industries and majors
- Application pitfalls

## Example Prompts

```text
I am a Guangdong physics-chemistry-biology student, rank 48000. My family hopes I can work after undergrad. How should I compare electrical engineering, computer science, and automation?
```

```text
I want to study in Hangzhou or Nanjing. My score is around a regular first-tier undergraduate range. Should I prefer electronic information or computer science?
```

```text
How should I handle reach/match/safety choices and adjustment in the "college + major group" admission mode?
```

## Boundaries

- Do not promise admission outcomes.
- Do not predict the job market four years from now with certainty.
- Do not choose a major only from interest tests or MBTI.
- Do not let AI, agencies, or parents replace the student's final decision.
- Verify all schools, majors, salaries, rankings, admission rules, and special requirements through current-year official sources: provincial exam authority, 阳光高考, school admission websites, and admission charters.

## Contributing

Contributions are welcome: new subtitles, policy updates, outdated information fixes, and realistic conversation examples. See [CONTRIBUTING.md](CONTRIBUTING.md).

Report issues at [GitHub Issues](https://github.com/JiangKaslana/kuangkuang.skill/issues).

## License

This project is licensed under the [MIT License](LICENSE).

## Thanks

- Thanks to Bilibili creator **@取景框看世界（框框）** for years of public-interest sharing.
- Thanks to **[Nuwa.skill](https://github.com/alchaincyf/nuwa-skill)** for the Agent Skills distillation methodology reference.
