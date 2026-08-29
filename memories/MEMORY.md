# Project Alpha Persistent Memory

## Purpose

This file stores durable cross-project knowledge, standards, and lessons for Project Alpha.

It should shape future projects without duplicating the operating rules already defined in Project Alpha OS.

Project-specific requirements belong with their individual projects.

---

# 1. Project Alpha Identity

Project Alpha should be known for:

- premium websites
- unusual digital experiences
- business systems
- automation
- fast execution

Project Alpha should not compete by producing ordinary template websites faster.

The goal is to produce work that feels intentionally designed and technically capable.

---

# 2. Premium Website Standard

When Project Alpha describes a website as premium or high-tier, that generally means considering:

- GSAP
- advanced purposeful animation
- cinematic presentation
- strong visual storytelling
- 3D where appropriate
- high-quality interaction design
- strong typography
- distinctive composition
- excellent desktop execution
- excellent mobile execution

For suitable projects, a cinematic hero may use a high-quality looping video approximately 5–10 seconds long.

Animation should contribute to the experience rather than simply increase motion density.

---

# 3. Generic Output Is Unacceptable

Project Alpha websites should not look like generic templates commonly found across the web.

Avoid recurring AI-generated patterns such as:

- predictable SaaS layouts
- repetitive card sections
- generic hero compositions
- weak typography
- arbitrary gradients
- excessive glassmorphism
- identical visual systems across unrelated clients
- decorative effects without purpose

Every serious client website should have its own visual identity.

---

# 4. Typography Standard

Bad typography can make an otherwise functional website unacceptable.

Typography must be treated as a primary design element.

Evaluate:

- font selection
- hierarchy
- scale
- weight
- line height
- line length
- spacing
- Arabic typography separately from English typography

Do not accept weak typography merely because the layout technically works.

---

# 5. Website Baseline

Unless the project requires otherwise, public-facing Project Alpha websites should consider:

- strong desktop experience
- equally strong mobile experience
- technical SEO
- deliberate keyword strategy
- indexing readiness
- Cloudflare deployment/infrastructure
- Arabic and English when the project is bilingual

Admin panels are NOT automatically required.

Build an admin panel only when the project needs one.

---

# 6. Arabic / English Philosophy

Arabic/English websites should NOT be treated as:

English page
→ literal translation
→ Arabic page

They should be planned as two intentional versions of the same brand/product.

Each language may require its own:

- composition
- typography
- content rhythm
- hierarchy
- wording
- spacing
- visual balance
- interaction details

Arabic RTL and English LTR should both feel intentionally designed.

The goal is not translation parity.

The goal is experience quality in both languages.

---

# 7. Prototype-First Philosophy

For substantial products, Project Alpha generally prefers to build the visual prototype before wiring production infrastructure.

The first serious prototype should look close to the final production product.

It should normally include:

- realistic mock data
- all major pages
- finished visual design
- desktop experience
- mobile experience
- animations
- interactions
- navigation
- realistic content presentation

The prototype should be convincing enough to evaluate the actual product experience.

It must not look like an unfinished wireframe unless a wireframe was explicitly requested.

---

# 8. Prototype Infrastructure Boundary

During the visual prototype stage, do NOT wire real infrastructure unless specifically requested.

Normally leave disconnected:

- database
- authentication
- payments
- emails
- WhatsApp
- external APIs
- real admin actions
- other production-side integrations
Use realistic connected mock state when necessary to demonstrate workflows.

First prove the product experience.

Then wire the real system.

---

# 9. Prototype Asset Standard

Prototype visuals must use HIGH-QUALITY real assets.

For images and videos:

- obtain high-quality assets appropriate to the project
- prefer visually credible professional material
- use assets that support the intended brand and product
- maintain sufficient resolution for the intended presentation

NEVER substitute geometric shapes, abstract blocks, fake CSS constructions, or primitive generated figures to imitate real photography, products, environments, machinery, people, video footage, or other real-world imagery.

This is especially important for:

- hero sections
- product imagery
- industrial websites
- premium brand websites
- cinematic experiences
- background video
- editorial imagery

Geometric / abstract visual design is allowed when it is deliberately part of the requested art direction.

It must not be used as a cheap substitute for real assets.

---

# 10. Visual Concept Selection

When multiple strong visual directions are possible, prefer describing the concepts first.

For example:

Concept A
→ cinematic editorial

Concept B
→ experimental industrial

Concept C
→ minimal luxury

Explain enough for Adham to choose a direction before spending substantial time building multiple full prototypes.

Only build multiple prototypes when doing so has clear decision value.

---

# 11. Creative Freedom

Cursor should have substantial creative and technical freedom.

It should:

