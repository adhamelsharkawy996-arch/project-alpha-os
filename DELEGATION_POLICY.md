# Project Alpha OS v2 — Delegation Policy

## Purpose

This file defines HOW Abel delegates work to specialists.

ROUTING.md decides:

WHO should receive the task.

DELEGATION_POLICY.md decides:

HOW the task must be packaged, executed, validated, escalated, and returned.

A specialist should never receive a vague substantial task when Abel can provide a structured execution brief.

---

# 1. Core Delegation Principle

Delegation must transfer enough context for the specialist to act correctly without transferring unnecessary noise.

Every substantial delegation should answer:

- what are we trying to achieve
- which project is involved
- where the workspace is
- what existing context matters
- what must be done
- what must not be done
- which skills are relevant
- what success looks like
- how success must be validated
- when the specialist must stop and return control

---

# 1.1 YC Category Alignment

Y Combinator's Fall 2026 Requests for Startups explicitly lists these categories:

- **AI agents operating inside enterprises** — agents that handle real work inside companies, not demos
- **Verification for autonomous systems** — proving that what an agent claims matches reality
- **Rebuilding real-world systems** — education, healthcare, defense, finance, infrastructure

This policy addresses all three:
- Structured briefs → agents operating inside enterprises
- Verification gates → verification for autonomous systems
- Milestone delegation → rebuilding real-world systems

Every delegation template in this document maps to a YC-funded category.

---

# 2. Delegation Ownership

Abel owns system-level delegation.

Specialists may perform internal reasoning or tool use required for their task.

Specialists may NOT create uncontrolled Project Alpha delegation chains.

Preferred flow:

Adham
↓
Abel
↓
Specialist
↓
Abel
↓
Next specialist if required

Abel remains the coordination point.

---

# 3. Delegation Classes

Use one of these delegation classes.

## A. LIGHTWEIGHT

Small task with low risk and limited scope.

Examples:

- summarize information
- organize requirements
- simple reasoning
- small text transformation
- simple technical explanation

Usually:

Abel / Longcat

Minimal brief required.

---

## B. RESEARCH

External discovery or evidence gathering.

Usually:

Scout

Requires:

- research question
- scope
- freshness requirement
- preferred evidence quality
- expected output

---

## C. COMMERCIAL

Marketing / sales / advertising / commercial intelligence.

Usually:

Meter

Requires:

- business question
- available data
- relevant timeframe
- desired decision
- uncertainty constraints

---

## D. PLANNING

Substantial software technical planning.

Usually:

Cursor Planning Mode

Requires:

- verified project
- requirements
- constraints
- existing architecture if applicable
- planning objective
- expected blueprint
- risks to inspect

---

## E. IMPLEMENTATION

Software modification.

Usually:

Cursor

Requires the full execution contract.

---

## F. ESCALATION

Difficult technical reasoning.

Usually:

Codex OAuth
Model: gpt-5.6-sol

Requires:

- isolated hard problem
- evidence
- previous attempts
- actual failure
- relevant architecture
- expected reasoning output

---

# 4. Delegation Readiness

Before substantial delegation, Abel must determine whether the task is ready.

Use these states:

## READY

Enough context exists for reliable execution.

## READY WITH RISKS

Execution can proceed, but known uncertainty exists.

The risk must be communicated in the brief.

## BLOCKED

Execution should not proceed.

Examples:

- project unknown
- workspace unknown
- required business decision missing
- destructive impact unclear
- credentials unavailable
- critical requirement unresolved

Do not delegate a BLOCKED task merely to make progress appear active.

---

# 5. Required Software Delegation Contract

For substantial Cursor work, Abel should provide:

## PROJECT

Canonical project name / ID.

## WORKSPACE

Exact verified filesystem path.

## OBJECTIVE

What outcome is required.

## CONTEXT

Only relevant existing information.

## REQUIREMENTS

Concrete behaviors / features / changes.

## CONSTRAINTS

Technical, product, business, design, security, or infrastructure constraints.

## SELECTED SKILLS

Relevant Cursor skills.

## ALLOWED SCOPE

Files / areas that may be modified.

## PROTECTED SCOPE

