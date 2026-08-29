# Project Alpha OS v3 — Current State

**Version**: v3  
**Last Updated**: 2026-08-29  
**Status**: Transition complete

## Purpose

This file records the CURRENT operational state of Project Alpha OS.

It should answer:

- what is active
- what is installed
- what is connected
- what is verified
- what is pending
- what is blocked

This file is operational state, not permanent policy.

Permanent rules belong in the appropriate OS policy files.

Update this file whenever the real system state materially changes.

---

## Current Primary Agent

Cursor (Orchestrator + Builder)

Cursor is the single live entry point. It owns routing, planning, implementation, self-validation, completion status, and final reporting.

---

## Interface

Slack (`#all-alpha-command` and related channels)

Canonical chain:

Adham → Slack → Cursor → Project Alpha OS → Code / Tools / Deploy

---

## Source of Truth

Private GitHub repositories:

- `project-alpha-os` — operating system, routing, memory, skills catalog
- `project-alpha-core` — companion core repo when present
- project repos — implementation truth for each product

Conversation provides current context.  
OS files provide operating truth.  
Project files provide implementation truth.  
Verification provides completion truth.

---

## Live Components

- OS files: Active
- Skills catalog: Active
- Memory systems: Active
- Cursor Cloud Agents: Primary execution path

---

## Deprecated

- Hermes / Abel orchestration path
- Telegram as primary interface
- Old agent roster (Meter, Longcat, Codex)

These are historical. They must not be treated as live routing, intake, or authority.

---

## Next Focus

Real multi-repo tasks executed entirely under Cursor orchestration with full OS compliance.

---

# 1. OS Version

System:

Project Alpha OS v3

Status:

TRANSITION COMPLETE

Current phase:

Cursor-orchestrated multi-repo execution

---

# 2. Cursor

Status:

ACTIVE

Role:

Primary orchestrator and software builder

Execution path:

Cursor Cloud Agents (primary)

Interface:

Slack

Reports to:

Adham

Authority:

Full within OS hard limits

Hard limits:

- no production deploy without Adham's explicit approval
- no secrets in memory, reports, or git
- no OS architecture changes without explicit instruction
- never guess a workspace

---

# 3. Scout

Status:

DEFINED / OPTIONAL

Role:

Deep research specialist

Called by:

Cursor only

Does:

Research, synthesis, source gathering

Does not:

Write production code, own routing, or make architecture decisions

Operational routing:

Available when enabled. Not required for every task.

---

# 4. OS Files

Current OS root:

`project-alpha-os` (this repository)

Cloud workspace for this session:

`/workspace`

Canonical files:

- BOOTSTRAP.md
- OPERATING_SYSTEM.md
- AGENT_REGISTRY.md
- ROUTING.md
- CURRENT_STATE.md
- PROJECT_REGISTRY.md
- MEMORY_POLICY.md
- DELEGATION_POLICY.md
- SKILL_POLICY.md

Directories:

- memories/
- skills/
- agents/
- knowledge/

---

# 5. Skills Catalog

Status:

ACTIVE

Catalog location:

`skills/` in this repository, plus Cursor global / plugin skills when present

Repo-owned skill currently present:

- deep-research (Scout)

Skill-first rule remains in force:

use the smallest capable skill set that materially improves the task.

Full curated skill stress test:

PENDING — should happen against real multi-repo work, not file discovery alone.

---

# 6. Memory Systems

Status:

ACTIVE

Locations:

- memories/USER.md
- memories/MEMORY.md
- MEMORY_POLICY.md

Memory is for durable continuity.

It is not conversation history and not a substitute for OS policy.

---

# 7. Project Registry

Status:

ACTIVE / PARTIALLY POPULATED

Registered:

- project-alpha-os — VERIFIED
- cursor-test — previously registered as a local safe test workspace

Production / client projects:

NOT YET VERIFIED under OS v3

Active production project:

