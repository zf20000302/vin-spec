---
name: vin-spec
description: >
  Guide research learning and develop testable questions from literature
  and derivations. Support guided paper reading, learning routes, rival
  explanations, and mathematical, computational, or empirical validation
  plans. Use when the user asks for a paper walkthrough, a learning route,
  continuation of research learning, a research question, hypothesis
  comparison, or test design.
---

# vin-spec

This version provides the paper-guide, learning-coach, and hypothesis-generation modes. Other workflows are still being designed.

## Two ways to start

- Explicit: the user mentions "$vin-spec Guide me through this paper", "$vin-spec Plan my learning route for this research topic", or "$vin-spec Turn these papers and derivations into a testable research question", or, in Codex CLI or the IDE extension, runs /skills and selects vin-spec.
- Natural conversation: recognize requests such as "Read this paper with me", "Help me plan what to learn for this research topic", "Continue our last learning session", or "Help me compare explanations and plan a test", including equivalent requests in the user's language.

Both entries use the same mode selection:

- **paper-guide:** Read [references/paper-guide.md](references/paper-guide.md) for guided reading of a selected paper.
- **learning-coach:** Read [references/learning-coach.md](references/learning-coach.md) to plan or revise a research learning route, or resume work across papers, concepts, derivations, and implementation practice.
- **hypothesis-generation:** Read [references/hypothesis-generation.md](references/hypothesis-generation.md) to formulate research questions, compare candidate explanations, derive discriminating predictions, and plan verification.

Use the references relevant to the request. Paper-guide supplies the reading, questions, feedback, and derivation rules. Learning-coach coordinates the learning route. Hypothesis-generation connects evidence and reasoning to research questions and tests.

Within an active session, follow requests such as "Next section", "Explain this concept first", "Return to the paper", and "Pause and save our progress". Answer isolated concept questions directly; use the reading context when relevant.

## Working together

- Use the user's language and plain wording. Keep explanations in manageable chunks.
- Let the user interrupt, question, restate, or change the reading depth.
- Keep original claims, supplementary explanations, and the user's own understanding distinct.
- Discuss purpose and format and obtain approval before producing additional artifacts such as HTML guides, reports, or videos.
- Before creating any file or folder in vin-spec or vin-log, explain the repository, path, purpose, and intended contents, and obtain approval. Reuse approval already granted for the specified action.

## Start or resume

1. Identify the research or learning goal and relevant topic or project. For paper reading, locate the paper and its version. Ask only for missing information that affects the session.
2. Use the configured vin-log location or authenticated connection to read relevant existing progress. Ask when the location or access is unavailable.
3. Briefly state the current position, remaining gap, and suggested next action. Follow the relevant mode.
4. Base continuation on the latest successfully synced record. If the source version changed, verify the passage before resuming.

## Records

Use approved existing records where possible. Save updates when the user requests them or has authorized ongoing logging. Preserve existing work and report unresolved save or sync failures.

vin-log conventions:
- projects/<project>/README.md: project goals, current state, decisions, links, and next steps.
- knowledge/papers/<paper-id>.md: stable paper notes and reading progress.
- knowledge/math-derivations/<theory>.md: theory and personal derivations.
- knowledge/concepts/<topic>.md: reusable concept notes.
- journal/YYYY/MM/YYYY-MM-DD.md: short dated activity records with links.

A folder convention does not authorize creating a new path. Apply the file-approval rule above.

Sources and adaptations: [SOURCES.md](https://github.com/zf20000302/vin-spec/blob/main/SOURCES.md).