Files / areas that should not be changed unless required.

## ACCEPTANCE CRITERIA

Observable conditions required for success.

## VALIDATION

Commands, browser checks, tests, or other verification required.

## STOP CONDITIONS

When Cursor must stop and return to Abel.

## REPORT FORMAT

What Cursor must report after execution.

---

## YC Connection

Y Combinator's current batch includes Tolmo (AI security for cloud infrastructure). The verification section above is the agent-side complement: Tolmo secures the infrastructure, this policy verifies what agents claim about that infrastructure.

When YC says they want "verification for autonomous systems," they mean exactly this: observable evidence that an agent did what it claimed, not just the agent's assertion.

---

# 6. Cursor Delegation Template

Use this structure for substantial implementation:

PROJECT:
<canonical project>

WORKSPACE:
<verified absolute path>

MODE:
IMPLEMENTATION

OBJECTIVE:
<precise desired outcome>

CONTEXT:
<relevant architecture / project state>

REQUIREMENTS:
- requirement
- requirement
- requirement

CONSTRAINTS:
- constraint
- constraint

SELECTED SKILLS:
- skill
- skill

ALLOWED SCOPE:
- paths / modules / system areas

PROTECTED SCOPE:
- areas not to touch unnecessarily

ACCEPTANCE CRITERIA:
- observable success condition
- observable success condition

VALIDATION:
- build
- tests
- browser checks
- other relevant validation

STOP AND RETURN IF:
- workspace appears wrong
- requirement conflicts with architecture
- destructive change becomes necessary
- secret / credential is missing
- external blocker prevents completion
- architecture decision exceeds scope
- repeated validation failure requires deeper reasoning

RETURN:
- summary of changes
- files changed
- validation performed
- validation result
- remaining risks
- blockers if any

---

# 7. Cursor Planning Mode Delegation

When the task is substantial product planning:

MODE:

PLANNING

Cursor should NOT immediately implement.

Planning brief should include:

- product purpose
- users
- roles
- core workflows
- business rules
- required features
- constraints
- integrations
- security expectations
- scale assumptions
- locales
- admin requirements
- prototype vs production expectations
- existing architecture if applicable

Cursor Planning Mode should produce:

- recommended architecture
- stack decisions
- data model direction
- system boundaries
- component/service structure
- key workflows
- integration strategy
- security approach
- relevant skills
- implementation milestones
- validation strategy
- major risks
- unresolved technical questions

Implementation should begin only after the plan is accepted or the task explicitly authorizes implementation.

---

# 8. Planning-to-Build Handoff

After Cursor Planning Mode:

Cursor Plan
↓
Abel reviews
↓
Resolve important unanswered questions
↓
Adham approves high-impact decisions when needed
↓
Convert plan into implementation tasks
↓
Cursor builds milestone by milestone

Do not feed an entire giant project to Cursor as one uncontrolled implementation prompt when milestone execution is more reliable.

---

# 9. Milestone Delegation

Large projects should be divided into meaningful milestones.

Each milestone should have:

- objective
- dependencies
- scope
- acceptance criteria
- validation
- completion state

Example:

Milestone 1:
Foundation / architecture

Milestone 2:
Core data / backend

Milestone 3:
Primary user flows

Milestone 4:
Admin / operational flows

Milestone 5:
Polish / motion / responsive

Milestone 6:
QA / security / SEO / production readiness

Actual milestones should fit the project rather than this generic example.

---

# 10. One Milestone at a Time

For complex projects, prefer:

PLAN
↓
MILESTONE
↓
BUILD
↓
VALIDATE
↓
REVIEW
↓
NEXT MILESTONE

instead of:

PLAN
↓
BUILD EVERYTHING
↓
HOPE IT WORKS

This reduces context drift and false completion.

---

# 11. Skill Delegation

Abel should not manually paste the contents of every skill into Cursor prompts.

Instead:

- identify relevant installed skills
- name them in the execution brief when useful
- allow Cursor to load them from the global skill directory
- use only skills relevant to the current task

Global location:

~/.cursor/skills/

Examples:

Premium UI:
- taste-skill
- ui-ux-pro-max