- challenge weak ideas
- propose stronger concepts
- improve obvious weaknesses
- use its technical expertise
- freely refactor weak implementation where appropriate
- continue improving a technically correct but visually weak result before presenting it

Cursor is expected to know the technical materials better than Adham and may choose the most appropriate implementation stack.

Next.js and GSAP are strong recurring preferences for modern premium websites, but they are not mandatory when another approach is clearly superior.

---

# 12. Major Architecture Changes

If Cursor identifies a substantially better architecture than the one currently planned, it should propose the change before executing it.

Minor implementation decisions do not require interruption.

Major architectural changes that materially affect:

- scope
- maintainability
- infrastructure
- cost
- security
- data
- delivery
- future development

should be surfaced before proceeding.

---

# 13. Question / Assumption Standard

One of the recurring failures of AI coding agents is making assumptions when important information is unclear.

Project Alpha prefers:

LOW-RISK / NON-CRITICAL UNCERTAINTY
→ use professional judgment and continue

UNCERTAINTY THAT COULD CAUSE THE FINAL RESULT TO FAIL
→ stop and ask the right question

Do not interrupt Adham for routine technical details that Cursor can safely decide.

Do interrupt when uncertainty materially threatens the product outcome.

---

# 14. Important Interruption Triggers

Adham especially wants to be consulted when:

- a decision requires spending money
- work needs to route outside the established Project Alpha OS path
- an agent has hit a wall and is repeatedly retrying without meaningful progress
- a critical unknown could make the final result fail
- a major architecture change requires approval

Do not hide these situations behind repeated autonomous attempts.

---

# 15. Large Project Build Pattern

For substantial projects, preferred progression is:

REQUIREMENTS
↓
TECHNICAL PLANNING
↓
HIGH-QUALITY VISUAL PROTOTYPE
↓
REVIEW / IMPROVEMENT
↓
APPROVAL
↓
REAL SYSTEM WIRING
↓
VALIDATION
↓
DEPLOYMENT

The prototype is not merely an early sketch.

It is the visual proof of the intended finished product.

---

# 16. Refactoring Philosophy

Weak existing implementation may be freely refactored when doing so materially improves the product.

Do not preserve bad code merely because it already exists.

At the same time:
- avoid unnecessary rewrites
- preserve working architecture when it is sound
- surface major architectural replacement decisions before executing them

---

# 17. Visual Quality Gate

A technically correct implementation can still fail Project Alpha review.

If a design is:

- generic
- visually weak
- poorly typeset
- awkward on mobile
- badly animated
- inconsistent
- obviously unfinished

it should continue through improvement rather than being presented as complete.

Technical correctness is necessary.

It is not sufficient.

---

# 18. Completion Standard

For website work, Project Alpha does not treat generated code as completion.

Before a final completion claim, the actual experience should be:

- reviewed
- tested
- visually inspected
- scrolled through
- interacted with
- checked on relevant desktop sizes
- checked on relevant mobile sizes
- evaluated for visible defects

When the project is intended for Cloudflare production, final completion means the approved product has also been successfully deployed to Cloudflare.

A passing build alone is not "finished."

---

# 19. Completion Honesty

Another recurring AI-agent failure is saying work is finished while important things remain unclear.

Never hide uncertainty behind completion language.

If something remains unclear:

state it.

If something could not be tested:

state it.

If something remains visually weak:

state it.

If something needs Adham's judgment:

state it.

Evidence matters more than confidence language.

---

# 20. Visual Review Principle

If the actual visual result is mediocre, Cursor must not silently approve it.

Cursor should tell Adham:

- what appears weak
- why it appears weak
- what evidence supports that judgment
- what could be improved

Adham then decides whether the result should be revised.

---

# 21. Asset Quality Is Product Quality

Premium design cannot be rescued by poor assets.

High-quality:

- photography
- video
- product images
- textures
- illustrations
- 3D assets

can be as important as layout and code.

Asset selection should therefore be treated as part of design execution, not as placeholder work.

---

# 22. SEO Standard

For public websites, SEO should be considered during the build rather than bolted on after completion.

Relevant concerns may include:

- search intent
- keyword strategy
- semantic content structure
- metadata
- canonical URLs
- sitemap
- robots
- structured data
- hreflang
- performance
- indexability

SEO copy should still sound natural and appropriate to the business.

Do not sacrifice premium presentation for keyword stuffing.

---

# 23. Durable Project Alpha Principle

Project Alpha should combine:

HIGH-END EXPERIENCE
+
STRONG ENGINEERING
+
FAST EXECUTION
+
REAL VALIDATION

Do not trade away one of these unnecessarily.

The objective is not merely to make software work.

The objective is to produce something Project Alpha is comfortable putting its name on.

