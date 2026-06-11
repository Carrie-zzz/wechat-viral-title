---
name: aidd-viral-title
description: This skill should be used when the user asks to generate, optimize, score, or analyze WeChat public account article titles for the biotech, pharmaceutical, and AI drug discovery (AIDD) vertical. It should also be used when the user asks for viral title formulas, title writing methodology, clickbait optimization, or title analysis for biomedical and AI-pharma content. Triggers include keywords like "公众号标题", "爆款标题", "标题", "viral title", "clickbait", "title optimization", "AIDD", "生物医药", "AI制药", "drug discovery" in the context of content creation.
agent_created: true
---

# AIDD / 生物医药爆款标题生成器

## Overview

This skill enables the generation of high-click-through-rate (CTR) article titles for WeChat public accounts in the biotech, pharmaceutical, and AI drug discovery (AIDD) vertical. It provides 8 proven title formulas, a domain-specific keyword library, a taboo word checklist, and a 5-step execution workflow.

## Workflow Decision Tree

When the user asks for title-related help, determine the task type:

1. **Generate titles** → Follow "Generate Candidate Titles" workflow
2. **Optimize existing titles** → Follow "Score and Optimize" workflow
3. **Explain methodology** → Load `references/methodology.md` and explain key formulas
4. **Show examples** → Load `references/examples.md` and demonstrate with real cases
5. **Need interactive tools** → Copy `assets/title-toolkit.html` or `assets/title-scorer.html` to the workspace and present them

## Generate Candidate Titles

### Step 1: Understand the Content

Read or summarize the article content the user wants titles for. Identify:
- Core news/event/discovery
- Key entities (company, drug, target, method)
- Data points (phase, sample size, metrics)
- Emotional angle or controversy
- Target audience (scientists, investors, industry professionals)

### Step 2: Select Formulas

Load `references/methodology.md` to access the 8 title formulas. Based on content, select 2-4 most relevant formulas:

1. **Pipeline Milestone** — clinical data, regulatory approval, NDA/BLA
2. **Undruggable Breakthrough** — first-in-class, novel target, KRAS/MYC
3. **Methodology Comparison** — AI vs traditional, head-to-head
4. **Big Pharma Deep Dive** — internal report, exclusive, behind the scenes
5. **Academia-Industry Gap** — paper vs reality, SOTA vs wet lab
6. **Counter-Intuitive Discovery** — unexpected results, "but actually"
7. **Deal & Landscape Shift** — M&A, funding, partnership, IPO
8. **Personal Narrative** — "I interviewed", "I discovered", career story

### Step 3: Generate Candidates

For each selected formula, generate 2-3 candidate titles following these rules:

- **Length**: 15-25 Chinese characters (optimal for mobile display)
- **Front-loading**: Put the hook (number, question, key term) in the first 15 characters
- **Specificity**: Include concrete numbers (phase, percentage, sample size, dollar amount)
- **Information gap**: Use questions (吗, ？, 为什么) or悬念 words
- **Domain terms**: Use AIDD/pharma terminology to filter the right audience
- **Avoid taboos**: Never use "震惊", "颠覆", "神药", "治愈全世界"

### Step 4: Score and Rank

For each candidate title, score it using the 5-dimension system (100-point scale):

| Dimension | Max | Criteria |
|-----------|-----|----------|
| Length Control | 25 | ≤20 chars = 25; ≤25 = 20; ≤30 = 12; >30 = 5 |
| Concrete Numbers | 20 | Each number = 10 pts, max 20 |
| Emotion/Suspense | 20 | Each high-click word = 5 pts, max 20 |
| Information Gap | 15 | Contains ？/吗/为什么 = 15 |
| Domain Terminology | 10 | Contains AIDD/pharma terms = 10 |
| **Penalty** | - | Danger words = -10 each; Taboo phrases = -20 each |

### Step 5: Deliver

Present the top 3-5 titles with:
- Formula name matched
- Score (if calculated)
- One-line explanation of why it works
- If score < 60, provide improvement suggestions

## Score and Optimize

When the user provides an existing title:

1. Score it using the 5-dimension system above
2. Identify missing dimensions and specific issues
3. Provide 2-3 optimized versions targeting 60+ or 80+ scores
4. Explain what was changed and why

## Methodology Reference

For complete details on formulas, keyword libraries, and taboo lists, load `references/methodology.md`.

## Examples Reference

For real-world case studies (same news event written with 8 different formulas), load `references/examples.md`.

## Interactive Tools

When the user needs self-service tools:

- **Title Toolkit** (`assets/title-toolkit.html`): Formula quick-reference, title generator, keyword library, and self-check checklist in one interactive HTML page
- **Title Scorer** (`assets/title-scorer.html`): Input any title, get instant score (0-100), improvement suggestions, and formula matching

To use: Copy the HTML file to the user's workspace and open it with `preview_url`.

## Title Generation Checklist

Before finalizing any title, verify:
- [ ] Length is 15-25 characters
- [ ] First 15 characters contain a hook (number, question, or key term)
- [ ] Contains at least one concrete number or specific fact
- [ ] Contains at least one emotion/suspense word or a question mark
- [ ] Uses domain terminology appropriate for the audience
- [ ] Does NOT contain any danger words (震惊, 颠覆, 神药, 治愈, etc.)
- [ ] Does NOT contain any taboo phrases (AI颠覆药物研发, AI设计的药物, etc.)
- [ ] Matches at least one of the 8 formulas
- [ ] Would make the target reader feel "I must click to know more"
