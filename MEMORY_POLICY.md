# Project Alpha OS v3 — Memory Policy

## Purpose

This file defines how Project Alpha OS stores, retrieves, updates, and removes persistent memory.

Memory exists to preserve useful continuity across sessions.

Memory must improve decisions.

Memory must not become a dump of conversation history.

---

# 1. Core Memory Principle

Conversation is temporary.

Memory is persistent.

Project files are implementation truth.

OS files are operating truth.

Memory should contain durable context that helps Cursor operate better across sessions.

Do not store information simply because it appeared in conversation.

Store it only if it is likely to matter again.

---

# 2. Memory Ownership

Cursor owns persistent memory management.

Other specialists may recommend something be remembered, but they do not directly redefine global memory policy.

Scout may produce information that later becomes memory only after Cursor determines it is durable and useful.

---

# 3. Memory Locations

Primary memory directory:

~/project-alpha-os/memories/

Canonical global memory files:

## USER.md

Stores durable information about Adham's working preferences, communication preferences, approval habits, and operating expectations.

## MEMORY.md

Stores durable Project Alpha knowledge that is useful across multiple projects and sessions.

Additional project-specific memory should normally live with the project rather than inside global memory.

---

# 4. Global Memory vs Project Memory

Use GLOBAL MEMORY for information that is useful across many projects.

Examples:

- Adham prefers Slack as the primary interface
- Cursor is the primary builder
- preferred working patterns
- reusable Project Alpha standards
- recurring technical preferences
- durable company operating facts

Use PROJECT MEMORY for information that belongs primarily to one project.

Examples:

- project architecture
- client-specific requirements
- database schema decisions
- project milestones
- deployment configuration
- project-specific design direction
- unresolved project blockers

Do not flood global memory with project-specific implementation details.

---

# 5. What Belongs in USER.md

USER.md should contain durable user-specific operating preferences.

Examples:

- preferred communication style
- preferred level of detail
- preferred workflow
- approval preferences
- preferred tools
- preferred development approach
- recurring technical preferences
- recurring business preferences

Only store something when it is likely to remain useful.

---

# 6. What Does NOT Belong in USER.md

Do not store:

- casual conversation
- jokes
- temporary emotions
- one-time requests
- temporary debugging details
- speculative assumptions
- sensitive personal information
- passwords or credentials
- temporary project requirements

A one-time instruction does not automatically become a permanent preference.

---

# 7. What Belongs in MEMORY.md

MEMORY.md stores durable Project Alpha operational knowledge.

Examples:

- stable company standards
- recurring development principles
- validated workflow improvements
- persistent specialist behavior
- reusable architecture preferences
- durable lessons learned across projects
- confirmed tool capabilities that materially affect workflow

Do not duplicate policy already defined in canonical OS files.

---

# 8. Policy vs Memory

This distinction is mandatory.

## OS Policy

Defines what the system MUST do.

Examples:

- Cursor is the primary orchestrator and builder
- production deployment requires approval
- project workspace must be verified

These belong in OS policy files.

## Memory

Stores useful facts and learned context.

Examples:

- Adham generally prefers concise operational answers
- a recurring project pattern has proven successful
- a certain deployment environment is commonly used

Do not use memory as a substitute for operating policy.

---

# 9. Source-of-Truth Hierarchy
When memory conflicts with verified reality, verified reality wins.

Preferred truth order:

1. directly verified current state
2. actual project files / runtime evidence
3. current OS policy
4. project documentation
5. current persistent memory
6. old conversation assumptions

Memory is never authoritative enough to override current evidence.

---

# 10. Memory Admission Test

Before writing something to persistent memory, Cursor should ask:

## A. Is it durable?

Will this likely matter in future sessions?

## B. Is it useful?

Will remembering it improve future decisions or reduce repeated work?

## C. Is it sufficiently verified?

Is this known rather than guessed?

## D. Is global memory the correct place?

Would project documentation be better?

## E. Is it already stored elsewhere?

Avoid duplication.

If the answer is weak, do not persist it.

---

# 11. Memory Confidence

Persistent facts should be treated according to confidence.

Recommended categories:

## CONFIRMED

Explicitly stated by Adham or directly verified.

## OBSERVED

Derived from repeated verified behavior or system state.

## TENTATIVE

Potentially useful but not fully confirmed.

Tentative information should rarely be stored globally.

Do not convert an inference into a confirmed memory.

---

# 12. User Corrections

If Adham corrects a stored fact:

1. accept the correction
2. update the canonical memory
3. remove or replace the stale fact
4. do not preserve contradictory versions
5. use the corrected information immediately

Newest verified correction wins.

---

# 13. Memory Contradictions

If two memory entries conflict:

DO NOT silently choose one.

Instead:

1. inspect current evidence
2. identify the newest verified fact
3. ask Adham if necessary
4. remove stale information
5. preserve one canonical truth

Memory should become cleaner over time, not more contradictory.

---

# 14. Repeated Information

Do not create duplicate entries for the same fact.

BAD:

- Adham prefers Cursor
- Cursor is Adham's preferred coding tool
- Adham likes Cursor for development
- Cursor should be used for code

GOOD:

- Cursor is the primary software builder for Project Alpha.

Where that fact is policy, store it in the OS rather than memory.

---

# 15. Memory Compression

Memory should remain compact enough to be useful.

Periodically:

- merge duplicate facts
- remove obsolete information
- shorten verbose entries
- move project-specific facts into projects
- remove temporary context
- keep only durable conclusions

Do not compress away important distinctions.

---

# 16. Memory Expiration

Some memories naturally become stale.

Examples:

- pricing
- software versions
- current subscriptions
- project status
- provider limits
- current infrastructure
- temporary team structure

For time-sensitive information, store the date or mark it as requiring re-verification.

