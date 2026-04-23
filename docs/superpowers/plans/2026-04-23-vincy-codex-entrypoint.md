# Vincy Codex Entrypoint Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Let Vince invoke SecondMe inside Codex by calling `Vincy`.

**Architecture:** Add a repository-level Codex instruction file, a CEO office entrypoint for Vincy, and a harness adapter that defines Codex's execution boundary. Keep this as documentation-driven behavior with no custom runtime yet.

**Tech Stack:** Markdown, Codex repository instructions, git.

---

### Task 1: Add Repository-Level Codex Instructions

**Files:**
- Create: `AGENTS.md`

- [x] **Step 1: Create `AGENTS.md`**

Write activation rules for `Vincy`, required context files, operating style, department routing, and the boundary between Codex and SecondMe.

Expected: Codex has a clear repository-level instruction for how to behave when Vince invokes Vincy.

### Task 2: Add Vincy CEO Office Entrypoint

**Files:**
- Create: `01-ceo-office/vincy-entrypoint.md`

- [x] **Step 1: Create Vincy entrypoint**

Write Vincy's identity, default workflow, examples, reading order, output preference, and permission reminders.

Expected: SecondMe has a human-readable entrypoint for Codex sessions.

### Task 3: Add Codex Harness Adapter

**Files:**
- Create: `10-harness/codex-adapter.md`

- [x] **Step 1: Create Codex adapter**

Write Codex's role as an execution partner, activation method, permission boundary, recommended workflow, and failure handling.

Expected: Harness has a documented boundary for Codex use.

### Task 4: Update Project README

**Files:**
- Modify: `README.md`

- [x] **Step 1: Add Codex usage section**

Document how to call `Vincy`, provide examples, and link to the entry files.

Expected: Vince can open the README and immediately know how to use SecondMe inside Codex.

