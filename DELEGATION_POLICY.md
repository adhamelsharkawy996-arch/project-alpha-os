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

Hermes / Abel

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

Hermes / Abel (dynamically)

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

Hermes / Abel (dynamically)

Requires:

- isolated hard problem
- evidence
- previous attempts
- actual failure
- relevant architecture
- expected reasoning output

Hermes / Abel handles this directly using available tools.

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