Example:

Cursor CLI version verified:
2026-08-25

Do not assume time-sensitive memories remain current forever.

---

# 17. Last Verified Metadata

For facts likely to change, include:

Last verified:

YYYY-MM-DD

Examples:

- service subscription
- CLI version
- hosting environment
- model availability
- project status
- integration status

Static preferences usually do not require verification dates.

---

# 18. Specialist Output and Memory

Specialist output does not automatically become memory.

## Scout

Research findings may become memory only when they represent durable reusable knowledge.

Current pricing, repository popularity, or changing product availability should normally be re-researched later.

## Cursor

Implementation details normally belong in the project.

Technical reasoning may become reusable memory only if it produces a durable cross-project lesson.

Summaries or interpretations are not automatically memory.

---

# 19. Project Completion Memory

When a project milestone is completed, global memory should not copy the entire project state.
Instead preserve only durable cross-project lessons if useful.

Example:

GOOD:

"Project Alpha websites should visually validate RTL layouts at mobile breakpoints."

BAD:

Copying every file, bug, task, and milestone from one website into global memory.

---

# 20. Preferences vs Temporary Instructions

Distinguish between:

## Durable Preference

"Keep operational responses concise."

Potential memory.

## Temporary Request

"For this report, make it very detailed."

Not global memory.

Do not turn one-off instructions into permanent behavior.

---

# 21. Secrets and Sensitive Information

NEVER persist:

- passwords
- API keys
- authentication tokens
- OAuth secrets
- SSH private keys
- session cookies
- payment credentials
- recovery codes
- database passwords
- private certificates

Allowed:

"OPENAI_API_KEY is configured in the environment."

Not allowed:

The actual key value.

---

# 22. Credentials Mentioned in Conversation

If Adham accidentally exposes a credential:

- do not copy it into memory
- do not repeat it unnecessarily
- recommend rotation when appropriate
- reference only the credential name or storage location later

---

# 23. Project Paths

Verified workspace paths may be persisted in:

PROJECT_REGISTRY.md

Do not duplicate every project path inside global memory.

PROJECT_REGISTRY.md is the canonical source for workspace resolution.

---

# 24. Agent Roles

Permanent agent responsibilities belong in:

AGENT_REGISTRY.md

Routing rules belong in:

ROUTING.md

Do not duplicate these rules inside MEMORY.md.

Memory may contain learned behavior about agents only when it is not already canonical policy.

---

# 25. Skills

Installed skill inventory and skill policy should not be duplicated extensively in memory.

Skill inventory belongs in current state or skill policy.

Memory may preserve durable conclusions such as:

"Premium web projects benefit from combining design, motion, engineering, QA, accessibility, and SEO skills."

But the exact installed skill list should live outside memory.

---

# 26. Session Startup

On a fresh session or after major context loss:

1. load BOOTSTRAP.md
2. load required OS files
3. load USER.md
4. load MEMORY.md
5. load project-specific context only when a project is selected

Do not load every project into context at startup.

---

# 27. Context Efficiency

Persistent memory exists to reduce context waste.

Prefer:

small canonical facts

over:

large historical transcripts

Prefer:

current durable conclusions

over:

the full story of how the conclusion was reached

---

# 28. Memory Write Timing

Do not write memory after every message.

Write memory when:

- Adham establishes a durable preference
- a persistent operating fact changes
- a reusable lesson is confirmed
- important durable context would otherwise be lost
- Adham explicitly asks to remember something

Batch related updates when practical.

---

# 29. Explicit Remember Requests

When Adham explicitly says:

- remember this
- save this
- keep this
- don't forget this
- make this permanent

Cursor should determine the correct persistent location.

Possible destinations:

USER.md
MEMORY.md
PROJECT_REGISTRY.md
CURRENT_STATE.md
project documentation
OS policy

"Remember" does not always mean MEMORY.md.

Store it where it belongs.

---

# 30. Explicit Forget Requests

If Adham asks the system to forget or remove a persistent fact:

1. locate the canonical entry
2. remove it
3. remove conflicting duplicates
4. do not continue relying on the removed fact
5. report what was removed when useful

Do not keep hidden duplicate copies.

---

# 31. Historical Information

Historical information may remain when it is genuinely useful.

Label historical facts clearly.

Example:

Previous deployment provider:
X

Current deployment provider:
Y

Do not allow historical information to appear current.

---

# 32. Memory Review

Periodically review memory for:

- duplication
- contradiction
- stale facts
- project leakage
- excessive verbosity
- policy duplication
- sensitive data
- outdated assumptions
Memory quality matters more than memory size.

---

# 33. USER.md Structure

Recommended structure:

# User Memory

## Working Style

## Communication Preferences

## Development Preferences

## Business / Approval Preferences

## Durable Tool Preferences

## Other Confirmed Preferences

Keep sections concise.

---

# 34. MEMORY.md Structure

Recommended structure:

# Project Alpha Persistent Memory

## Company Standards

## Engineering Lessons

## Product / Design Lessons

## Operations

## Reusable Workflow Knowledge

## Other Durable Knowledge

Do not create empty categories merely for appearance.

---

# 35. Memory Change Reporting

Routine memory updates do not require verbose reporting.

For important changes, Cursor may report:

- what was remembered
- where it was stored
- what stale information was replaced

Do not expose the entire memory file unless requested.

---

# 36. Memory Integrity Rule

Persistent memory should contain the smallest amount of information required to preserve useful continuity.

It should be:

- accurate
- current
- concise
- non-duplicative
- appropriately scoped
- safe
- easy to update

---

# 37. Core Memory Rule

Remember what will matter again.

Keep policy out of memory.

Keep project detail with the project.

Keep secrets out entirely.

When reality changes, update memory rather than defending the past.
