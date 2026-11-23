# vin-spec

My personal framework for working with AI on everyday tasks, engineering, research, and learning.

This system should help me understand the work, participate in reasoning and implementation, and gradually develop working methods I can understand, control, and revise.

## Working Together

- Start with the problem I want to work on today, and choose the appropriate skills as needed.
- Work through engineering and research with me. Explain the purpose of new folders, code, and important logic, and how they relate to the rest of the project.
- Use plain language and provide a manageable amount of information at a time. Decide how to divide the work and how much assistance to provide for each task.
- Discuss results in text first. Before producing additional outputs such as HTML pages, reports, or videos, discuss their purpose and format, and let me decide whether to create them.
- Before adding files or folders to vin-spec or vin-log, explain their location, name, purpose, and contents, and obtain my approval before creating them.

## Adapting Skills

Understand the methods in each source skill individually. Then discuss whether to adopt it, which parts to keep, how to adapt it, what to call it, how to invoke it, and its scope.

Credit every skill actually consulted, adopted, or adapted. Record its source and the parts borrowed, and distinguish the original instructions from my ideas and Codex's suggestions.

The source register is [SOURCES.md](SOURCES.md) at the root of this repository. It records source versions, borrowed methods, and adaptations.

## Research and Mathematics

The research workflow currently under discussion is:

1. Map the literature related to the topic, its main research directions, and the value of reading each paper.
2. Learn about important journals, classic papers, and highly cited work, then decide the reading order.
3. Read the selected papers closely, paragraph by paragraph.
4. In guided-reading mode, Codex leads chapter by chapter, I explain my understanding and answer questions, and I can interrupt to ask for explanations or additional derivations.
5. Develop research questions and candidate explanations from the literature and derivations, compare their predictions, and plan appropriate verification.
6. Implement code and compare the theory with practical results.

My standard for understanding a mathematical theory is being able to derive it independently, by hand, on a whiteboard.

The working environments covered include MATLAB, Ubuntu, ROS / ROS 2, C++, and Python, with the details discussed according to each project's needs.

## Roles of the Two Repositories

- **vin-spec (public):** Collaboration rules, skills adopted after individual discussion and approval, and their sources.
- **vin-log (private):** Work logs, learning and research notes, mathematical derivations, issues, and progress. Code may also live in separate project repositories linked from the records.

## Current Status

The [vin-spec entry](skills/vin-spec/SKILL.md) provides:

- [paper-guide](skills/vin-spec/references/paper-guide.md)
  for guided paper reading.
- [learning-coach](skills/vin-spec/references/learning-coach.md)
  for learning routes, cumulative progress, and continuity across sessions.
- [hypothesis-generation](skills/vin-spec/references/hypothesis-generation.md)
  for research questions, competing explanations, and verification plans.

All three modes use the same explicit and natural entry methods once
loaded into Codex. Other workflows remain under discussion;
installation and verification on each computer are separate setup steps.
