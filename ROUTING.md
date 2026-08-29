# Project Alpha OS v3 — Routing Policy

## Purpose

This file defines WHEN Project Alpha OS routes work.

AGENT_REGISTRY.md defines WHO each specialist is.

DELEGATION_POLICY.md defines HOW work is handed off.

Cursor owns the final routing decision.

---

## Default Entry Point

All work enters through Cursor in Slack (primarily `#all-alpha-command`).

---

## Routing Priority (in order)

1. Explicit repository, environment, or branch stated in the message
2. Channel default repository
3. Recent activity in the conversation
4. Named Environment defaults
5. Global default (`project-alpha-os` or the Project Alpha Environment)

---

## Multi-Repository Support

Prefer using named **Environments** that group:

- project-alpha-os (or project-alpha-core) — the brain
- Active project repositories
- Shared internal tools if needed

Example intent:

`@Cursor env="Project Alpha" fix the issue in client-x`

---

## Cloud Agents & Parallel Work

Cursor may launch Cloud Agents, background agents, or parallel agents for:

- Large implementations
- Independent subtasks
- Research (via Scout if enabled)
- Validation and testing

Cursor remains responsible for the overall result and final completion state.

---

## Workspace Safety

- Never assume the current directory is correct.
- Always confirm against PROJECT_REGISTRY.md and routing rules.
- If the workspace is wrong or ambiguous → stop and report BLOCKED or NEEDS REVIEW.

---

# 1. Core Routing Principle

Use the smallest capable execution path that can reliably complete the task.

Do not invoke a specialist merely because the task category exists.

A task category and an agent are different things.

Preferred execution paths:

Simple reasoning / operations
→ Cursor directly

Product requirements discussion
→ Cursor directly

Large software product planning
→ Cursor Planning Mode

Research / discovery
→ Scout, when enabled

Commercial intelligence
→ Cursor (dynamically, using available tools)

Software implementation
→ Cursor

Difficult technical reasoning
→ Cursor (dynamically)

---

# 2. Default Request Flow

Every meaningful request should conceptually pass through:

REQUEST
↓
CURSOR UNDERSTANDS INTENT
↓
CLASSIFY TASK
↓
LOAD RELEVANT CONTEXT
↓
SELECT EXECUTION PATH
↓
DELEGATE IF NEEDED
↓
EXECUTE
↓
VALIDATE
↓
CURSOR REVIEWS
↓
REPORT
↓
PERSIST IMPORTANT STATE

Not every small task requires every stage.

Substantial work does.

---

# 3. Cursor Direct Execution

Use Cursor directly for:

- general reasoning
- conversations
- summaries
- transformations
- lightweight analysis
- task decomposition
- operational planning
- organizing information
- creating specialist briefs
- requirement interviews
- clarifying product ideas
- simple technical reasoning
- routine company operations
- interpreting specialist output
- maintaining Project Alpha state
- commercial intelligence (using available tools)
- difficult technical reasoning (using available tools)
- software implementation

---

# 4. New Product Planning Trigger

When Adham says or clearly implies something such as:

- "I want to build a product"
- "I have a new project"
- "Let's plan a platform"
- "I have a client project"
- "I want to build an app"
- "I want to build a CRM"
- "I want to build a website"
- "Let's architect this"
- "Let's plan the system"

Cursor should enter PRODUCT PLANNING FLOW.

Do not immediately begin implementation.

---

# 5. Product Planning Flow

For substantial software products:

ADHAM
↓
CURSOR
↓
REQUIREMENTS DISCOVERY
↓
CURSOR PLANNING MODE
↓
TECHNICAL BLUEPRINT
↓
ADHAM APPROVAL WHEN NEEDED
↓
CURSOR IMPLEMENTATION

---

# 6. Cursor's Role During Product Planning

Before entering Planning Mode, Cursor should clarify the product enough for meaningful technical planning.

Gather relevant information such as:

- product purpose
- target users
- user roles
- core workflows
- business rules
- required features
- required integrations
- languages
- mobile requirements
- admin requirements
- authentication requirements
- payments if applicable
- notifications if applicable
- data requirements
- security requirements
- deployment expectations
- existing domain / infrastructure
- expected scale
- project constraints
- prototype vs production scope
- client-specific requirements
- known budget constraints when relevant

Do not ask unnecessary questions merely to fill a template.

Ask only questions that materially affect architecture, scope, cost, risk, or implementation.

---

# 7. Cursor Planning Mode

For large or serious software projects, Cursor Planning Mode is the DEFAULT technical planner.

Cursor Planning Mode owns technical planning such as:

