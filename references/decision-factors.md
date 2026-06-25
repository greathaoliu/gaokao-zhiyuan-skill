# Decision Factors

Use this reference when building a comprehensive Gaokao application strategy. The goal is to make hidden preferences explicit, not to pretend subjective values are objective facts.

## Factor Map

Consider these categories before final ordering:

- Admission evidence: score, rank, batch line, prior ranks, plan count, policy changes, volunteer model.
- Major fit: interest, subject strength, learning style, curriculum, math/physics/English load, lab/fieldwork/clinical demands, certification requirements.
- School fit: academic level, discipline strength, teaching quality signals, postgraduate pathways, transfer policy, major diversion policy, campus culture.
- City and region: distance from home, climate, language/dialect, cost of living, internship density, industry cluster, future settlement possibility.
- Career path: employment direction, civil service/teacher/medical/legal/engineering certification path, postgraduate necessity, industry cyclicality, family network relevance.
- Career targets: high salary, stability, city opportunity, public-sector exam, state-owned enterprise, hospital, power grid, finance, internet, chip/semiconductor, teacher track, or "undecided".
- Family finance: tuition, accommodation, living costs, travel costs, private/Sino-foreign/co-op fees, ability to support postgraduate study.
- Student fit and wellbeing: strong/weak subjects, coding tolerance, memorization tolerance, long-term study tolerance, independence, mental pressure tolerance, health, social support, adaptation to far-away cities, campus size, schedule intensity.
- Parent preferences: distance, safety, school reputation, major stability, employment expectations, budget, relatives nearby, willingness to accept uncertainty.
- Hard restrictions: selected subjects, physical exam restrictions, single-subject requirements, language limits, gender limits where officially stated, political review where relevant.
- Risk tolerance: whether the family values a higher ceiling, major certainty, city certainty, low退档 risk, or low滑档 risk.

## Intake Questions For Subjective Factors

Ask concise questions when subjective priorities are unclear:

```text
除了分数位次，我还需要了解这些偏好，方便把 96 个志愿排得更贴近你们家：
1. 学生最想学和最不想学的专业分别是什么？
2. 家长最看重学校层次、专业就业、城市距离、费用里的哪两个？
3. 能接受离家多远？有没有必须避开的城市或地区？
4. 能否接受民办、中外合作、高收费、不同校区？
5. 更怕“没录上/滑档”，还是更怕“录到不喜欢的专业”？
6. 本科就业、考研、考公、出国、进体制，哪个方向更倾向？
7. 家庭有没有行业资源、亲友照应、经济上限或健康因素需要考虑？
```

Use one-question micro-intake by default. Do not ask this full list unless the user requests a full questionnaire.

## Preference Weighting

When enough information exists, create a simple weight profile:

| 因素 | 权重 | 学生意见 | 家长意见 | 结论 |
|---|---:|---|---|---|
| 专业适配 | 25% | ... | ... | ... |
| 院校层次 | 20% | ... | ... | ... |
| 城市/距离 | 15% | ... | ... | ... |
| 录取稳健 | 20% | ... | ... | ... |
| 费用/家庭资源 | 10% | ... | ... | ... |
| 长期路径 | 10% | ... | ... | ... |

Adjust weights to the family. Do not force these defaults if the user states different priorities.

## Parent-Student Conflict Handling

When student and parent preferences conflict:

1. Name the conflict neutrally.
2. Identify whether it is a hard constraint, a risk concern, or a preference.
3. Offer two or three viable strategies with tradeoffs.
4. Keep final ordering aligned with the explicitly chosen strategy.

Common conflict patterns:

- Student wants interest, parents want employment stability: compare curriculum, career routes, and fallback options.
- Student wants far-away city, parents want nearby: keep a controlled number of far-away choices and ensure strong local保底.
- Parents want famous school, student wants specific major: split 冲 rows toward school and 稳/保 rows toward major certainty.
- Family wants low risk, student wants high ceiling: reduce 冲比例 and use only evidence-backed冲.

## Subjective Fit Notes In Tables

For each recommended option, include a short fit note when useful:

- `学生匹配`: why the major/city/learning style fits the student.
- `家长关注`: how it addresses distance, cost, employment, school level, or safety concerns.
- `取舍`: what is being sacrificed, such as school rank, major certainty, city, cost, or risk.

If subjective information is missing, mark `偏好待确认` instead of guessing.

## Red Flags

Treat these as reasons to pause or ask follow-up questions:

- The student strongly rejects the major but the table includes it only because the school is famous.
- Parents reject the cost or distance but the plan relies on many such rows.
- Every保底 row has a hidden unacceptable condition.
- The family says "anything is fine" but later gives absolute exclusions.
- The plan maximizes admission probability while ignoring major diversion or transfer difficulty.
