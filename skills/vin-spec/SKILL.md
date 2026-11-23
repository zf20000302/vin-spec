---
name: vin-spec
description: >
  Guide research and engineering through literature discovery and comparison,
  critical appraisal, citation checks, paper and code walkthroughs, learning
  routes, spec-driven project planning, algorithm proposals, hypothesis testing, debugging,
  behavior tests, code review, delivery, and completion verification.
  Use for related research or engineering requests, including continuing
  saved work and connecting mathematical reasoning to implementation.
---

# vin-spec

Use the relevant mode for the user's research or engineering task.

## Two ways to start

- Explicit: the user mentions "$vin-spec" with the task, such as
  "$vin-spec Compare these papers", "$vin-spec Guide me through this code",
  "$vin-spec Help me investigate this failure", or "$vin-spec Plan a new project using SDD". In Codex CLI or the
  IDE extension, the user can also run /skills and select vin-spec.
- Natural conversation: recognize requests to read papers or code
  together, plan learning, compare literature or hypotheses, check
  citations, plan or execute project work, review changes, prepare delivery,
  investigate failures, or verify completed work, including
  equivalent requests in the user's language.

Both entries use the same mode selection. Read only the references
relevant to the task:

- **literature-review:** Read [references/literature-review.md](references/literature-review.md) to map an area, select papers, compare methods and metrics, and synthesize evidence.
- **scientific-critical-thinking:** Read [references/scientific-critical-thinking.md](references/scientific-critical-thinking.md) to appraise assumptions, reasoning, validation, and applicability.
- **citation-management:** Read [references/citation-management.md](references/citation-management.md) to verify source identity, versions, citation metadata, and claim support.
- **paper-guide:** Read [references/paper-guide.md](references/paper-guide.md) to read a selected paper together by chapter or section.
- **learning-coach:** Read [references/learning-coach.md](references/learning-coach.md) to plan learning routes, maintain progress, and resume across sessions.
- **spec-driven-development:** Read [references/spec-driven-development.md](references/spec-driven-development.md) for project scope, design choices, algorithm proposals, confirmed arrangement, planning, implementation, behavior tests, review, and delivery.
- **hypothesis-generation:** Read [references/hypothesis-generation.md](references/hypothesis-generation.md) to form research questions, compare explanations, and plan discriminating tests.
- **learn-codebase:** Read [references/learn-codebase.md](references/learn-codebase.md) to read implementations, trace data flow, and connect formulas to code.
- **systematic-debugging:** Read [references/systematic-debugging.md](references/systematic-debugging.md) to investigate failures, test candidate causes, and make scoped fixes.
- **verification-before-completion:** Read [references/verification-before-completion.md](references/verification-before-completion.md) to check deliverables and support completion claims with appropriate evidence.

Answer isolated questions directly and use the active context when
relevant. Let the user redirect the work.

## Engineering stages within SDD

The following names select stages inside the existing SDD mode.
They share the vin-spec entry and do not require separate skill folders:

- **brainstorming:** Use [clarify needs and compare viable approaches](references/spec-driven-development.md#clarify-goals-and-compare-approaches).
- **writing-plans:** Use [write concrete tasks and verification](references/spec-driven-development.md#write-an-actionable-plan).
- **executing-plans:** Use [implement and keep resumable progress](references/spec-driven-development.md#execute-with-checkpoints).
- **test-driven-development:** Use [use meaningful test-first behavior checks](references/spec-driven-development.md#test-behavior-before-implementation).
- **requesting-code-review:** Use [prepare requirements, change scope, and evidence for review](references/spec-driven-development.md#request-and-handle-review).
- **receiving-code-review:** Use [evaluate feedback before correcting the code](references/spec-driven-development.md#request-and-handle-review).
- **using-git-worktrees:** Use [arrange explicitly approved workspace isolation](references/spec-driven-development.md#isolate-work-when-needed).
- **finishing-a-development-branch:** Use [verify, integrate, and hand off authorized work](references/spec-driven-development.md#finish-and-deliver).

Use only the stages relevant to the current task. Preserve prior
decisions and reuse the user's existing authorization.

## Working together

- Use the user's language and plain wording. Keep explanations in
  manageable chunks.
- Let the user interrupt, question, restate, or change the depth.
- Keep original claims, supplementary reasoning, and the user's own
  understanding distinct.
- Discuss purpose and format and obtain approval before producing
  additional artifacts such as HTML guides, reports, or videos.
- Before creating any file or folder in vin-spec or vin-log, present
  the exact paths, names, purposes, and intended contents for the user's
  confirmation. Reuse confirmation only for the paths and arrangement
  already approved.
- For engineering projects, present folder structure, module roles,
  code placement, dependencies, and reasons for confirmation before
  creating or changing that arrangement. Moves, renames, file splits,
  merges, and other reorganizations require the same confirmation.
- Automatic integration authorizes content work within the agreed task
  and confirmed arrangement. It does not by itself approve new paths or
  a different organization. Continue independent authorized work while
  arrangement-dependent changes await confirmation.

For a recommendation to adopt an algorithm or work implementing it,
follow the [algorithm-proposal rules](references/spec-driven-development.md#algorithm-proposal).
Include the architecture diagram and subsystem explanations, and reuse
only the relevant approval already given.

## Start or resume

1. Identify the research or engineering goal and relevant topic or
   project. For paper or code work, locate the source and version.
   Ask only for missing information that affects the task.
2. Use the configured vin-log location or authenticated connection
   to read relevant existing progress. Ask when access is unavailable.
3. Briefly state the current position, remaining gap, and next action.
4. Base continuation on the latest successfully synced record.
   If a source or implementation changed, check the relevant content
   before relying on the earlier interpretation.

## Records

Use approved existing records where possible. Save updates when the
user requests them or has authorized ongoing logging. Preserve existing
work and report unresolved save or sync failures.

vin-log conventions:

- projects/<project>/README.md: goals, current state, decisions, links,
  and next steps.
- knowledge/papers/<paper-id>.md: stable paper notes and reading progress.
- knowledge/math-derivations/<theory>.md: theory and personal derivations.
- knowledge/concepts/<topic>.md: reusable concept notes.
- journal/YYYY/MM/YYYY-MM-DD.md: short dated activity records with links.

A folder convention alone does not authorize creating new paths.
Apply the authorization rule above.

## Verify changes and credit sources

For changed deliverables and completion claims, follow
[verification-before-completion](references/verification-before-completion.md)
with checks appropriate to the actual work and claimed scope.

Sources and adaptations:
[SOURCES.md](https://github.com/zf20000302/vin-spec/blob/main/SOURCES.md).
