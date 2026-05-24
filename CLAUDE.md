# ATLAS — Context for Claude

## Who you're working with
An automation engineer in a pharmaceutical manufacturing environment. Work is performed under **GAMP 5** and **FDA** oversight in a **fully audited (GxP)** setting. Decisions ultimately drive **physical equipment** — bad output has consequences beyond software.

## What ATLAS is for
An **AI co-pilot for ISA-88-compliant automation design**. ATLAS exists to help a capable engineer:
- design batch systems faster,
- verify decisions against standards and prior context,
- and shepherd the process from stakeholder input through to qualified, deployable code.

The human engineer remains the decision-maker. ATLAS proposes; the engineer disposes.

## Scope ambition (north star)
End-to-end coverage of the design lifecycle:
1. **Inputs** from all stakeholders — MS&T, Engineering, Operations, Quality, etc.
2. **Design artifacts** — narratives, ISA-88 decomposition, physical model (ISA-5.1), phase sequences, FRS.
3. **Outputs** — executable code (e.g. DeltaV FHX) **plus** a **qualification plan** and every required document produced along the way.

Today's prototype covers the middle of that pipeline (see README). The ambition is the full span.

## Relationship to STARS (future project)
**STARS** will define the *standards layer* ATLAS operates within:
- which deliverables are required at each lifecycle stage,
- the format each deliverable follows,
- and the best practices we adopt as an organization.

When STARS exists, ATLAS will be grounded in it. Until then, treat standards/format decisions as **provisional** and flag them as places STARS will eventually govern.

## Working principles
- **Regulatory awareness:** assume GxP. Traceability, reviewability, and auditability matter more than cleverness.
- **Physical consequence:** this drives real equipment. Prefer cautious, explicit, reviewable output over confident shortcuts.
- **Engineer-in-the-loop:** every AI output is a draft for a qualified engineer to accept, edit, or reject.
- **Synthetic data only** in the prototype; no real product/process data.

## Tech surface
Client-side only — `index.html` + JS, no build step. Claude Sonnet 4.6 via the Messages API. See README for the user-facing pipeline and stack details.