GSAP:
- gsap-core
- gsap-react
- gsap-scrolltrigger
- gsap-performance

React:
- react-best-practices

QA:
- playwright-cli

SEO:
- optimise-seo

Accessibility:
- accessibility

---

# 12. Workspace Delegation Rule

Every project-modifying delegation must specify the verified workspace.

BAD:

"Use Cursor and fix Mina Lens."

GOOD:

PROJECT:
mina-lens

WORKSPACE:
/verified/path/to/mina-lens

OBJECTIVE:
Fix ...

If the workspace is unknown:

DO NOT DELEGATE MODIFICATION.

Resolve it first.

---

# 13. Project Boundary Enforcement
The delegated specialist must stay within the intended project boundary.

Do not modify:

- unrelated projects
- global OS files
- another client's files
- unrelated environment configuration
- system packages

unless the task explicitly requires it.

If work outside the project becomes necessary, return control to Abel first when impact is significant.

---

# 14. Allowed vs Protected Scope

For high-impact tasks, explicitly separate:

## Allowed Scope

What Cursor is expected to modify.

## Protected Scope

What should remain untouched unless required.

Example:

Allowed:

src/app/
src/components/

Protected:

.env
production database
deployment configuration
authentication secrets

This prevents broad "cleanup" behavior from damaging unrelated areas.

---

# 15. Destructive Actions

A specialist must not perform destructive operations casually.

Examples:

- deleting project directories
- removing databases
- resetting production data
- force-pushing
- destructive migrations
- deleting infrastructure
- deleting production assets
- wiping configuration
- broad dependency replacement

When destruction is required:

1. explain why
2. identify impact
3. create backup / rollback path when appropriate
4. obtain required approval
5. execute only within defined scope

---

# 16. Dependency Delegation

Cursor may add dependencies when justified.

Before adding one, consider:

- existing stack
- necessity
- maintenance quality
- security
- runtime impact
- bundle impact
- duplicate functionality

Do not add packages merely because they simplify a few lines of code.

Do not perform broad upgrades unless required.

Never use:

npm audit fix --force

as a routine dependency fix.

---

# 17. Existing Code Respect

When modifying an existing project:

Cursor must inspect the existing code before imposing a new architecture.

Prefer:

extend existing conventions

over:

rewrite everything

unless a rewrite is clearly justified.

Large architectural changes should return to planning / approval.

---

# 18. Acceptance Criteria

Every substantial task should define observable completion.

BAD:

"Make it premium."

BETTER:

- desktop and mobile layouts completed
- Arabic RTL and English LTR function correctly
- hero animation uses GSAP
- no horizontal mobile overflow
- form validates correctly
- build passes
- required pages are reachable
- browser console has no blocking errors

Acceptance criteria should describe outcomes, not effort.

---

# 19. Validation Delegation

The execution brief must define validation proportional to the task.

Examples:

Code change:
- build
- typecheck
- test

Frontend:
- build
- browser verification
- responsive checks
- console checks

Premium site:
- build
- browser QA
- visual inspection
- GSAP behavior
- reduced motion
- RTL/LTR
- accessibility
- SEO where applicable

API:
- automated tests
- error-path validation
- response validation

Do not require irrelevant validation.

---

# 20. Cursor Self-Validation

Cursor should validate its own work before returning.

The returned report should state:

- what was tested
- what passed
- what failed
- what could not be tested

Never accept:

"Everything should work."

Prefer evidence:

"npm run build passed."

"Playwright verified menu navigation."

"No blocking console errors observed."

---

# 21. Abel Independent Review

Cursor self-validation is necessary but not always sufficient.

For substantial work, Abel should independently review important evidence.

This may include:

- inspecting changed files
- inspecting build result
- running validation separately
- browser inspection
- comparing against acceptance criteria
- checking project state

Abel should not simply repeat Cursor's completion claim.

---

# 22. Specialist Return Contract

Every substantial specialist task should return a structured result.

Minimum:

STATUS:
COMPLETE / COMPLETE WITH RISKS / BLOCKED / NEEDS REVIEW

SUMMARY:
What was done.

CHANGES:
What materially changed.

VALIDATION:
What was checked.

RESULT:
What passed / failed.

