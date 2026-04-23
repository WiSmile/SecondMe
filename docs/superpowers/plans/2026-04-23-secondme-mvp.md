# SecondMe MVP Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build the first documentation-driven MVP of SecondMe as a personal AI company.

**Architecture:** Use directories as departments and Markdown files as the first system of record. Keep harness as a documented execution boundary for now, not an automated runtime.

**Tech Stack:** Markdown, git, local filesystem.

---

### Task 1: Create Department Structure

**Files:**
- Create directories from `00-governance` through `10-harness`
- Create `inbox`, `workspace`, `logs`, and `docs`

- [x] **Step 1: Create directories**

Run:

```bash
mkdir -p 00-governance 01-ceo-office 02-learning 03-knowledge 04-career 05-engineering 06-behavior-lab 07-operations 08-shared-memory 09-agent-factory 10-harness inbox workspace logs docs docs/superpowers/specs docs/superpowers/plans
```

Expected: directories exist.

### Task 2: Create Governance Documents

**Files:**
- Create `00-governance/company-charter.md`
- Create `00-governance/permission-boundaries.md`
- Create `00-governance/operating-principles.md`
- Create `00-governance/approval-rules.md`
- Create `00-governance/safety-reviewer-agent.md`

- [x] **Step 1: Write governance docs**

Expected: governance documents define company purpose, permissions, behavior principles, approval rules, and Safety Reviewer responsibilities.

### Task 3: Create Department and Agent Documents

**Files:**
- Create department `README.md` files
- Create agent job descriptions for Chief of Staff, Archivist, Learning Coach, Career Strategist, Profile Analyst, Builder, and Safety Reviewer

- [x] **Step 1: Write department and agent docs**

Expected: every first-version department has a clear responsibility and its core agent has a job description.

### Task 4: Create Memory and Workflow Documents

**Files:**
- Create `08-shared-memory/profile.md`
- Create `08-shared-memory/current-context.md`
- Create `08-shared-memory/memory-rules.md`
- Create `01-ceo-office/intake-workflow.md`
- Create `03-knowledge/inbox-processing.md`

- [x] **Step 1: Write memory and workflow docs**

Expected: new information can be routed from inbox to departments, knowledge, shared memory, and logs.

### Task 5: Create Roadmap and Logs

**Files:**
- Create `docs/roadmap.md`
- Create `docs/mvp-phase-1-plan.md`
- Create `docs/detailed-directory-tree.md`
- Create `logs/decision-log.md`
- Create `logs/change-log.md`
- Create `logs/run-log.md`

- [x] **Step 1: Write roadmap and logs**

Expected: SecondMe has a visible roadmap, MVP plan, directory map, and initial audit records.

