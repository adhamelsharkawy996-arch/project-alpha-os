# Project Alpha OS v2 — Routing Policy

## Purpose

This file defines WHEN Project Alpha OS routes work to each specialist.

AGENT_REGISTRY.md defines WHO each specialist is.

DELEGATION_POLICY.md defines HOW work is handed to a specialist.

Hermes / Abel owns the final routing decision.

---

# 1. Core Routing Principle

Use the smallest capable execution path that can reliably complete the task.

Do not invoke a specialist merely because the task category exists.

A task category and an agent are different things.

For example:
- COMMERCIAL may remain a classification without requiring a Meter agent
- ESCALATION may remain an execution state without requiring a Codex agent
- lightweight reasoning does not require a Longcat role

Preferred execution paths:

Simple reasoning / operations
→ Hermes / Abel directly

Product requirements discussion
→ Hermes / Abel directly

Large software product planning
→ Cursor Planning Mode

Research / discovery
→ Scout

Commercial intelligence
→ Hermes / Abel (dynamically, using available tools)

Software implementation
→ Cursor

Difficult technical reasoning
→ Hermes / Abel (dynamically)

---

# 2. Default Request Flow

Every meaningful request should conceptually pass through:

REQUEST
↓
HERMES / ABEL UNDERSTANDS INTENT
↓
CLASSIFY TASK
↓
LOAD RELEVANT CONTEXT
↓
SELECT EXECUTION PATH
↓
DELEGATE
↓
EXECUTE
↓
VALIDATE
↓
HERMES / ABEL REVIEWS
↓
REPORT
↓
PERSIST IMPORTANT STATE

Not every small task requires every stage.

Substantial work does.

---

# 3. Hermes / Abel Direct Execution

Use Hermes / Abel directly for:

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

Hermes / Abel should enter PRODUCT PLANNING FLOW.

Do not immediately begin implementation.

---

# 5. Product Planning Flow

For substantial software products:

ADHAM
↓
HERMES / ABEL
↓
REQUIREMENTS DISCOVERY
↓
CURSOR PLANNING MODE
↓
TECHNICAL BLUEPRINT
↓
HERMES / ABEL REVIEW
↓
ADHAM APPROVAL WHEN NEEDED
↓
CURSOR IMPLEMENTATION

---

# 6. Hermes / Abel's Role During Product Planning

Before invoking Cursor Planning Mode, Hermes / Abel should clarify the product enough for meaningful technical planning.

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

Hermes / Abel should not independently produce the final technical architecture for a serious project when Cursor Planning Mode is available.

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

HERMES / ABEL
↓
CURSOR
↓
VALIDATION
↓
HERMES / ABEL REVIEW

---

# 9. Existing Project Planning

When planning substantial changes to an existing project:

Hermes / Abel must identify the correct workspace first.

Then:

HERMES / ABEL
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

HERMES / ABEL
↓
CURSOR
↓
CURSOR SELF-VALIDATION
↓
HERMES / ABEL INDEPENDENT REVIEW
↓
REPORT

---

# 11. Cursor Workspace Rule

Never invoke Cursor for project modification until the intended workspace is known.

Hermes / Abel must never guess a project path.

For substantial work, Cursor should execute inside the verified project directory.

No unrelated project may be modified.

---

# 12. Cursor Skill Routing

Cursor has globally installed specialist skills at:

~/.cursor/skills/

Before substantial implementation or planning, Hermes / Abel and/or Cursor should determine which skills are relevant.

Do not activate every skill indiscriminately.

Select by task.

Example premium Next.js website:

Design:
- taste-skill
- ui-ux-pro-max

Motion:
- gsap-core
- gsap-react
- gsap-timeline
- gsap-scrolltrigger
- gsap-plugins
- gsap-performance
- animate
- improve-animations
- review-animations

Engineering:
- react-best-practices

QA:
- playwright-cli

Accessibility:
- accessibility

SEO:
- optimise-seo

Skills improve specialist execution.

They do not replace project requirements or validation.

---

# 13. Scout Routing

Route to Scout when the task primarily requires external discovery or evidence.

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

HERMES / ABEL
↓
SCOUT
↓
RESEARCH FINDINGS
↓
HERMES / ABEL SYNTHESIZES
↓
CURSOR PLANNING MODE IF SUBSTANTIAL
↓
CURSOR IMPLEMENTS
↓
VALIDATION

Examples:

- unfamiliar payment provider
- new authentication provider
- current API limits
- current library capability
- new framework feature
- unknown hosting limitations
- third-party integrations
- external security products

---

# 15. Scout vs Cursor Research

Use Scout when the main task is discovering what exists or determining current facts.

Use Cursor when the main task is understanding and modifying the actual codebase.

Example:

"Which current GSAP skill repositories are best?"
→ Scout

"Why does this project's GSAP ScrollTrigger implementation break on mobile?"
→ Cursor

If Cursor requires current external documentation:

Scout may research first or Cursor may inspect documentation when the task is tightly connected to implementation.

Hermes / Abel decides based on efficiency.

---

# 16. Commercial Intelligence

Commercial intelligence is handled dynamically by Hermes / Abel using available tools.

Route commercial questions to Hermes / Abel for:

- advertising analysis
- campaign strategy
- sales intelligence
- pricing strategy
- competitor offer analysis
- conversion analysis
- funnel analysis
- customer acquisition
- positioning
- lead economics
- marketing performance
- sales opportunities
- commercial prioritization
- revenue-related product thinking

Hermes / Abel should reason from real available data.

Do not fabricate missing commercial numbers.

Unknown numbers must remain unknown unless they are explicitly estimated and clearly labeled.

---

# 17. Commercial-to-Product Flow

When Hermes / Abel identifies a software/product opportunity from commercial analysis:

HERMES / ABEL
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

Difficult technical reasoning is handled dynamically by Hermes / Abel using available tools.

This includes:

- difficult architecture decisions
- complex debugging
- deep code analysis
- hard algorithmic reasoning
- difficult implementation strategy
- independent technical review
- resolving technically ambiguous problems

Hermes / Abel may:
- reason through the problem directly
- consult documentation
- run experiments
- escalate to Adham if the decision exceeds scope

---

# 19. Historical Note

Previous versions of Project Alpha OS included Meter, Longcat, and Codex OAuth as dedicated agent roles. These were removed to keep the architecture intentionally small. Task classifications (COMMERCIAL, ESCALATION, LIGHTWEIGHT) remain as categories but no longer have dedicated agents. Hermes / Abel handles them dynamically using the available tools and agents.
