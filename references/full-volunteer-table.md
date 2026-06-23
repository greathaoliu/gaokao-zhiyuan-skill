# Full Volunteer Table

Use this reference when the user asks for a complete ranked volunteer form, such as 山东普通类常规批 96 个志愿.

## Non-Negotiable Accuracy Rule

Separate two meanings of "accurate":

- Data accuracy: codes, plans, restrictions, tuition, campus, subject requirements, and source citations must be verified against current official sources before labeling the table final.
- Admission accuracy: never promise admission. Estimate risk from rank evidence, plan changes, and preference constraints.

If current official data is unavailable, output a `草案/研究表` and mark unverified fields. Do not call it a final submission table.

If the final-plan readiness gate in `guided-consultation.md` is not satisfied, do not output a complete final ranked table. Ask for the missing information and, at most, provide a partial research table or candidate-pool framework.

## Required Inputs Before A 96-Row Table

Collect or derive:

- Province and application year.
- Batch and volunteer model, such as 山东普通类常规批 and `专业（类）+学校`.
- Candidate score, province rank, selected subjects, and relevant lines.
- Preference weights and exclusions, including student and parent views.
- Official current-year plan data with school/major codes.
- Prior admission data by the same province/category/volunteer unit where available.

For Shandong-like `专业（类）+学校`, each row should represent one major or major category at one school, not only a school.

## Table Columns

Use these columns for a complete table:

| 序号 | 梯度 | 院校代码 | 院校名称 | 专业/专业类代码 | 专业/专业类名称 | 计划数 | 选科要求 | 往年最低位次 | 位次差 | 学费/校区 | 学生匹配 | 家长关注 | 核验状态 | 排序理由 | 风险提示 |
|---|---|---|---|---|---|---:|---|---:|---:|---|---|---|---|---|---|

Keep rows concise. Put long explanations below the table rather than bloating every cell.

## Suggested 96-Row Structure

Adjust by risk tolerance and evidence quality:

- 冲: about 15-25 rows. Use only where the user accepts uncertainty.
- 稳: about 35-45 rows. Prioritize fit and realistic rank evidence.
- 保: about 20-30 rows. Make these meaningfully safer, not just slightly lower.
- 垫底: about 5-10 rows. Use for strong anti-slip protection.

If the user is very risk-averse, shift rows from 冲 to 保/垫底. If the user is major-first, reduce school-reputation chasing and add more same-major alternatives.

## Build Procedure

1. Confirm current official rules for the province/year/batch.
2. Filter by selected subjects and hard constraints.
3. Create a broad candidate pool larger than the final count.
4. Assign preliminary risk bands using rank evidence.
5. Remove rows with unacceptable restrictions, costs, campus, or program type.
6. Score subjective fit using the student/parent preference profile; mark unresolved preference conflicts.
7. Sort within each band by the user's stated priorities.
8. Fill exactly the requested row count only after conservative options are sufficient.
9. Mark each row as one of:
   - `已核验`: current official plan and章程-sensitive fields checked.
   - `待核验`: likely candidate but official current-year field missing.
   - `不建议提交`: unresolved hard risk; keep only if explaining exclusion.

## Final Output

Before the table, state:

- Data sources and retrieval dates.
- Whether it is `最终核验版`, `可提交前复核版`, or `研究草案`.
- The candidate assumptions used.

After the table, include:

- 5-10 highest-risk rows needing manual confirmation.
- Any rows removed and why, if important.
- Student-parent preference conflicts that still need a family decision.
- A final checklist for official application-system cross-checking.
