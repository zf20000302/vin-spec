# Sources and Adaptations

Last updated: 2026-11-23.

This register distinguishes methods used in the current vin-spec workflows, authoring support, and candidates consulted during the wider design discussion. A listed candidate is not automatically an implemented mode or a runtime dependency.

## Confirmed design decisions

The vin-spec design discussions established the single entry, explicit and natural invocation, chapter-led reading, the user's explanations and answers, interruptible teaching detours, return points, the independent whiteboard-derivation standard, cumulative vin-log records, and approval before creating files or folders.

These decisions are recorded separately from the upstream authors' rules.

## Methods used in this draft

| Source | Use in this draft |
| --- | --- |
| [literature-guide-read](https://github.com/Liangzhen-Chen/literature-guide-read/blob/f47dbd8a5ca7d5568b60c2d8da53125257f9e2c9/SKILL.md) and its [reading method](https://github.com/Liangzhen-Chen/literature-guide-read/blob/f47dbd8a5ca7d5568b60c2d8da53125257f9e2c9/references/method.md), Liangzhen-Chen / literature-guide-read contributors | Passage-level grounding; identifying paragraph roles, definitions, formulas, evidence, and qualifications; connecting reasoning steps; part-by-part walkthroughs and recall questions. |
| [literature-review](https://github.com/K-Dense-AI/scientific-agent-skills/blob/ec59a29a03d5c40f73ab40878df04860bc00e876/skills/literature-review/SKILL.md), K-Dense Inc., v1.11 | Linking summarized claims to the actual source and preserving the scope of the supporting evidence. Its complete search and review workflow is not implemented in this version. |
| [scientific-critical-thinking](https://github.com/K-Dense-AI/scientific-agent-skills/blob/ec59a29a03d5c40f73ab40878df04860bc00e876/skills/scientific-critical-thinking/SKILL.md), K-Dense Inc., v1.5 | Attention to assumptions, reasoning, claim scope, and the distinction between missing information and a demonstrated error. Its full appraisal workflow is not implemented in this version. |
| [socratic-tutor](https://github.com/janestreet/agent_skills/blob/469868f4489cbdbe178c775a0af05bb6bef63689/socratic-tutor/SKILL.md), Jane Street Group, LLC | Focused questions about reasons, predictions, new examples, and missing conditions; evidence-based feedback and progress checks. The diagnostic and 0–5 states are adapted below. |
| [learning-coach](https://github.com/cheng-dp/learning-coach-skill/blob/a64963bee49fee0e3aba1b5af648e545bb48bba0/SKILL.md) and its [workflow references](https://github.com/cheng-dp/learning-coach-skill/tree/a64963bee49fee0e3aba1b5af648e545bb48bba0/references), cheng-dp / Learning Coach Skill contributors | Goal-based milestones, progress-informed session planning, durable checkpoints, adaptive routes, and targeted review. Adapted to the existing vin-log classification and whiteboard-derivation standard. |

Reviewed snapshots:
- literature-guide-read: f47dbd8a5ca7d5568b60c2d8da53125257f9e2c9.
- Scientific Agent Skills: ec59a29a03d5c40f73ab40878df04860bc00e876.
- Jane Street agent_skills: 469868f4489cbdbe178c775a0af05bb6bef63689.
- Learning Coach Skill: a64963bee49fee0e3aba1b5af648e545bb48bba0.

The adaptation uses a conversational chapter loop, user-directed detours, explicit return points, and vin-log checkpoints. Upstream HTML generation, scripts, assets, and fixed reading-density quotas are not included in this draft. Detailed mathematical checking also reflects the user's requirements and the design discussion.

## Socratic adaptation

- Use an adaptive diagnostic, normally one to three questions, informed by existing progress. Teach unfamiliar prerequisites before asking the user to apply them.
- Ask one focused question at a time, give specific feedback, and provide hints or direct explanation according to the user's needs.
- Redefine the 0–5 progression for named mathematical targets. Keep not assessed separate from level 0, make independent handwritten derivation the level-4 target, and use level 5 for optional transfer and teaching.
- Distinguish attainment in one attempt from reconfirmation on another occasion. Record the date, assistance, the user's confirmation of independence, and which written reasoning was reviewed.
- Detailed rules are in paper-guide.md. The upstream fixed diagnostic gate, mandatory failed attempts before explanation, automatic progress graphics, and unannounced retests are not carried over.

## Learning-coach adaptation

- Describe milestones through research purpose, learning material, prerequisites, observable abilities, and completion checks.
- Map route and progress roles to the existing project, paper, derivation, concept, and journal conventions. Keep detailed evidence in stable knowledge records and link to it from summaries.
- Separate activity completion from demonstrated understanding. Reuse paper-guide's target-specific whiteboard standard and evidence rules.
- Resume from synced records, preserving the exact position, unfinished task, and detour return points.
- Choose checks according to the target and gaps, and agree later review with the user.
- The upstream separate course-file layout, fixed phase or assessment counts, and optional calendar intervals are adapted to the user's existing organization and learning preferences. Logging and new-path creation remain subject to the user's approval rules.

## Authoring and preparation support

- **skill-creator**, supplied with Codex: consulted for scope, concise instructions, and supporting references.
- **openai-docs**, supplied with Codex: consulted to verify discovery, invocation, and loading behavior against [OpenAI's Build skills documentation](https://learn.chatgpt.com/docs/build-skills).
- **computer-use**: preparation tooling for reading the user-provided shared discussion; no computer-control procedure is part of this skill.
- Locally installed **bmad-deep-recon** and **bmad-review** were inspected for applicability; their workflows were not adopted.

Local authoring and preparation revisions are not pinned in this register. These skills are not required runtime dependencies.

## Consulted candidates awaiting further integration

| Skill | Status |
| --- | --- |
| [citation-management](https://github.com/K-Dense-AI/scientific-agent-skills/blob/main/skills/citation-management/SKILL.md) | Consulted; a dedicated bibliography workflow remains pending. |
| [hypothesis-generation](https://github.com/K-Dense-AI/scientific-agent-skills/blob/main/skills/hypothesis-generation/SKILL.md) | Consulted; research-question and experiment-planning integration remains pending. |
| [learn-codebase](https://github.com/ktaletsk/learn-codebase/blob/main/SKILL.md) | Consulted for future code learning and invocation examples; its platform-specific instructions were not imported. |
| Superpowers: [systematic-debugging](https://github.com/obra/superpowers/blob/main/skills/systematic-debugging/SKILL.md) and [verification-before-completion](https://github.com/obra/superpowers/blob/main/skills/verification-before-completion/SKILL.md) | Consulted for future engineering work; neither workflow is implemented in this version. |

Add future sources and describe their actual contribution when they are consulted or adopted.

## Upstream MIT notices

The upstream license files are [literature-guide-read LICENSE](https://github.com/Liangzhen-Chen/literature-guide-read/blob/f47dbd8a5ca7d5568b60c2d8da53125257f9e2c9/LICENSE), [Scientific Agent Skills LICENSE.md](https://github.com/K-Dense-AI/scientific-agent-skills/blob/ec59a29a03d5c40f73ab40878df04860bc00e876/LICENSE.md), [Jane Street agent_skills LICENSE.md](https://github.com/janestreet/agent_skills/blob/469868f4489cbdbe178c775a0af05bb6bef63689/LICENSE.md), and [Learning Coach Skill LICENSE](https://github.com/cheng-dp/learning-coach-skill/blob/a64963bee49fee0e3aba1b5af648e545bb48bba0/LICENSE).

MIT License

For literature-guide-read:
Copyright (c) 2026 literature-guide-read contributors

For Scientific Agent Skills:
Copyright (c) 2025 K-Dense Inc.

For socratic-tutor:
Copyright (c) 2026 Jane Street Group, LLC <opensource-contacts@janestreet.com>

For learning-coach:
Copyright (c) 2026 Learning Coach Skill contributors

The following permission and warranty text is shared by those upstream licenses:

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
