# Province And Year Rules

Use this reference whenever the user gives a province, asks for a province-specific plan, or asks to use a historical year such as 2020.

## Rule Selection Principle

Every plan must bind to a specific province and year:

```text
规则版本 = 考生所在省份 + 招生年份 + 批次/类别
```

Do not infer a province's rules from another province. Shandong's `专业（类）+学校` and 96-volunteer ordinary regular batch model is only one possible pattern. Other provinces may use 院校专业组, 院校+专业, 专业+院校, sequential志愿, parallel志愿, different batch names, different volunteer counts, and different服从调剂 mechanics.

## Historical-Year Handling

If the user requests a historical year, such as "按2020年规则":

1. Treat 2020 as the target rules year.
2. Search or consult official archived provincial education exam authority materials for that province and year.
3. Use 2020 batch names, volunteer counts,志愿单位,投档 rules, score/rank data,招生计划, and章程-sensitive restrictions where available.
4. Clearly label the output as `按2020年规则复盘/模拟`, not current-year advice.
5. Do not mix 2020 rules with current-year plans or current major codes unless the user explicitly asks for a comparison.

If the user wants to apply now, use the current application year rules instead; 2020 rules can be used only as background or comparison.

## Rule Intake Questions

When province/year/rule version is unclear, ask:

```text
你希望我按哪个规则版本来做？
1. 考生所在省份：
2. 招生年份：例如 2020、2024、2026
3. 类别/批次：普通类本科批、普通类常规批、专科批、提前批、艺术/体育等
4. 是真实填报，还是用历史规则复盘/模拟？
```

## Rule Fields To Verify

For the selected province/year/batch, verify:

- Volunteer unit: 院校、院校专业组、专业（类）+学校、专业+院校, or another official unit.
- Number of volunteers and number of majors per volunteer unit.
- Parallel or sequential submission.
- Whether服从调剂 exists and its scope.
- Batch names and filing/录取 sequence.
- Score/rank conversion and whether rank is published by category.
- Special rules for提前批,专项计划,地方专项,公费师范,军警,艺术,体育,春季高考,综合评价,强基计划.
- Official source date and document title.

## Output For Non-Shandong Provinces

Adapt the table to the official volunteer unit:

- `专业（类）+学校`: one row is one major/category at one school.
- `院校专业组`: one row is one school professional group; include majors inside the group and调剂 risk.
- `院校+专业`: one row may represent one institution volunteer with several major choices; include major order and服从调剂.
- Sequential志愿: emphasize first-choice priority and avoid using parallel志愿排序 logic.

For each province, table columns should match the official unit. Do not force a 96-row table unless the official model and requested batch support it.

## Current-Year Versus 2020 Warning

Rules after 2020 may differ because of new Gaokao reforms, batch mergers, subject requirement updates, plan changes, and volunteer-unit changes. When answering, explicitly state which rule year is being used and avoid cross-year assumptions.
