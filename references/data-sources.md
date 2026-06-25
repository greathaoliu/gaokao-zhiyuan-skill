# Data Sources And Verification

## Source Priority

Use official sources for the target province and target year. For current applications, use current official sources; for historical simulations such as 2020, use archived official materials from that year.

1. Provincial education examination authority: application rules, dates, batch lines, 一分一段, official volunteer filling guides,招生计划 for the target year.
2. College undergraduate admissions website: target-year 招生章程 where available, province-specific plan, campus, tuition, subject requirements, special restrictions.
3. Ministry of Education 阳光高考 platform: college information, 招生章程, official policy pages when available.
4. Official application system or official printed/electronic plan book: final codes and plan counts.
5. Ministry of Education website and official releases: national admissions policies,普通高等学校名单,本科专业目录,新高考选科指引,双一流 or discipline-related official notices where relevant.
6. Provincial education department or municipal education commission: province-level policy interpretations, special-program notices, fee or student-status policy links when not hosted by the exam authority.
7. College academic official sources:教务处,本科生院,学院/系官网 for培养方案, major curriculum, major diversion, transfer policy, graduation requirements, accreditation notices, and campus training model.
8. Official employment and quality reports: college-issued就业质量报告,本科教学质量报告,毕业生去向落实 reports, and official career center pages. Use these for career-path discussion, not for admission-code verification.
9. Official accreditation or qualification sources when relevant: engineering education accreditation, medical education certification,师范类专业认证, law/medicine/teacher/civil-service qualification policy pages, or official industry regulator pages.
10. Official finance or school fee pages: college财务处/招生章程, provincial price/education departments, or official plan books for tuition,住宿费, and high-fee program confirmation.
11. Third-party databases: use only as convenience aids; verify important fields against official sources.

When the user asks for latest/current-year advice, browse or otherwise verify current official sources. When the user asks for 2020 or another historical year, verify archived official sources and label the year. Include source names and dates where practical.

## Source Tiers By Use

For final submission fields, use only official admissions sources:

- Province exam authority, official application system, official plan book.
- College admissions website and招生章程.
- Ministry of Education 阳光高考 when it hosts the official章程 or policy.

For decision quality and fit, use official supporting sources:

- Ministry of Education website for national institution, major, and policy information.
- College教务处/本科生院/学院官网 for curriculum, training plans, transfer rules, and major diversion.
- Official employment quality reports and career center pages for就业方向, postgraduate/employment proportions, and employer examples.
- Official accreditation or qualification bodies for majors tied to licensure or professional certification.

For convenience screening, third-party databases may be used only to discover candidates faster. Every final row must be traced back to official sources for rules, codes, plans, restrictions, and current-year details.

## Required Data Fields

For each candidate:

- Province, year, subject category or selected subjects.
- Score and province rank/位次.
- Relevant batch line, special control line, section line, and一分一段/rank context from official sources; the assistant should look these up after province/year/category are known.
- Hard constraints: region, budget, public/private, Sino-foreign/co-op, campus, medical limits, language, family constraints.
- Preference weights: school, major, city, employment, postgraduate path, cost, risk tolerance.

For each option:

- Institution name and code.
- Volunteer unit type: 院校专业组, 专业(类)+院校, 院校+专业, etc.
- Major or major group name and code.
- Target-year plan count in the user's province.
- Prior-year minimum rank and score for the same province/category/unit, ideally 2-3 years; include plan count for each year when available.
- Subject requirements, physical exam limits, single-subject requirements, foreign language limits.
- Tuition, campus, program type, major diversion or transfer policy.
- Curriculum/training model source when major fit is important.
- Employment or postgraduate-path source when career fit is part of the recommendation.
- Source and retrieval date.

## Rank-Based Comparison

Prefer 位次 over score:

- Compare candidate rank with prior admission ranks in the same province/category.
- Watch for changed volunteer unit definitions; old school-level lines may not match new major-group lines.
- Treat plan count changes, renamed major groups, new campuses, new programs, and major popularity shifts as uncertainty.
- Do not overfit one year of data. If only one year exists, say so.

For every final-table option, summarize the last 2-3 years of admission evidence where available:

- Use the same province, same subject category/selected-subject context, same batch, and same volunteer unit whenever possible.
- Keep yearly records separate: year, minimum score, minimum rank, plan count, and source.
- If the official historical data uses a different unit, label the mismatch, such as `2023为院校专业组口径，不等同于2026专业+学校`.
- If data is missing, use `未公开/暂未查到官方数据` and lower the confidence level instead of inventing or inferring a precise rank.
- Use third-party historical databases only to discover leads; verify final rows with official provincial or college sources when possible.

## Target-Year Verification Rules

Before final recommendations, verify:

- Official target-year batch lines, special control lines, section lines, and一分一段/rank data for the candidate's province/category.
- The province's target-year application policy and deadline.
- The target-year 招生计划 and codes.
- The target-year 招生章程 or archived equivalent.
- Any batch, major group, subject requirement, tuition, or campus changes.
- Whether the user's selected subjects satisfy every target option.
- Major diversion, transfer policy, and curriculum fit when the recommendation relies on major certainty.
- Tuition and fee source for every high-fee, private, or Sino-foreign/co-op option.

If browsing fails or sources are unavailable, clearly state which fields remain unverified and avoid presenting a final submission order.
