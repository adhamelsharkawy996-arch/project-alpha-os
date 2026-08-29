# Project Alpha OS v3 — Project Registry

## Purpose

This file is the canonical registry of Project Alpha projects.

It exists to prevent:

- modifying the wrong project
- guessing project directories
- confusing similarly named projects
- losing project status between sessions
- mixing project-specific context
- accidental cross-project changes

Before substantial project work, Cursor must resolve the requested project through this registry.

---

# 1. Core Rule

A project is NOT considered registered until its actual workspace has been verified.

Never invent or infer a filesystem path.

Never modify a project based only on a remembered project name.

Correct flow:

PROJECT REQUEST
↓
RESOLVE PROJECT NAME
↓
CHECK REGISTRY
↓
VERIFY WORKSPACE
↓
LOAD PROJECT CONTEXT
↓
PLAN / EXECUTE

---

# 2. Project Identity

Every registered project should have:

- canonical project ID
- project name
- aliases
- client/company if applicable
- project type
- verified workspace
- current status
- current phase
- primary stack if known
- deployment target if known
- important project files
- last verified date
- relevant notes

---

# 3. Canonical Project ID

Use stable lowercase IDs.

Examples:

project-alpha-site

mina-lens

al-ostaz

trade-research

marketplace-platform

Do not rename a canonical project ID casually.

Display names may change.

---

# 4. Project Resolution

When Adham mentions a project:

1. attempt exact canonical-name match
2. check registered aliases
3. inspect context if there is one clear match
4. if ambiguity remains, ask Adham
5. verify the workspace before modification

Example:

Adham:
"Open the Mina project."

Possible alias resolution:

mina
mina lens
mina website
mina-lens

→ canonical ID:

mina-lens

But only if that alias has been registered.

---

# 5. Workspace Verification

A workspace is VERIFIED only when its real filesystem location has been confirmed.

Example:

Workspace:
/home/adham/projects/example

Workspace status:
VERIFIED

Never mark a guessed path VERIFIED.

If the project exists but its location is not known:

Workspace:
UNKNOWN

Workspace status:
UNVERIFIED

No modification is allowed until resolved.

---

# 6. Project Status Values

Use one of:

## ACTIVE

Currently under active development.

## PLANNING

Requirements / architecture phase.

## PAUSED

Known project, intentionally not being worked on.

## MAINTENANCE

Production/live project receiving fixes or updates.

## COMPLETED

Primary project scope completed.

## ARCHIVED

No longer active but retained for reference.

## BLOCKED

Cannot currently proceed.

## UNKNOWN

Status has not yet been verified.

---

# 7. Project Phase

Optional current phase examples:

- discovery
- requirements
- planning
- architecture
- prototype
- implementation
- QA
- client-review
- deployment
- production
- maintenance

Do not invent a phase when it is unknown.

---

# 8. Active Project Pointer

Current active project:

NONE

Current verified workspace:

NONE

Rule:

Do not treat the previously used project as the active project for a new request unless context clearly establishes continuation.

When Adham explicitly switches projects, update this section.

---

# 9. Safe System Workspaces

These are NOT client production projects.

## Project Alpha OS

ID:

project-alpha-os

Type:

internal operating system

Workspace:

/home/adham/project-alpha-os

Workspace status:

VERIFIED

Status:

ACTIVE

Purpose:

Project Alpha OS v3 configuration, routing, memory, registry, and operating policy.

GitHub:

github.com/adhamelsharkawy996-arch/project-alpha-os

Production project:

NO

---

## Cursor Test Workspace

ID:

cursor-test

Type:

temporary system validation workspace

Workspace:

/home/adham/cursor-test

Workspace status:

VERIFIED

Status:

ACTIVE

Purpose:

Safe testing of Cursor CLI and Project Alpha execution workflows.

Production project:

NO

Allowed destructive testing:

ONLY when the test explicitly targets this workspace.

---

# 10. Production / Client Project Registry

No production or client workspace should be added here from memory alone.
Each existing project must be verified before registration.

Current production/client projects registered:

NONE VERIFIED YET

This does NOT mean no projects exist.

It means Project Alpha OS v2 has not yet verified and registered their actual workspaces.

---

# 11. Project Registration Template

Use this exact structure for new entries:

---

## [Project Name]

Project ID:

project-id

Aliases:

- alias one
- alias two

Client / Company:

UNKNOWN

Project type:

UNKNOWN

Workspace:

UNKNOWN

Workspace status:

UNVERIFIED

Status:

UNKNOWN

Current phase:

UNKNOWN

Primary stack:

UNKNOWN

Primary language / locales:

UNKNOWN

Primary builder:

Cursor

Planning:

Cursor Planning Mode when substantial

Deployment target:

UNKNOWN

Production URL:

UNKNOWN

Important project files:

UNKNOWN

Last verified:

NEVER

Notes:

None.

---

# 12. Registering an Existing Project

Before registering an existing project:

1. determine its real directory
2. inspect enough files to confirm identity
3. verify the project name
4. verify whether it is active/live/paused
5. identify the primary stack when useful
6. add aliases Adham commonly uses
7. record the verification date
8. avoid unnecessary historical detail

Do not alter the project merely to register it.

Registration is inspection only.

---

# 13. Registering a New Project

When Adham starts a new software project:

1. gather requirements
2. establish canonical project name
3. establish project ID
4. establish intended workspace
5. create/register workspace when authorized
6. mark status PLANNING
7. invoke Cursor Planning Mode when substantial
8. update registry as implementation begins

Typical lifecycle:

PLANNING
↓
ACTIVE
↓
QA
↓
MAINTENANCE / COMPLETED

---

# 14. Project Blueprint Relationship

The registry is NOT the project blueprint.

PROJECT_REGISTRY.md answers:

"What project is this and where is it?"

A project blueprint answers:

"What are we building and how?"

Large projects should maintain their own persistent planning documentation inside the project or a designated blueprint location.

Do not overload the registry with detailed architecture.

---

# 15. Project-Specific Memory

Do not store large amounts of project-specific detail in global OS memory.

Project-specific facts should preferably live:

1. in the project itself
2. in its blueprint/state documentation
3. in PROJECT_REGISTRY.md only when required for identification/routing

Global memory should contain only durable cross-project information.

---

# 16. Project Switching

When Adham switches projects:

Cursor should:

1. resolve the new project
2. update Active Project Pointer if appropriate
3. load the new project's relevant context
4. stop applying assumptions from the previous project
5. keep workspaces isolated

Never carry unresolved implementation assumptions across projects.

---

# 17. Ambiguous Project Names

If multiple projects could match the same name:

DO NOT GUESS.

Example:

"the gelatin website"

If multiple registered projects relate to gelatin, Cursor must resolve the ambiguity before modification.

Aliases should reduce this problem over time.

---

# 18. Workspace Boundary

Cursor must operate from the verified workspace associated with the selected project.

Example:

Registered workspace:

/home/adham/projects/client-a

Then Cursor implementation should be scoped to that workspace.

Do not invoke Cursor from /home/adham for normal project modifications.

Do not use --trust on arbitrary unverified directories.

---

# 19. Production Identification

For live projects, record when verified:

Production URL:

Deployment platform:

Production status:

This helps prevent confusion between:

- local development
- staging
- production

Never assume a local project maps to a particular production site without verification.

---

# 20. Secrets

Never store secrets in this registry.

Allowed:

Environment variable name:

DATABASE_URL

Not allowed:

Actual database password or connection secret.

Allowed:

Secret location:

.env.production

Not allowed:

Contents of the secret.

---
# 21. Registry Updates

Update the registry when:

- a project is created
- a workspace is verified
- a project is renamed
- an alias becomes useful
- status materially changes
- production URL is established
- stack materially changes
- project is archived
- active project changes

Do not update it for ordinary commits or tiny implementation details.

---

# 22. Verification Date

Use an explicit date whenever a project is materially re-verified.

Format:

YYYY-MM-DD

Example:

2026-08-25

Old registry information should never override newly verified reality.

---

# 23. Registry Integrity

This file is the canonical global project index.

Do not maintain competing project registries elsewhere unless they serve a clearly different purpose.

If conflicting project information appears:

1. inspect current reality
2. correct this registry
3. correct stale persistent state
4. proceed only after the workspace is clear

---

# 24. Current Registry Verdict

Project Alpha OS:

REGISTERED / VERIFIED

Cursor test workspace:

REGISTERED / VERIFIED

Production/client projects:

NOT YET VERIFIED UNDER OS v3

Active production project:

NONE

Registry status:

READY FOR PROJECT DISCOVERY
