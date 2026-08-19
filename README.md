# CV Improvement Toolkit

A collection of prompts designed to help improve consultant CVs through structured review, feedback, rewriting, and assignment-specific analysis.

The toolkit is intended for consultants who want to strengthen their profiles before:

- Client presentations
- Job applications
- Consultant sales processes
- Interview processes
- Internal CV databases

---

# Repository Structure

| File | Purpose |
|--------|--------|
| `review.md` | Evaluates the CV from a consultant buyer perspective |
| `feedback.md` | Defines the feedback structure and scoring model |
| `rewrite.md` | Rewrites and strengthens the CV based on review findings |
| `analyze.md` | Compares the CV against a specific assignment or requirements profile |

---

# Recommended Workflow

The prompts are designed to be used in sequence.

```text
Current CV
    ↓
Review
    ↓
Feedback
    ↓
Rewrite
    ↓
Review Again
    ↓
Assignment Analysis
    ↓
Final CV
```

---

# Step 1 – Review the Current CV

## Goal

Understand how a consultant buyer perceives the CV.

## Use

- `review.md`
- `feedback.md`

## Input

```text
[Review Prompt]

[Feedback Prompt]

<Your CV>
```

## Questions Answered

- Is the profile relevant?
- Is the profile easy to understand?
- Does the CV create confidence?
- Would a client continue reading?

## Output

Examples:

- Strengths
- Weaknesses
- Risks
- Missing information
- General CV score

---

# Step 2 – Rewrite the CV

## Goal

Transform the feedback into an improved CV.

## Use

- `rewrite.md`

## Input

```text
[Rewrite Prompt]

Review Output

Current CV
```

## Questions Answered

- How can the summary be improved?
- How can assignments become more client-focused?
- How can consultant value become clearer?
- How can the profile become more commercially attractive?

## Output

Examples:

- Improved summary
- Better assignment descriptions
- Stronger consultant positioning
- Suggested headlines
- Prioritized improvement plan

---

# Step 3 – Review Again

## Goal

Validate that the rewritten version is actually better.

## Use

- `review.md`
- `feedback.md`

## Input

```text
[Review Prompt]

[Feedback Prompt]

Rewritten CV
```

## Questions Answered

- Did the CV improve?
- Are previous concerns addressed?
- What gaps remain?

## Output

A new score and updated recommendations.

---

# Step 4 – Assignment Analysis

## Goal

Evaluate how well the CV matches a specific role.

## Use

- `analyze.md`

## Input

```text
Assignment Description

Current CV
```

## Questions Answered

- How well does the CV match the assignment?
- What requirements are well supported?
- What evidence is missing?
- What should be emphasized?

## Output

Examples:

- Assignment match score
- Strengths against requirements
- Gaps against requirements
- Customization recommendations

---

# Example Workflow

## Scenario

A consultant wants to apply for a Microsoft Fabric Data Engineer assignment.

### Step 1

Review current CV.

Result:

```text
General CV Score: 3/5
```

Main findings:

- Strong technical background
- Limited focus on business value
- Few measurable outcomes

### Step 2

Rewrite assignments and summary.

Result:

- Improved consultant positioning
- More client-oriented wording
- Clearer value proposition

### Step 3

Review updated CV.

Result:

```text
General CV Score: 4/5
```

### Step 4

Analyze assignment fit.

Result:

```text
Assignment Score: 4/5
```

Missing:

- More examples of CI/CD
- More stakeholder interaction

Final action:

Update CV specifically for the assignment.

---

# Recommended Mindset

Do not treat the review score as the goal.

The goal is to answer:

> "Would a busy client or consultant buyer feel confident enough to move forward with this profile?"

A strong CV does not simply list technologies.

A strong CV clearly communicates:

- Problems solved
- Value delivered
- Consultant contribution
- Business impact
- Relevant expertise

---

# Tips

✅ Start with a strong "master CV"

✅ Review before rewriting

✅ Rewrite before tailoring

✅ Tailor before applying

✅ Focus on customer value, not technology lists

✅ Show outcomes whenever possible

❌ Do not invent experience

❌ Do not invent results

❌ Do not exaggerate responsibilities

❌ Do not optimize for score alone

---

# Suggested Iterative Process

```text
Master CV
    ↓
Review
    ↓
Rewrite
    ↓
Review Again
    ↓
Assignment Analysis
    ↓
Assignment-Specific CV
    ↓
Application
```

This process helps create a reusable consultant profile while making it easy to adapt for specific client opportunities.
