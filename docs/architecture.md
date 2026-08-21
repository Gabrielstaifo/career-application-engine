# Architecture Document

## Project Name

Career Application Engine

---

# Architecture Overview

The system follows an AI Workflow architecture.

The workflow is deterministic and user-driven.

The user provides the inputs.

The system executes a predefined sequence of AI-powered analysis steps.

---

# High-Level Flow

```text
User
 ↓
CV Input
 ↓
Assignment Input
 ↓
Run Full Workflow
 ↓
Job Advertisement Analysis
 ↓
CV Review
 ↓
CV Rewrite
 ↓
Assignment Match Analysis
 ↓
Gap Analysis
 ↓
Results
```

---

# System Components

## Frontend

Technology:

```text
Streamlit
```

Responsibilities:

- Display user interface
- Accept input
- Display results
- Trigger workflow execution

---

## Workflow Engine

Technology:

```text
Python
```

Responsibilities:

- Coordinate workflow
- Load prompts
- Execute AI calls
- Pass outputs between modules

---

## Prompt Layer

Location:

```text
prompts/
```

Components:

### Job Advertisement Analyzer

Input:

- Assignment Description

Output:

- Requirements Analysis

---

### CV Reviewer

Input:

- CV
- Assignment Description

Output:

- Review Report

---

### Feedback Structure

Input:

- Review Findings

Output:

- Structured Feedback

---

### CV Rewrite Recommendations

Input:

- CV
- Review Results

Output:

- Improved CV

---

# Workflow Modules

## Module 1

Job Advertisement Analysis

Purpose:

Extract:

- Must-Have Skills
- Nice-To-Have Skills
- Keywords
- Risks

Output:

Requirements Profile

---

## Module 2

CV Review

Purpose:

Evaluate CV quality.

Output:

Review Report

---

## Module 3

CV Rewrite

Purpose:

Generate an improved CV.

Output:

Improved CV

---

## Module 4

Assignment Match

Purpose:

Compare CV against requirements.

Output:

Match Report

---

## Module 5

Gap Analysis

Purpose:

Identify:

- Missing Skills
- Missing Evidence
- Weak Areas

Output:

Gap Report

---

# Input Sources

## CV

Supported formats:

### Text Input

```text
Paste CV
```

### File Upload

```text
PDF
DOCX
```

---

## Assignment Description

Required.

Supported format:

```text
Text Input
```

---

# Output Objects

## Review Report

Markdown

---

## Improved CV

Markdown

---

## Assignment Match Report

Markdown

---

## Gap Analysis

Markdown

---

# File Structure

```text
career-application-engine/

├── README.md
│
├── docs/
│   ├── product_requirements.md
│   └── architecture.md
│
├── prompts/
│   ├── CV Reviewer.md
│   ├── Feedback Structure.md
│   ├── CV Rewrite Recommendations.md
│   └── Job Advertisement Analyzer.md
│
├── templates/
│   └── master_cv_template.md
│
├── examples/
│   ├── sample_cv.md
│   ├── sample_assignment.md
│   └── sample_output.md
│
├── app/
│   ├── app.py
│   ├── services/
│   └── assets/
│
└── outputs/
```

---

# LLM Layer

The system should support interchangeable providers.

Design Principle:

```text
Pluggable LLM Provider
```

Supported providers may include:

- Groq
- Gemini
- OpenRouter
- OpenAI
- Azure OpenAI

The rest of the application should not depend on a specific provider.

---

# State Management

MVP:

```text
Session-Based
```

The application stores data during the workflow execution only.

---

# Master CV Strategy

Future versions should support:

```text
Master CV
```

Capabilities:

- Load Master CV
- Reuse Master CV
- Generate Opportunity-Specific CVs

Master CV acts as the system's source of truth.

---

# Future Architecture

## Phase 2

Enhanced Workflow

```text
Job Analysis
 ↓
Review
 ↓
Rewrite
 ↓
Match
 ↓
Gap
```

with improved exports.

---

## Phase 3

Agentic Workflow

```text
Career Application Agent
```

Responsibilities:

- Decide next actions
- Select prompts
- Coordinate workflow

---

## Phase 4

Multi-Agent System

```text
Job Analysis Agent

CV Review Agent

CV Rewrite Agent

Assignment Match Agent

Gap Analysis Agent
```

Agents collaborate to generate a complete application package.

---

# Architectural Principles

- Modular Design
- Prompt Driven
- Provider Agnostic
- Extendable
- Testable
- Reusable
- Human-In-The-Loop
- AI-Assisted