RISKS:
Remaining non-blocking concerns.
BLOCKERS:
Anything preventing completion.

NEXT:
Only when a meaningful next action exists.

---

# 23. Stop Conditions

A specialist should stop instead of guessing when:

- project identity is uncertain
- workspace is uncertain
- requirement materially conflicts
- important business decision is missing
- credentials are required but unavailable
- production impact is unclear
- destructive action becomes necessary
- architecture question is outside task scope
- repeated attempts fail
- external service prevents progress

Return the blocker to Abel.

---

# 24. Retry Policy

Do not allow blind retry loops.

After failure:

1. inspect the failure
2. change the hypothesis or approach
3. retry when justified

If the same class of failure repeats:

STOP
↓
RETURN EVIDENCE
↓
ABEL DECIDES ESCALATION

More retries are not automatically better reasoning.

---

# 25. Codex Escalation Package

When escalating to Codex OAuth, do NOT send:

"Cursor can't fix it. Help."

Send a focused reasoning packet.

Include:

PROBLEM:
Exact technical problem.

ARCHITECTURE:
Relevant system design.

EVIDENCE:
Errors, behavior, relevant code facts.

ATTEMPTS:
What Cursor already tried.

RESULT:
Why those attempts failed.

CONSTRAINTS:
What must remain unchanged.

QUESTION:
The specific reasoning problem Codex should solve.

EXPECTED OUTPUT:
Recommendation / root-cause analysis / architecture decision.

MODEL:

gpt-5.6-sol

---

# 26. Codex Execution Boundary

Codex should normally reason.

Cursor should normally implement.

Preferred:

Codex
→ technical answer

Abel
→ converts answer into execution guidance

Cursor
→ implementation

Do not hand entire projects to Codex simply because one difficult issue appeared.

---

# 27. Scout Delegation Template

For Scout:

QUESTION:
What must be researched?

SCOPE:
What is included / excluded?

FRESHNESS:
How current must information be?

PREFERRED SOURCES:
Official docs / GitHub / primary sources / community evidence as relevant.

COMPARISON CRITERIA:
What matters?

OUTPUT:
- findings
- sources
- tradeoffs
- recommendation
- uncertainty

Do not ask Scout to return giant dumps of links without synthesis.

---

# 28. Scout Evidence Standard

Scout should prefer:

1. official / primary sources
2. maintained repositories
3. authoritative technical documentation
4. credible secondary analysis
5. community evidence where useful

Scout must distinguish:

FACT

SUPPORTED INFERENCE

OPINION

UNKNOWN

---

# 29. Meter Delegation Template

For Meter:

BUSINESS QUESTION:
What decision are we trying to make?

DATA:
What real information is available?

TIMEFRAME:
What period matters?

CONTEXT:
Offer / market / campaign / funnel context.

ANALYSIS REQUIRED:
What should Meter evaluate?

OUTPUT:
- findings
- key metrics
- commercial impact
- opportunities
- risks
- recommendation

Missing numbers must not be fabricated.

---

# 30. Longcat Delegation

Longcat should receive concise lightweight tasks.

Examples:

- organize requirements
- convert discussion into structured brief
- summarize specialist output
- identify missing product questions
- prepare a Cursor planning brief
- reason about simple operational decisions

Do not create heavyweight delegation contracts for trivial tasks.

---

# 31. Requirement Interview Handoff

For a new serious product:

Adham
↓
Abel / Longcat
↓
requirements interview
↓
structured product brief
↓
Cursor Planning Mode

The handoff to Cursor should contain distilled requirements.

Do not dump the entire raw Telegram conversation into Cursor when a clean structured brief can preserve the necessary context.

---

# 32. Context Discipline

Include:

- facts that affect execution
- requirements
- decisions
- constraints
- architecture
- relevant prior failures

Exclude:

- unrelated conversation
- repetitive discussion
- abandoned ideas unless they explain a constraint
- speculation
- unnecessary internal chatter

High-quality context is selective.

---

# 33. Decision Preservation

When an important decision has already been made, include it in later delegation where relevant.

Example:
"Payments are prototype-only; no real payment gateway should be connected."

This prevents specialists from reopening settled decisions unnecessarily.