NONE

Do not modify a client or production workspace until it is resolved in PROJECT_REGISTRY.md.

---

# 8. Multi-Repo / Environments

Preferred model:

Named Cursor Environments that group:

- project-alpha-os (or project-alpha-core) — the brain
- active project repositories
- shared internal tools if needed

Example intent:

`@Cursor env="Project Alpha" fix the issue in client-x`

Current named Environment status:

NOT YET CONFIRMED as a saved `Project Alpha` Environment from this session.

Until a named Environment is saved, routing falls back to:

1. explicit repository / environment / branch in the message
2. channel default repository
3. recent conversation activity
4. named Environment defaults
5. global default (`project-alpha-os` or the Project Alpha Environment)

---

# 9. Verified Execution Architecture

Current live path:

Adham
↓
Slack
↓
Cursor (Cloud Agent)
↓
Project Alpha OS
↓
code / tools / optional Scout / parallel agents
↓
evidence
↓
completion state
↓
Slack report

Status:

LIVE

Cursor remains responsible for the overall result even when Cloud Agents, background agents, or Scout run in parallel.

---

# 10. Product Planning Architecture

Current intended planning flow:

Adham
↓
Cursor (Slack)
↓
requirements discovery
↓
technical plan when the work is substantial
↓
Adham approval where needed
↓
Cursor implementation (milestones)
↓
evidence
↓
completion state

Status:

POLICY DEFINED

---

# 11. Project Safety State

Existing project directories must remain untouched unless explicitly selected for work.

Never assume the current directory is correct.

Always confirm against PROJECT_REGISTRY.md and ROUTING.md.

If the workspace is wrong or ambiguous:

stop and report BLOCKED or NEEDS REVIEW.

---

# 12. Completed Transition Work

Completed:

- Cursor established as primary orchestrator and builder
- Slack established as the primary interface
- GitHub established as the source of truth
- Hermes / Abel removed from the live orchestration path
- Telegram removed as the primary interface
- Meter, Longcat, and Codex removed from the live roster
- OS files, skills catalog, and memory systems marked live
- Cursor Cloud Agents marked as the primary execution path
- Core OS policy files realigned to v3 (Cursor / Slack)

---

# 13. Pending Work

Current priority order:

1. execute real multi-repo tasks entirely under Cursor orchestration
2. verify and register production / client workspaces
3. confirm or create the named Project Alpha Environment
4. stress-test skill selection and evidence-based completion on real work
5. keep Scout optional and Cursor-called only

---

# 14. Not Yet Verified

The following are NOT yet considered fully verified:

- named `Project Alpha` Environment saved and reusable
- production / client workspace registry
- automatic skill selection under real load
- full multi-repo Cloud Agent workflows
- end-to-end large project planning and implementation under v3
- Scout as an operational parallel specialist

Do not claim these are working until tested.

---

# 15. Current Blockers

No critical blocker currently known.

The v2 Hermes / Telegram path is deprecated and must not be used as a live dependency.

---

# 16. State Update Rule

When material system state changes:

UPDATE THIS FILE.

Examples:

- specialist becomes operational
- interface or source of truth changes
- integration is verified
- new global capability is installed
- a blocker appears
- a blocker is resolved
- system architecture changes
- stress test passes or fails

Do not preserve obsolete state merely because it was previously true.

Verified current reality overrides this file.

---

# 17. Current System Verdict

Project Alpha OS v3:

TRANSITION COMPLETE

Primary agent:

CURSOR — ORCHESTRATOR + BUILDER

Primary interface:

SLACK

Source of truth:

PRIVATE GITHUB REPOSITORIES

Execution path:

CURSOR CLOUD AGENTS — LIVE

Deprecated path:

HERMES / ABEL / TELEGRAM — DO NOT USE

Next focus:

REAL MULTI-REPO TASKS UNDER CURSOR, WITH FULL OS COMPLIANCE