- architecture
- project structure
- frontend architecture
- backend architecture
- database architecture
- data models
- API structure
- authentication design
- authorization model
- state management
- dependency selection
- framework decisions
- component boundaries
- service boundaries
- integrations
- technical risks
- implementation milestones
- testing strategy
- validation strategy
- deployment architecture
- relevant Cursor skills
- implementation order

---

# 8. Small Project Exception

Cursor Planning Mode is not mandatory for trivial implementation work.

Examples:

- small bug fix
- text change
- simple component
- isolated style adjustment
- basic script
- tiny automation
- obvious configuration change

For these:

CURSOR
↓
IMPLEMENT
↓
VALIDATE
↓
REPORT

---

# 9. Existing Project Planning

When planning substantial changes to an existing project:

Cursor must identify the correct workspace first.

Then:

CURSOR
↓
LOAD PROJECT STATE
↓
CURSOR PLANNING MODE INSPECTS EXISTING CODEBASE
↓
TECHNICAL CHANGE PLAN
↓
IMPLEMENTATION

Cursor Planning Mode should reason from the actual existing architecture rather than designing a replacement architecture from assumptions.

---

# 10. Cursor — Primary Builder

Cursor is the primary implementation specialist.

Route to Cursor for:

- websites
- web applications
- SaaS products
- dashboards
- CRM systems
- admin systems
- automation tools
- APIs
- frontend engineering
- backend engineering
- databases
- integrations
- authentication
- payment integrations
- refactoring
- migrations
- bug fixes
- testing
- performance work
- responsive implementation
- accessibility implementation
- SEO implementation
- animation implementation
- deployment preparation

Default software flow:

CURSOR
↓
IMPLEMENT
↓
SELF-VALIDATION
↓
EVIDENCE REVIEW
↓
REPORT

---

# 11. Cursor Workspace Rule

Never begin project modification until the intended workspace is known.

Cursor must never guess a project path.

For substantial work, execute inside the verified project directory.

No unrelated project may be modified.

---

# 12. Cursor Skill Routing

Before substantial implementation or planning, determine which skills are relevant.

Do not activate every skill indiscriminately.

Select by task.

Skills improve specialist execution.

They do not replace project requirements or validation.

---

# 13. Scout Routing

Route to Scout when the task primarily requires external discovery or evidence and Scout is enabled.

Examples:

- GitHub repository research
- finding current tools
- finding current libraries
- technology comparisons
- competitor research
- documentation research
- current pricing research
- API capability research
- SaaS comparisons
- hosting research
- security solution research
- market research
- implementation-option research
- discovering current best practices
- verifying current technical information

Scout should normally research before Cursor builds when implementation depends on uncertain external information.

---

# 14. Research-Then-Build Flow

When implementation depends on current or uncertain information:

CURSOR
↓
SCOUT (if enabled)
↓
RESEARCH FINDINGS
↓
CURSOR SYNTHESIZES
↓
CURSOR PLANNING MODE IF SUBSTANTIAL
↓
CURSOR IMPLEMENTS
↓
VALIDATION

---

# 15. Scout vs Cursor Research

Use Scout when the main task is discovering what exists or determining current facts.

Use Cursor when the main task is understanding and modifying the actual codebase.

Example:

"Which current GSAP skill repositories are best?"
→ Scout

"Why does this project's GSAP ScrollTrigger implementation break on mobile?"
→ Cursor

If Cursor requires current external documentation, Cursor may inspect documentation when the task is tightly connected to implementation.

---

# 16. Commercial Intelligence

Commercial intelligence is handled dynamically by Cursor using available tools.

Do not fabricate missing commercial numbers.

Unknown numbers must remain unknown unless they are explicitly estimated and clearly labeled.

---

# 17. Commercial-to-Product Flow

When Cursor identifies a software/product opportunity from commercial analysis:

CURSOR
↓
COMMERCIAL FINDING
↓
SYNTHESIZE OPPORTUNITY
↓
CURSOR PLANNING MODE IF SUBSTANTIAL
↓
CURSOR IMPLEMENTS
↓
VALIDATION

---

# 18. Difficult Technical Reasoning

Difficult technical reasoning is handled dynamically by Cursor using available tools.

This includes:

- difficult architecture decisions
- complex debugging
- deep code analysis
- hard algorithmic reasoning
- difficult implementation strategy
- independent technical review
- resolving technically ambiguous problems

Cursor may:

- reason through the problem directly
- consult documentation
- run experiments
- escalate to Adham if the decision exceeds scope

---

# 19. Historical Note

Previous versions of Project Alpha OS routed work through Hermes / Abel on Telegram, with Meter, Longcat, and Codex as dedicated agents. Those paths are deprecated. All work now enters through Cursor in Slack.
