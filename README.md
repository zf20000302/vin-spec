# vin-spec

My personal framework for working with AI on everyday tasks, engineering, research, and learning.

This system should help me understand the work, participate in reasoning and implementation, and gradually develop working methods I can understand, control, and revise.

## Working Together

- Start with the problem I want to work on today, and choose the appropriate skills as needed.
- Work through engineering and research with me. Explain the purpose of new folders, code, and important logic, and how they relate to the rest of the project.
- Use plain language and provide a manageable amount of information at a time. Decide how to divide the work and how much assistance to provide for each task.
- Discuss results in text first. Before producing additional outputs such as HTML pages, reports, or videos, discuss their purpose and format, and let me decide whether to create them.
- Before adding files or folders to vin-spec or vin-log, show the exact paths, names, purposes, and contents for my confirmation. Reuse approval only for the placement and arrangement I have already confirmed.
- Confirm project folder structures, module roles, code placement, and their relationships with me before creating or reorganizing them, including moves, renames, file splits, and merges.
- I may delegate automatic content integration within an agreed task and confirmed arrangement. Changes to that arrangement still require my confirmation.
- When recommending an algorithm for adoption, or before implementing it, present an algorithm proposal with an architecture diagram and an explanation of each subsystem. Keep algorithm approval separate from confirmation of folder and code placement.

## Adapting Skills

Understand the methods in each source skill individually. Then discuss whether to adopt it, which parts to keep, how to adapt it, what to call it, how to invoke it, and its scope.

Credit every skill actually consulted, adopted, or adapted. Record its source and the parts borrowed, and distinguish the original instructions from my ideas and Codex's suggestions.

The source register is [SOURCES.md](SOURCES.md) at the root of this repository. It records source versions, borrowed methods, and adaptations.

## Research and Mathematics

The research workflow combines:

1. Map the literature related to the topic, its main research directions, and the value of reading each paper.
2. Learn about important journals, classic papers, and highly cited work, then decide the reading order.
3. Read the selected papers closely, paragraph by paragraph.
4. In guided-reading mode, Codex leads chapter by chapter, I explain my understanding and answer questions, and I can interrupt to ask for explanations or additional derivations.
5. Develop research questions and candidate explanations from the literature and derivations, compare their predictions, and plan appropriate verification.
6. Read relevant implementations, trace data flow, and connect formulas to code before or while making scoped changes.
7. Implement code and compare the theory with practical results.

My standard for understanding a mathematical theory is being able to derive it independently, by hand, on a whiteboard.

The working environments covered include MATLAB, Ubuntu, ROS / ROS 2, C++, and Python, with the details discussed according to each project's needs.

## Engineering Workflow

The SDD mode incorporates the adapted methods from brainstorming,
writing-plans, executing-plans, test-driven-development,
requesting-code-review, receiving-code-review, using-git-worktrees,
and finishing-a-development-branch.

They operate as stages within the same vin-spec entry.
Use the relevant stage for the task and keep algorithm proposals,
folder and code placement confirmation, proportionate verification,
and cumulative progress records.

## Roles of the Two Repositories

- **vin-spec (public):** Collaboration rules, skills adopted after individual discussion and approval, and their sources.
- **vin-log (private):** Work logs, learning and research notes, mathematical derivations, issues, and progress. Code may also live in separate project repositories linked from the records.

## Current Status

The [vin-spec entry](skills/vin-spec/SKILL.md) provides ten connected modes:

- [literature-review](skills/vin-spec/references/literature-review.md) for field mapping, paper selection, metric comparison, and synthesis.
- [scientific-critical-thinking](skills/vin-spec/references/scientific-critical-thinking.md) for claim, assumption, derivation, validation, and applicability appraisal.
- [citation-management](skills/vin-spec/references/citation-management.md) for source identity, versions, references, and claim-support checks.
- [paper-guide](skills/vin-spec/references/paper-guide.md) for guided paper reading and independent derivation assessment.
- [learning-coach](skills/vin-spec/references/learning-coach.md) for learning routes, cumulative progress, and continuity.
- [spec-driven-development](skills/vin-spec/references/spec-driven-development.md) for requirements, design choices, confirmed arrangement, plans, implementation, behavior tests, review, and delivery.
- [hypothesis-generation](skills/vin-spec/references/hypothesis-generation.md) for research questions, rival explanations, and verification plans.
- [learn-codebase](skills/vin-spec/references/learn-codebase.md) for guided implementation reading, data flow, and formula-to-code mapping.
- [systematic-debugging](skills/vin-spec/references/systematic-debugging.md) for evidence-based failure investigation and scoped correction.
- [verification-before-completion](skills/vin-spec/references/verification-before-completion.md) for checks and evidence supporting completion claims.

All modes share explicit and natural entry methods once loaded into Codex.
The selected Socratic rules are incorporated into paper-guide and reused
where relevant.

The SDD mode includes the agreed engineering stages. OpenSpec and Spec Kit
tool integration remains pending as recorded in [SOURCES.md](SOURCES.md). Installation and
verification on each computer are separate setup steps.
