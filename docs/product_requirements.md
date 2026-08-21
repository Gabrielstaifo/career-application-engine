# Product Requirements Document (PRD)

## Project Name

Career Application Engine

---

# Overview

Career Application Engine is an AI-powered CV optimization workflow designed to help job seekers improve their CVs and increase their chances of being invited to interviews.

The application focuses on analyzing job advertisements, reviewing CVs, identifying requirement gaps, and generating tailored CV recommendations.

The initial version (MVP) follows a structured AI Workflow rather than a fully autonomous agent architecture.

---

# Problem Statement

Many candidates struggle to:

- Understand what employers are actually looking for
- Adapt their CVs to specific opportunities
- Identify missing skills or evidence
- Present their experience effectively
- Communicate business value rather than tasks

As a result, qualified candidates are often rejected before reaching the interview stage.

---

# Target Audience

Primary users:

- Job seekers
- Data and IT professionals
- Newly graduated professionals

Secondary users:

- Consultants
- Career changers
- Technical specialists

---

# Product Goal

The goal is to increase interview opportunities by generating a stronger, more targeted CV based on a specific job advertisement.

---

# User Inputs

## CV

The user must provide a CV using one of the following methods:

### Option A

Paste CV text directly into the application.

### Option B

Upload a CV file.

Supported formats:

- PDF
- DOCX

---

## Assignment Description

Required.

The user must provide a complete job advertisement, assignment description, or requirements profile.

This can be entered via:

- Text input

The workflow cannot start without an assignment description.

---

# User Flow

```text
Provide CV
        ↓
Provide Job Advertisement
        ↓
Run Full Workflow
        ↓
Receive Results
```

---

# Output Deliverables

## 1. Review Report

Purpose:

Evaluate the current CV.

Contains:

- CV Score
- Strengths
- Weaknesses
- Risks
- Missing Evidence

---

## 2. Improved CV

Purpose:

Generate a stronger version of the CV.

Contains:

- Improved Summary
- Improved Assignment Descriptions
- Better Consultant Positioning
- Improved Value Communication

---

## 3. Assignment Match Report

Purpose:

Evaluate how well the CV matches the job advertisement.

Contains:

- Match Score
- Must-Have Match Analysis
- Nice-To-Have Match Analysis
- Requirement Coverage
- Risk Areas

---

## 4. Gap Analysis

Purpose:

Identify missing or weakly supported requirements.

Contains:

### Strong Match

Requirements clearly supported by the CV.

### Partial Match

Requirements with limited evidence.

### Missing Evidence

Requirements not supported by the CV.

### Recommendations

Suggested improvements.

---

# MVP Features

## Included

✅ Paste CV

✅ Upload PDF

✅ Upload DOCX

✅ Mandatory Job Advertisement

✅ Run Full Workflow

✅ Review Report

✅ Improved CV

✅ Assignment Match Report

✅ Gap Analysis

✅ Markdown Export

---

## Not Included

❌ User Editing Inside App

❌ DOCX Export

❌ PDF Export

❌ Job Search

❌ Interview Preparation

❌ Cover Letter Generation

❌ Agentic Reasoning

❌ Multi-Agent Architecture

---

# Master CV Support

The application should support a reusable Master CV.

Purpose:

Provide a single source of truth that can be adapted for different opportunities.

Future versions may allow:

- Saving Master CV
- Versioning
- Historical tracking

---

# Success Criteria

The application succeeds when users can:

- Understand how their CV is perceived
- Improve the quality of their CV
- Better match job requirements
- Identify missing evidence
- Produce a tailored CV more efficiently

---

# Future Roadmap

## Version 2

- DOCX Export
- PDF Export
- Cover Letter Generation

---

## Version 3

- Interview Preparation
- LinkedIn Optimization
- Career Recommendations

---

## Version 4

- Agentic Workflow
- Autonomous Decision Making
- Multi-Agent Collaboration

Examples:

- Job Analysis Agent
- CV Review Agent
- CV Rewrite Agent
- Match Analysis Agent

---

# Guiding Principles

- Improve clarity
- Improve relevance
- Improve credibility
- Improve interview opportunities
- Never invent experience
- Never invent achievements
- Prioritize truth over marketing
