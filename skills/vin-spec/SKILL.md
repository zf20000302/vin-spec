---
name: vin-spec
description: >
  Guide research and engineering through literature discovery and comparison,
  critical appraisal, citation checks, paper and code walkthroughs, learning
  routes, hypothesis testing, debugging, and completion verification.
  Use for related research or engineering requests, including continuing
  saved work and connecting mathematical reasoning to implementation.
---

# vin-spec

Use the relevant mode for the user's research or engineering task.

## Two ways to start

- Explicit: the user mentions "$vin-spec" with the task, such as
  "$vin-spec Compare these papers", "$vin-spec Guide me through this code",
  or "$vin-spec Help me investigate this failure". In Codex CLI or the
  IDE extension, the user can also run /skills and select vin-spec.
- Natural conversation: recognize requests to read papers or code
  together, plan learning, compare literature or hypotheses, check
  citations, investigate failures, or verify completed work, including
  equivalent requests in the user's language.

Both entries use the same mode selection. Read only the references
relevant to the task:

- **literature-review:** Read [references/literature-review.md](references/literature-review.md) to map an area, select papers, compare methods and metrics, and synthesize evidence.
- **scientific-critical-thinking:** Read [references/scientific-critical-thinking.md](references/scientific-critical-thinking.md) to appraise assumptions, reasoning, validation, and applicability.
- **citation-management:** Read [references/citation-management.md](references/citation-management.md) to verify source identity, versions, citation metadata, and claim support.
- **paper-guide:** Read [references/paper-guide.md](references/paper-guide.md) to read a selected paper together by chapter or section.
- **learning-coach:** Read [references/learning-coach.md](references/learning-coach.md) to plan learning routes, maintain progress, and resume across sessions.
- **hypothesis-generation:** Read [references/hypothesis-generation.md](references/hypothesis-generation.md) to form research questions, compare explanations, and plan discriminating tests.
- **learn-codebase:** Read [references/learn-codebase.md](references/learn-codebase.md) to read implementations, trace data flow, and connect formulas to code.
- **systematic-debugging:** Read [references/systematic-debugging.md](references/systematic-debugging.md) to investigate failures, test candidate causes, and make scoped fixes.
- **verification-before-completion:** Read [references/verification-before-completion.md](references/verification-before-completion.md) to check deliverables and support completion claims with appropriate evidence.

Answer isolated questions directly and use the active context when
relevant. Let the user redirect the work.

## Working together

- Use the user's language and plain wording. Keep explanations in
  manageable chunks.
- Let the user interrupt, question, restate, or change the depth.
- Keep original claims, supplementary reasoning, and the user's own
  understanding distinct.
- Discuss purpose and format and obtain approval before producing
  additional artifacts such as HTML guides, reports, or videos.
- Before creating any file or folder in vin-spec or vin-log, explain
  the repository, path, purpose, and intended contents. Reuse existing
  authorization, including explicit delegation to integrate agreed
  workflows automatically. Ask only when the additions exceed or
  lack the required authorization.

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
