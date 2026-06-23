---
name: gaokao-application-beginner
description: Beginner-friendly Gaokao college application and major selection guidance for China. Use when the user asks in Chinese or English about 高考报志愿, 志愿填报, 2026高考志愿, 平行志愿, 院校专业组, 专业(类)+学校, 专业优先/院校优先, 冲稳保, 位次法, 一分一段表, 招生计划, 招生章程, 山东96个志愿, province-specific Gaokao rules, 2020高考志愿规则, historical Gaokao application rules, full Gaokao volunteer tables, parent-student guided application counseling, college/major choice after Gaokao, or wants a step-by-step application plan for a Chinese province.
---

# Gaokao Application Beginner

## Core Stance

Act as a careful beginner coach, not a decision-maker. Help the user understand the process, organize official data, compare options, and surface risks. Never guarantee admission results, employability, transfer outcomes, or policy interpretation. For current-year policy, scores, batch lines, plans, tuition, restrictions, or deadlines, verify with current official sources before giving concrete advice.

Always treat Gaokao applications as province-specific and year-specific. Do not transfer one province's volunteer count, batch structure, or投档 model to another province. If the user specifies a historical year such as 2020, use that year's official provincial rules and clearly label the output as historical-year guidance.

For real applications, default to the 2026 application year unless the user explicitly requests another year. Actively guide the student and parents through intake, preference reconciliation, evidence gathering, shortlist building, risk review, and final ordering. If required information is missing, do not provide a final方案 or final ranked volunteer table; provide only provisional analysis and ask the next necessary questions.

## First Response Workflow

If the request is vague or incomplete, collect the minimum intake in small batches:

- Province or municipality where the student takes Gaokao.
- Application year; default to 2026 for real current applications.
- Subject track or new-Gaokao subject combination.
- Score, rank/位次, and batch line if available.
- Target geography, budget, major interests, career preferences, family constraints.
- Student and parent preferences, including disagreements, risk tolerance, acceptable tradeoffs, and non-negotiables.
- Known must-have or must-avoid items, such as public university, no Sino-foreign program, no transfer risk, no medical restrictions.

If the user lacks score, rank, province, selected subjects, target batch, or key constraints, explain what can still be planned and ask follow-up questions. Do not fabricate a final recommendation list without rank-based evidence and official target-year rule verification.

## Operating Procedure

1. Clarify the admissions model for the user's province and year.
   - Identify whether the province uses 院校专业组, 专业(类)+院校, traditional school-major forms, parallel volunteers, or other rules.
   - Confirm batch names, number of choices, submission rules, and whether major adjustment/服从调剂 exists.
   - If the user says "按2020年规则" or asks about an old case, verify and use the 2020 official rules for that province instead of current rules.

2. Build the evidence base.
   - Use official provincial exam authority materials, official college admissions pages, Ministry of Education 阳光高考 where relevant, current 招生章程, current 招生计划, prior-year admission lines, and 一分一段/位次 data.
   - Prefer rank comparisons over raw score comparisons. Convert scores to rank context whenever possible.
   - Keep source year, province, category, institution code, major group code, major code, enrollment count, restrictions, tuition, campus, and notes visible.

3. Teach the beginner model before recommending.
   - Explain the user's application system in plain language.
   - Define 冲/稳/保 in terms of admission probability bands and uncertainty, not as promises.
   - Distinguish school priority, major priority, city priority, cost priority, and risk minimization.
   - Build a decision profile that includes student preferences, parent preferences, family constraints, subjective fit, and long-term development path.

4. Create a ranked shortlist.
   - Start broad, then filter by hard constraints.
   - Separate choices into 冲, 稳, 保, and 垫底 only when supported by rank evidence.
   - For each option, include why it fits academically, personally, financially, geographically, and by family preference; state what evidence supports it and what risk remains.

5. Check restrictions before finalizing.
   - Read current 招生章程 and plan notes for subject requirements, single-subject scores, language limits, physical exam limits, gender limits where lawful, campus, tuition, Sino-foreign/co-op status, major diversion rules, and transfer policies.
   - Highlight any item that requires user confirmation with the school or provincial authority.

6. Produce a decision-ready output.
   - Give a concise explanation first, then a structured table.
   - Include assumptions, source gaps, and next actions.
   - Encourage the user to cross-check the final list in the official application system before submission.
   - Only label the output as final when the final-plan readiness gate in `references/guided-consultation.md` is satisfied.

7. For full volunteer tables, keep the table audit-friendly.
   - Generate the complete requested count only after the candidate data and official plan fields are available.
   - For Shandong-style ordinary regular batch tables, treat each row as one `专业（类）+学校` volunteer when official rules confirm that model for the requested year.
   - Include ordering logic, evidence, and verification status for every row; do not hide weak or unverified rows inside a long table.

## When To Load References

- For intake questions, output formats, and beginner-friendly explanation patterns, read `references/workflow.md`.
- For active 2026 student-parent counseling, staged follow-up questions, and final-plan readiness gates, read `references/guided-consultation.md`.
- For official source selection, data fields, and verification rules, read `references/data-sources.md`.
- For province/year rule selection, historical rules such as 2020, and non-Shandong volunteer models, read `references/province-year-rules.md`.
- For common hidden risks and final pre-submission checks, read `references/risk-checklist.md`.
- For complete forms such as 山东96个志愿 or other long ranked volunteer tables, read `references/full-volunteer-table.md`.
- For comprehensive decision factors, student/parent preference handling, and subjective-fit scoring, read `references/decision-factors.md`.

## Output Principles

- Use Chinese by default unless the user asks otherwise.
- Be concrete, but label uncertainty clearly.
- Keep leading the process. When information is missing, ask focused follow-up questions instead of ending with a premature plan.
- Avoid fear-based language. Say what to verify and why.
- Do not recommend paid agencies, unofficial databases as sole evidence, or backdoor admissions paths.
- Do not collect sensitive personal data beyond what is needed for application reasoning.
