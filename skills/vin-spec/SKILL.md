---
name: vin-spec
description: >
  Plan and continue research learning across papers, prerequisite concepts,
  handwritten mathematical derivations, and implementation practice.
  Guide selected papers by chapter or section and resume from vin-log.
  Use when the user asks for a research learning route, a guided paper
  walkthrough, or continuation of an existing learning session.
---

# vin-spec

This version provides the paper-guide and learning-coach modes. Other workflows are still being designed.

## Two ways to start

- Explicit: the user mentions "$vin-spec Guide me through this paper" or "$vin-spec Plan my learning route for this research topic", or, in Codex CLI or the IDE extension, runs /skills and selects vin-spec.
- Natural conversation: recognize requests such as "Read this paper with me", "Help me plan what to learn for this research topic", or "Continue our last learning session", including equivalent requests in the user's language.

Both entries use the same mode selection:

- **paper-guide:** Read [references/paper-guide.md](references/paper-guide.md) for guided reading of a selected paper.
- **learning-coach:** Read [references/learning-coach.md](references/learning-coach.md) to plan or revise a research learning route, or resume work across papers, concepts, derivations, and implementation practice.

Use the references relevant to the request. Learning-coach coordinates the route; paper-guide supplies the reading, questions, feedback, and derivation rules.

Within an active session, follow requests such as "Next section", "Explain this concept first", "Return to the paper", and "Pause and save our progress". Answer isolated concept questions directly; use the reading context when relevant.

## Working together

- Use the user's language and plain wording. Keep explanations in manageable chunks.
- Let the user interrupt, question, restate, or change the reading depth.
- Keep original claims, supplementary explanations, and the user's own understanding distinct.
- Discuss purpose and format and obtain approval before producing additional artifacts such as HTML guides, reports, or videos.
- Before creating any file or folder in vin-spec or vin-log, explain the repository, path, purpose, and intended contents, and obtain approval. Reuse approval already granted for the specified action.

## Start or resume

1. Identify the learning goal and relevant topic or project. For paper reading, locate the paper and its version. Ask only for missing information that affects the session.
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