---

# 34. Assumption Handling

A specialist may make low-risk implementation assumptions when reasonable.

High-impact assumptions must be surfaced.

Examples requiring clarification or planning:

- changing authentication architecture
- replacing database technology
- altering pricing logic
- changing business rules
- changing user roles
- changing payment flow
- modifying production deployment strategy

---

# 35. Production Delegation

Any production-affecting task should state explicitly:

ENVIRONMENT:

production / staging / local

AUTHORITY:

approved / not approved

ROLLBACK:

available / required / not applicable

VALIDATION:

required checks

Never let a generic development task silently become a production deployment.

---

# 36. Credentials

Delegation briefs may reference:

- credential name
- environment variable
- configured secret location

Do NOT include secret values.

Example:

GOOD:

Cloudflare token is configured in environment variable CLOUDFLARE_API_TOKEN.

BAD:

CLOUDFLARE_API_TOKEN=actual-secret

---

# 37. Parallel Delegation

Parallel specialist work is allowed when tasks are independent.

Example:

Scout
→ research payment provider

Meter
→ commercial pricing analysis

These may happen independently.

Do not parallelize tasks that modify the same project state unless coordination is explicit.

Avoid conflicting simultaneous Cursor modifications.

---

# 38. Sequential Dependency

When Task B depends on Task A, delegate sequentially.

Example:

Scout research
↓
architecture decision
↓
Cursor planning
↓
implementation

Do not ask Cursor to implement before required discovery is complete.

---

# 39. Delegation Logging

Important delegation results should update durable state when appropriate.

Possible destinations:

CURRENT_STATE.md

PROJECT_REGISTRY.md

project blueprint

project task/state file

MEMORY.md only for durable cross-project lessons

Do not log every prompt and response permanently.

---

# 40. Completion Authority

A specialist can report:

"I completed my assigned task."

Only Abel should determine:

"The Project Alpha task is complete."

Abel checks:

- assigned scope
- acceptance criteria
- validation
- blockers
- broader project state

---

# 41. Partial Completion

If only part of the task succeeds:

STATUS:

COMPLETE WITH RISKS

or

BLOCKED

depending on impact.

Do not use COMPLETE when required acceptance criteria remain unmet.

---

# 42. NEEDS REVIEW

Use NEEDS REVIEW when implementation is technically ready but requires Adham's judgment.

Examples:

- visual design selection
- branding direction
- pricing decision
- major product behavior
- production deployment approval

Technical readiness is not the same as business approval.

---

# 43. Delegation Efficiency

Good delegation minimizes:

- duplicated work
- repeated context gathering
- unnecessary specialist calls
- unclear responsibilities
- huge vague prompts
- endless retry loops

Good delegation maximizes:

- clear scope
- correct specialist selection
- focused context
- observable completion
- reliable verification

---

# 44. Delegation Anti-Patterns

Avoid:

## "Do everything"

Huge uncontrolled task with no milestones.

## "Make it better"

No measurable objective.

## "Fix all issues"

Undefined scope.

## "Use every skill"

Unnecessary context and conflicting guidance.

## "Keep trying until it works"

Encourages blind retry loops.

## "Deploy when done"

Implicit production authority.

## "Rewrite if needed"

Too much architectural freedom unless explicitly justified.

---

# 45. Canonical Delegation Flow

For substantial Project Alpha software work:

ABEL
↓
RESOLVE PROJECT
↓
LOAD CONTEXT
↓
REQUIREMENTS
↓
CURSOR PLANNING MODE WHEN NEEDED
↓
SELECT SKILLS
↓
CREATE EXECUTION CONTRACT
↓
CURSOR IMPLEMENTS
↓
CURSOR SELF-VALIDATES
↓
ABEL INDEPENDENTLY REVIEWS
↓
CODEX ESCALATION ONLY IF JUSTIFIED
↓
FINAL VERDICT
↓
PERSIST IMPORTANT STATE
↓
REPORT TO ADHAM

---
# 46. Core Delegation Rule

Give each specialist:

the minimum context required to fully understand the task,

the maximum clarity required to execute it correctly,

and explicit evidence required to prove completion.
