# Career Application Engine

A structured AI-powered workflow for analyzing job opportunities, improving CVs, tailoring applications, and preparing for interviews.

This repository helps consultants, engineers, specialists, and job seekers systematically move from a generic master CV to a targeted application package.

The goal is not simply to improve a CV.

The goal is to maximize the likelihood of:

- Passing CV screenings
- Matching job requirements
- Being shortlisted
- Securing interviews
- Increasing consultant marketability
- Presenting a clear and credible professional profile

---

# Repository Structure

```text
career-application-engine/

├── README.md
│
├── examples/
│   ├── sample_cv.md
│   ├── sample_assignment.md
│   └── sample_output.md
│
├── prompts/
│   ├── CV Reviewer.md
│   ├── CV Rewrite Recommendations.md
│   ├── Feedback Structure.md
│   └── Job Advertisement Analyzer.md
│
└── templates/
    └── master_cv_template.md
```

---

# Purpose of Each Folder

## examples/

Contains example files that demonstrate how the workflow can be used.

| File | Purpose |
|--------|--------|
| `sample_cv.md` | Example consultant CV |
| `sample_assignment.md` | Example assignment or job advertisement |
| `sample_output.md` | Example AI-generated output |

---

## prompts/

Contains the core prompts used throughout the workflow.

| Prompt | Purpose |
|----------|----------|
| `Job Advertisement Analyzer.md` | Analyzes job advertisements and identifies key requirements |
| `CV Reviewer.md` | Evaluates CV quality and marketability |
| `Feedback Structure.md` | Provides standardized scoring and review criteria |
| `CV Rewrite Recommendations.md` | Generates rewrite recommendations and improvement suggestions |

---

## templates/

Contains reusable templates that serve as source material for future applications.

| Template | Purpose |
|------------|------------|
| `master_cv_template.md` | Master CV template containing the candidate's complete experience |

---

# Recommended Workflow

The prompts are intended to be used in the following order.

```text
Job Advertisement
        ↓
Job Advertisement Analysis
        ↓
CV Review
        ↓
Feedback
        ↓
CV Improvement
        ↓
CV Review Again
        ↓
Application-Specific CV
        ↓
Application Submission
```

---

# Step 1 - Analyze the Job Advertisement

## Goal

Understand what the employer is actually looking for before modifying the CV.

Most candidates immediately start editing their CV.

A better approach is to first analyze:

- Must-have requirements
- Nice-to-have requirements
- Business challenges
- Important keywords
- Potential rejection factors

## Use

```text
prompts/Job Advertisement Analyzer.md
```

## Input

```text
<Job Advertisement>
```

## Output

Examples:

- Role summary
- Required skills
- Nice-to-have skills
- Keywords
- Hidden requirements
- Risk factors
- Interview focus areas

---

# Step 2 - Review the Current CV

## Goal

Understand how the current profile is perceived by a recruiter, consultant manager, or hiring manager.

## Use

```text
prompts/CV Reviewer.md

prompts/Feedback Structure.md
```

## Input

```text
<Current CV>
```

## Questions Answered

- Is the profile credible?
- Is the value proposition clear?
- Does the CV create confidence?
- Would a recruiter continue reading?

## Output

Examples:

- Strengths
- Weaknesses
- Missing evidence
- Risks
- General CV score

---

# Step 3 - Improve the CV

## Goal

Transform review findings into actionable improvements.

## Use

```text
prompts/CV Rewrite Recommendations.md
```

## Input

```text
Current CV

Review Results

Feedback Results
```

## Questions Answered

- How can the summary be improved?
- How can achievements become clearer?
- How can assignments become more client-oriented?
- How can commercial value be strengthened?

## Output

Examples:

- Improved summary
- Rewritten assignment descriptions
- Better positioning
- Prioritized improvement plan

---

# Step 4 - Review Again

## Goal

Validate that the revised version is stronger than the original.

## Use

```text
prompts/CV Reviewer.md

prompts/Feedback Structure.md
```

## Input

```text
Improved CV
```

## Questions Answered

- Did the score improve?
- Were the major weaknesses resolved?
- What still needs attention?

## Output

Updated assessment and recommendations.

---

# Step 5 - Tailor the CV to the Opportunity

## Goal

Create a targeted version of the CV based on the analyzed requirements.

Use findings from:

- Job Advertisement Analysis
- CV Review
- Rewrite Recommendations

Focus on:

- Relevant experience
- Appropriate keywords
- Business value
- Requirement alignment

## Output

A customized CV designed for a specific opportunity.

---

# Example Workflow

## Scenario

A Data Engineer wants to apply for a Microsoft Fabric role.

### Step 1

Analyze the advertisement.

Result:

```text
Core Skills:
- Microsoft Fabric
- Azure
- SQL
- Python

Preferred:
- Terraform
- Databricks
```

### Step 2

Review current CV.

Result:

```text
General CV Score: 3/5
```

Findings:

- Strong technical background
- Limited business impact
- Few measurable outcomes

### Step 3

Improve CV.

Result:

- Stronger value proposition
- Better assignment descriptions
- Improved consultant positioning

### Step 4

Review revised version.

Result:

```text
General CV Score: 4/5
```

### Step 5

Tailor CV against job requirements.

Result:

```text
Opportunity Match: Strong
```

Recommended focus:

- Fabric projects
- Data platform delivery
- Stakeholder collaboration
- CI/CD examples

---

# Recommended Mindset

Do not optimize for a score.

Optimize for confidence.

The key question is:

> "Would a busy recruiter, consultant manager, or hiring manager feel confident enough to move forward with this profile?"

Strong CVs are not technology inventories.

Strong CVs communicate:

- Problems solved
- Business value
- Responsibilities
- Outcomes
- Relevant expertise
- Delivery capability

---

# Best Practices

✅ Maintain a single master CV

✅ Analyze the opportunity before tailoring

✅ Review before rewriting

✅ Rewrite before applying

✅ Highlight business value

✅ Demonstrate outcomes whenever possible

✅ Stay factually accurate

❌ Do not invent experience

❌ Do not invent results

❌ Do not exaggerate responsibilities

❌ Do not optimize solely for keywords

❌ Do not tailor before understanding the role

---

# Suggested Iterative Process

```text
Master CV
        ↓
Job Advertisement Analysis
        ↓
CV Review
        ↓
CV Improvement
        ↓
CV Validation
        ↓
Opportunity-Specific CV
        ↓
Application
        ↓
Interview
```

The repository is designed to support a repeatable and structured process that turns a generic CV into a targeted, credible, and competitive application.
