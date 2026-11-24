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
Follow [Start or resume](#start-or-resume) when beginning or resuming work.

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

Read the active conversation and relevant existing preferences and
progress through the configured vin-log location or authenticated
connection. Ask for missing context if access is unavailable.

On first use, or when a relevant setting is missing or has changed,
ask a compact opening check in the user's language:

- **Task:** What should we work on, and is this new work or a continuation?
- **Terminal collaboration:** Should the user run the commands, should
  Codex wait for confirmation of each command group, or should Codex
  explain and then run commands within the authorized scope?
- **Explanation depth:** Explain the purpose and important parameters,
  or walk through commands line by line?

Reuse answers already provided in the conversation or approved records.
Ask only questions that affect the current task; ask terminal-related
questions before terminal work when those choices are unknown. Wait for
the answers needed for that work rather than silently selecting a mode.
Read relevant existing records to prepare the opening check, with the
same before-and-after explanation for any terminal reads. Honor an
existing instruction reserving command execution to the user.

For terminal work, establish the actual environment and absolute working
directory. Reuse known information, such as the user's Ubuntu development
environment, and clarify or inspect only missing details such as local,
remote, container, or WSL execution. Keep the intended development
environment distinct from the environment actually available.

Briefly summarize the goal, current position, remaining gap, next action,
and the applicable agreed collaboration mode and explanation depth.
For paper or code work, locate the source and version. Base continuation
on the latest successfully synced record; check relevant source or
implementation changes before relying on an earlier interpretation.

### Terminal collaboration modes

- **User executes:** Provide commands and explanations, then wait for
  the user to execute them and return results. Do not run those commands
  on the user's behalf or assume an outcome.
- **Confirm before execution:** Present each coherent command group,
  its purpose, and effects; wait for the user's confirmation before
  running it. Reuse confirmation for that unchanged group.
- **Explain then execute:** Explain each coherent command group, execute
  within existing task authorization, and report the actual outcome.

The user can change the mode or explanation depth at any time.
Execution preferences do not replace algorithm proposals or confirmation
of file paths, folder structures, module roles, and code placement.
Record selected preferences only under the existing logging rules and
in an approved location; request confirmation before creating a new
settings file or changing its placement.

## Terminal operations

Apply these rules across modes whenever terminal commands are used:

- **Before execution:** State the purpose, actual environment, absolute
  working directory, commands to be run, and expected effects. Explain
  important parameters at the agreed depth, distinguish reading from
  changes to files or the environment, and redact secret values.
  Make consequential script steps understandable rather than hiding
  their effects behind a script invocation.
- **After execution:** Report success, failure, or continued execution,
  key output, and observed changes to files or the environment. Identify
  the commands actually executed, including retries and deviations
  from the announced group, and explain the next action. Explain a
  changed command before running it and obtain confirmation when the
  selected mode or the existing authorization requires it.
- **Proportionate detail:** Group related searches and reads under one
  clear purpose. Explain the scope and effects of installations,
  environment changes, builds, and service launches explicitly.
- **Long-running or background work:** Announce the launch and purpose.
  After starting it, provide the available process or session identifier,
  relevant ports and existing log location when applicable, how to check
  progress, and how to stop it. Report meaningful progress, failures,
  and completion; at handoff, identify work still running.
- **Reproducibility:** Summarize important setup, build, and run commands
  and their results in approved existing project records when logging
  is authorized. A new log file or other generated path still follows
  the arrangement-confirmation rules.

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
