# 志愿填报资料库索引

Use this directory as the structured database for concrete 2026-oriented gaokao application questions. Load only the file that matches the user's current problem.

## Files

| File | Load when the user asks about |
|---|---|
| `application-workflow-2026.md` | 2026 志愿填报全流程、工具、专业排除、院校筛选、位次法/线差法/位次转换法、冲稳保、调剂模式、志愿表提交 |
| `city-selection-2026.md` | 哪些城市适合读大学、城市和产业机会、城市/学校/专业权衡、目标城市候选池 |
| `score-band-schools.md` | 450-620 分普通本科、300-500 分职业本科/高职/专科候选学校、按省份和行业特色找学校 |
| `major-industry-guide.md` | 普通家庭专业选择、AI 时代稳就业、央国企路径、未来 10 大行业和专业、专业风险与适配 |
| `risk-checklist.md` | 十大志愿填报坑、招生章程、服从调剂、提前批、野鸡大学、手机填报、保存提交、决策权 |

## Source transcripts

New 2026 subtitle sources are archived in `references/sources/transcripts/2026/`:

- `一个视频讲透2026高考志愿填报的一切！所有省份适用！ 中文.srt`
- `15分钟速通所有适合读大学的城市！ 中文.srt`
- `450-620分？这50所宝藏本科你一定要知道！ 中文.srt`
- `300-500分，这些宝藏学校你一定得知道！ 中文.srt`
- `家里没钱的普通人，专业求你别瞎选啊啊啊！ 中文.srt`
- `填志愿必看，未来十年最稳的10大行业50个专业！ 中文.srt`
- `高考填志愿有这些坑，你千万不要踩啊！ 中文.srt`

## Database Use Rules

- Treat all school, major, salary, rank, and industry claims as leads for further verification.
- For any final application advice, require current-year招生计划,招生章程,省考试院政策, and the student's rank/位次.
- When lists include schools or majors, present them as候选池, not as final picks.
- When a question crosses domains, load the narrowest additional file. Example: "家里没钱，想去杭州学 AI" needs `major-industry-guide.md` plus the杭州 row in `city-selection-2026.md`.
