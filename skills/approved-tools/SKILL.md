---
name: approved-tools
description: "Use after a build has been scoped (e.g. once the kickoff/brainstorm has produced a design or spec) and when writing or finalizing the implementation plan, in plan mode, or before writing any code at Calo. Recommends Calo's approved tools for the build and writes them — plus Calo's GitHub rules — into the plan, so the plan approved before coding uses signed-off tools in a compliant repo. Also use whenever an AI agent or teammate proposes a tool mid-build."
---

# Calo Approved Tools — bake the right stack into the plan

Calo's background standards layer. It does **not** run the brainstorm — it runs once the build is scoped, at planning time, to make sure the plan the team approves (before any code is written) uses Calo-approved tools and follows Calo's GitHub rules.

**Read the reference files fresh each time — never recommend tools or quote rules from memory.**

## When to use

- Right after the idea is scoped (kickoff/brainstorm done), as the implementation plan is being written.
- In plan mode, before the plan is approved.
- Any time an AI agent (or a teammate) proposes a tool while building.

## What to do

### 1. Recommend the approved tools

Read [`references/approved-tools.md`](references/approved-tools.md). Work out which technical dimensions the build touches — language, frontend, hosting, database, AI model, automation, messaging/API, data tooling, monitoring — and recommend the specific **approved** tool for each, with a one-line "why". Prefer the smallest set that does the job; Calo deliberately keeps the list short.

Present a short **Recommended Approved Tools** table:

| Need | Recommended (approved) tool | Why |
|------|------------------------------|-----|
| … | … | … |

**Access and off-list tools.** Only recommend tools that appear in the register. If the build needs a capability the register doesn't cover — *including any tool an AI agent proposes while building* — do not silently adopt it. State:

> ⚠️ **`<tool/capability>` is not on Calo's approved list.** Don't sign up for it yourself. Speak to **Bohdan or Caspar**, who will set up an admin-managed company account and invite you. The same applies to any approved tool you don't yet have access to.

### 2. State the GitHub rules

Read [`references/github-rules.md`](references/github-rules.md) and note the rules that apply to this build: the repo must be **connected to the Calo org** (contact **Bohdan** first if it isn't); default branch **`master`**; **no direct pushes** — branch + PR with **2 approvals**; **signed commits only**; files **under 10MB**; **Internal** visibility by default (Public only for genuine open-source); and use the internal building blocks **`install`**, **`goui`**, **`actions`**, **`copilot`**.

### 3. Write it into the plan

Add an **"Approved tools & build standards"** section to the implementation plan, containing the table from step 1 and the applicable GitHub rules from step 2. This must be part of the plan that is reviewed **before coding starts**, so the build proceeds on signed-off tools, in a Calo-connected, compliant repo.
