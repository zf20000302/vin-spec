# Sources and Adaptations

Last updated: 2026-11-23.

This register distinguishes methods used in the current vin-spec workflows, authoring support, and candidates consulted during the wider design discussion. A listed candidate is not automatically an implemented mode or a runtime dependency.

## Confirmed design decisions

The vin-spec design discussions established the single entry, explicit and natural invocation, chapter-led reading, the user's explanations and answers, interruptible teaching detours, return points, the independent whiteboard-derivation standard, cumulative vin-log records, and approval before creating files or folders.

These decisions are recorded separately from the upstream authors' rules. Explicit authorization can delegate automatic content integration within an agreed task and confirmed arrangement. Folder structures, module roles, code placement, and reorganizations require the user's confirmation; an integration request alone does not approve them.

## Methods used in current workflows

| Source | Use in vin-spec |
| --- | --- |
| [literature-guide-read](https://github.com/Liangzhen-Chen/literature-guide-read/blob/f47dbd8a5ca7d5568b60c2d8da53125257f9e2c9/SKILL.md) and its [reading method](https://github.com/Liangzhen-Chen/literature-guide-read/blob/f47dbd8a5ca7d5568b60c2d8da53125257f9e2c9/references/method.md), Liangzhen-Chen / literature-guide-read contributors | Passage-level grounding; identifying paragraph roles, definitions, formulas, evidence, and qualifications; connecting reasoning steps; part-by-part walkthroughs and recall questions. |
| [literature-review](https://github.com/K-Dense-AI/scientific-agent-skills/blob/ec59a29a03d5c40f73ab40878df04860bc00e876/skills/literature-review/SKILL.md), K-Dense Inc., v1.11 | Scoped searches, paper maps, reasoned selection, uniform extraction, conditional metric comparisons, synthesis, and traceable claim support. Formal review coverage is reported only when actually achieved. |
| [scientific-critical-thinking](https://github.com/K-Dense-AI/scientific-agent-skills/blob/ec59a29a03d5c40f73ab40878df04860bc00e876/skills/scientific-critical-thinking/SKILL.md), K-Dense Inc., v1.5 | Claim-focused appraisal of assumptions, derivations, validation, and applicability; traceable concerns and uncertainty, with field-appropriate methods rather than a generic quality score. |
| [socratic-tutor](https://github.com/janestreet/agent_skills/blob/469868f4489cbdbe178c775a0af05bb6bef63689/socratic-tutor/SKILL.md), Jane Street Group, LLC | Focused questions about reasons, predictions, new examples, and missing conditions; evidence-based feedback and progress checks. The diagnostic and 0–5 states are adapted below. |
| [learning-coach](https://github.com/cheng-dp/learning-coach-skill/blob/a64963bee49fee0e3aba1b5af648e545bb48bba0/SKILL.md) and its [workflow references](https://github.com/cheng-dp/learning-coach-skill/tree/a64963bee49fee0e3aba1b5af648e545bb48bba0/references), cheng-dp / Learning Coach Skill contributors | Goal-based milestones, progress-informed session planning, durable checkpoints, adaptive routes, and targeted review. Adapted to the existing vin-log classification and whiteboard-derivation standard. |
| [hypothesis-generation](https://github.com/K-Dense-AI/scientific-agent-skills/blob/ec59a29a03d5c40f73ab40878df04860bc00e876/skills/hypothesis-generation/SKILL.md), K-Dense Inc., v2.4 | Evidence-bounded research questions, candidate and rival explanations, discriminating predictions, measurement and test design, uncertainty, and transparent separation of planned and exploratory work. |
| [learn-codebase](https://github.com/ktaletsk/learn-codebase/blob/06534bcba81ad14159b372cf4f636abc04d2fe66/SKILL.md), its [question patterns](https://github.com/ktaletsk/learn-codebase/blob/06534bcba81ad14159b372cf4f636abc04d2fe66/QUESTION-PATTERNS.md), and [journal template](https://github.com/ktaletsk/learn-codebase/blob/06534bcba81ad14159b372cf4f636abc04d2fe66/JOURNAL-TEMPLATE.md), Konstantin Taletskiy / ktaletsk | Code-grounded questions, prediction and execution tracing, specific feedback, and cumulative learning records. Formula-to-code mapping and vin-log integration are adapted to the user's requirements. |
| [citation-management](https://github.com/K-Dense-AI/scientific-agent-skills/blob/ec59a29a03d5c40f73ab40878df04860bc00e876/skills/citation-management/SKILL.md), K-Dense Inc., v2.3 | Source identity and version checks, metadata reconciliation, reference formatting, deduplication, and separation of bibliographic accuracy from source-to-claim support. |
| [systematic-debugging](https://github.com/obra/superpowers/blob/22f0b463e7a5e579904dd6211a520321035526f7/skills/systematic-debugging/SKILL.md), Jesse Vincent / obra | Reproduction, evidence gathering, data-flow and working-case comparison, candidate-cause testing, scoped fixes, and verified outcomes. |
| [verification-before-completion](https://github.com/obra/superpowers/blob/22f0b463e7a5e579904dd6211a520321035526f7/skills/verification-before-completion/SKILL.md), Jesse Vincent / obra | Evidence before completion claims, matching checks to the claim, inspecting results, and stating the actual verified scope. |
| SDD conceptual references: [OpenSpec workflow](https://github.com/Fission-AI/OpenSpec/blob/0c737dc1b543249b38b0f4716816fcf493d894dd/README.md) and [Spec Kit SDD overview](https://github.com/github/spec-kit/blob/a4d571229e164e440f8950cac034607bae7b7518/README.md) | Requirements, design, tasks, implementation, and iterative verification as a project workflow. The user's arrangement-confirmation gate, one-document starting format, and repository roles determine the adaptation. Framework setup remains optional and unimplemented. |
| [brainstorming](https://github.com/obra/superpowers/blob/22f0b463e7a5e579904dd6211a520321035526f7/skills/brainstorming/SKILL.md), Jesse Vincent / obra | Context-first clarification, concrete alternatives, trade-offs, and explicit separation of user decisions from proposals. |
| [writing-plans](https://github.com/obra/superpowers/blob/22f0b463e7a5e579904dd6211a520321035526f7/skills/writing-plans/SKILL.md), Jesse Vincent / obra | Requirement-linked tasks, approved file scope, interfaces, dependencies, concrete checks, and plan consistency. |
| [executing-plans](https://github.com/obra/superpowers/blob/22f0b463e7a5e579904dd6211a520321035526f7/skills/executing-plans/SKILL.md), Jesse Vincent / obra | Task-by-task execution, current source context, checkpoint evidence, recorded decisions, and resumable progress. |
| [test-driven-development](https://github.com/obra/superpowers/blob/22f0b463e7a5e579904dd6211a520321035526f7/skills/test-driven-development/SKILL.md), Jesse Vincent / obra | Focused failing behavior checks, minimal implementation, and refinement with justified expectations; applied proportionately. |
| [requesting-code-review](https://github.com/obra/superpowers/blob/22f0b463e7a5e579904dd6211a520321035526f7/skills/requesting-code-review/SKILL.md), Jesse Vincent / obra | Review context covering requirements, change range, evidence, and located actionable findings. |
| [receiving-code-review](https://github.com/obra/superpowers/blob/22f0b463e7a5e579904dd6211a520321035526f7/skills/receiving-code-review/SKILL.md), Jesse Vincent / obra | Understanding and checking feedback before changes, evidence-based disagreement, and verified corrections. |
| [using-git-worktrees](https://github.com/obra/superpowers/blob/22f0b463e7a5e579904dd6211a520321035526f7/skills/using-git-worktrees/SKILL.md), Jesse Vincent / obra | Detecting existing isolation, user-approved workspace arrangement, native-tool preference, and baseline context. |
| [finishing-a-development-branch](https://github.com/obra/superpowers/blob/22f0b463e7a5e579904dd6211a520321035526f7/skills/finishing-a-development-branch/SKILL.md), Jesse Vincent / obra | Verified completion, explicit delivery choices, integrated-state checks, handoff, and preservation of user work. |

Reviewed snapshots:
- literature-guide-read: f47dbd8a5ca7d5568b60c2d8da53125257f9e2c9.
- Scientific Agent Skills: ec59a29a03d5c40f73ab40878df04860bc00e876.
- Jane Street agent_skills: 469868f4489cbdbe178c775a0af05bb6bef63689.
- Learning Coach Skill: a64963bee49fee0e3aba1b5af648e545bb48bba0.
- learn-codebase: 06534bcba81ad14159b372cf4f636abc04d2fe66.
- Superpowers, adapted engineering workflows: 22f0b463e7a5e579904dd6211a520321035526f7.
- OpenSpec, consulted workflow overview: 0c737dc1b543249b38b0f4716816fcf493d894dd.
- Spec Kit, consulted SDD overview: a4d571229e164e440f8950cac034607bae7b7518.

The adapted workflows use conversational guidance, precise source locations, user-directed detours, and vin-log checkpoints. Upstream generation pipelines, scripts, assets, and fixed quotas are not bundled. Detailed mathematical checking also reflects the user's requirements and the design discussion.

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

## Hypothesis-generation adaptation

- Ground questions in traceable literature, observations, assumptions,
  and derivations, with a documented search boundary for
  literature-dependent claims.
- Invite the user's explanation, expand plausible rivals, and compare
  their predictions. The user chooses priorities through evidence
  and trade-offs.
- Connect questions to proof or counterexample, implementation checks,
  or method-performance tests as appropriate.
- Reuse the agreed comparison-metric structure and cumulative vin-log
  conventions.
- Record predictions and interpretation criteria before target results,
  distinguish exploratory changes, and preserve dated plans and results.
- Keep learning attainment under the existing whiteboard standard
  separate from scientific support.
- The proof/implementation/performance distinction, user-led learning,
  and vin-log integration reflect user-confirmed design decisions.
  Upstream scripts and full JSON/CSV schemas are not imported.

Reviewed the candidate-lifecycle and human-review guidance,
experimental-design and preregistration references, and the
hypothesis-record and prediction/rival templates at the Scientific
Agent Skills snapshot listed above.

The existing Scientific Agent Skills MIT notice also covers this
adaptation of hypothesis-generation.

## Learn-codebase adaptation

- Start from the user's goal and a relevant execution path. Ground
  data-flow and behavior explanations in the actual code and version.
- Add formula-to-code mapping, assumptions, dimensions, update order,
  numerical choices, and small-case checks as user-confirmed extensions.
- Reuse paper-guide's adaptive questions, direct explanations, feedback,
  detours, and whiteboard standard. Record code understanding through
  observed explanations, traces, and predictions.
- Use the existing vin-log project, paper, derivation, concept, and
  journal conventions, with precise code positions and return points.
- Connect guided exploration to implementation or fixes when requested,
  within the user's authorized scope.
- The upstream fixed hint ladder, success-percentage target, traffic-light
  mastery system, timed save and review schedules, Claude-specific
  settings, and separate journal path are not imported.
- Preserve both explicit and natural invocation through vin-spec.

## Literature, appraisal, and citation adaptation

- Extend the previously agreed selection, comparison, metric, and
  citation-checking methods into connected workflows.
- Match search and reporting to the task. Distinguish an exploratory
  paper map from the coverage and procedures of a formal review.
- Use the user's three-layer comparison structure and source anchors.
  Keep bibliographic identity, claim support, scientific reliability,
  and personal understanding as separate judgments.
- Assess mathematical reasoning and applicability using the user's
  requirements. Domain appraisal frameworks are used only where they fit.
- Preserve stable paper and version identities, investigate missing
  metadata against primary sources, and format requested references
  without inventing fields.
- Use the existing vin-log conventions and delegated authorization.
  External search services, bibliography scripts, rendering pipelines,
  default figures, and mandatory schema or tool dependencies are not imported.

## Debugging and verification adaptation

- Use reproduction, targeted evidence, competing explanations, scoped
  correction, and checks of the original symptom.
- Preserve uncertainty for intermittent, environmental, and unresolved
  failures. Reassess repeated unsuccessful attempts without a fixed
  attempt-count gate.
- Select meaningful checks proportionate to the change. Add tests for
  important behavior or genuine verification gaps.
- Check evidence against the final changed state and report its limits.
  Re-run affected checks when changes or unresolved concerns justify it.
- Reuse valid checks and the existing record system. Upstream blanket
  testing, repeated full-suite requirements, rhetoric, fixed stop gates,
  and mandatory delegation are not imported.

## SDD adaptation

- Start from one complete useful workflow and concrete acceptance examples.
- Begin a small project with requirements/acceptance, design/arrangement,
  and tasks/verification as sections in one project document.
- Present an algorithm proposal with the adoption recommendation and
  before implementation, including its architecture diagram, subsystem
  responsibilities, inputs, outputs, reasoning, and planned checks.
  This requirement is an explicit user contribution.
- Confirm exact folder and file placement, module roles, interfaces,
  dependencies, and reasons with the user before creating or reorganizing.
- Implement within the confirmed arrangement and reuse the existing
  code-reading, debugging, verification, and learning workflows as relevant.
- Keep project specifications authoritative in the actual project repository;
  keep personal understanding and linked progress in vin-log.
- The above decisions are user-confirmed. OpenSpec and Spec Kit are
  conceptual references, with no generated project layout, commands,
  configuration, or runtime dependency imported.

## Engineering lifecycle adaptation

- Incorporate the eight methods as stages in the existing SDD reference
  and entry, preserving the confirmed file arrangement.
- Reuse known context and confirmed choices. Ask only consequential
  unanswered questions and compare actual viable approaches.
- Use the existing project document for plans, design, task state, and
  evidence. Link personal progress from vin-log.
- Apply test-first cycles to important behavior and meaningful regressions,
  with independent expected outcomes and justified numerical tolerances.
- Ground review in requirements, actual changes, and evidence; verify
  feedback before acting and keep findings proportional to their effects.
- Create worktrees only under the user's explicit request or approval,
  with confirmed placement. Reuse authorized delivery instructions.
- Upstream default artifact paths, visual-companion setup, scripts and
  ledger directories, compulsory test gates, per-task commits, model
  choices, mandatory reviewer agents, external posting, and automatic
  workspace or branch cleanup are not imported.

## Authoring and preparation support

- **skill-creator**, supplied with Codex: consulted for scope, concise instructions, and supporting references.
- **openai-docs**, supplied with Codex: consulted to verify discovery, invocation, and loading behavior against [OpenAI's Build skills documentation](https://learn.chatgpt.com/docs/build-skills).
- **computer-use**: preparation tooling for reading the user-provided shared discussion; no computer-control procedure is part of this skill.
- Locally installed **bmad-deep-recon** and **bmad-review** were inspected for applicability; their workflows were not adopted.

Local authoring and preparation revisions are not pinned in this register. These skills are not required runtime dependencies.

## Consulted candidates awaiting further integration

| Skill | Status |
| --- | --- |
| [OpenSpec](https://github.com/Fission-AI/OpenSpec/blob/0c737dc1b543249b38b0f4716816fcf493d894dd/README.md) | Its conceptual workflow informs the SDD adaptation above; OpenSpec-specific setup, generated layout, and execution remain pending. |
| [Spec Kit](https://github.com/github/spec-kit/blob/a4d571229e164e440f8950cac034607bae7b7518/README.md) | Its conceptual workflow informs the SDD adaptation above; Spec Kit-specific setup, generated layout, and execution remain pending. |

Add future sources and describe their actual contribution when they are consulted or adopted.

## Upstream MIT notices

The upstream license files are [literature-guide-read LICENSE](https://github.com/Liangzhen-Chen/literature-guide-read/blob/f47dbd8a5ca7d5568b60c2d8da53125257f9e2c9/LICENSE), [Scientific Agent Skills LICENSE.md](https://github.com/K-Dense-AI/scientific-agent-skills/blob/ec59a29a03d5c40f73ab40878df04860bc00e876/LICENSE.md), [Jane Street agent_skills LICENSE.md](https://github.com/janestreet/agent_skills/blob/469868f4489cbdbe178c775a0af05bb6bef63689/LICENSE.md), [Learning Coach Skill LICENSE](https://github.com/cheng-dp/learning-coach-skill/blob/a64963bee49fee0e3aba1b5af648e545bb48bba0/LICENSE), [learn-codebase LICENSE](https://github.com/ktaletsk/learn-codebase/blob/06534bcba81ad14159b372cf4f636abc04d2fe66/LICENSE), [Superpowers LICENSE](https://github.com/obra/superpowers/blob/22f0b463e7a5e579904dd6211a520321035526f7/LICENSE), [OpenSpec LICENSE](https://github.com/Fission-AI/OpenSpec/blob/0c737dc1b543249b38b0f4716816fcf493d894dd/LICENSE), and [Spec Kit LICENSE](https://github.com/github/spec-kit/blob/a4d571229e164e440f8950cac034607bae7b7518/LICENSE).

MIT License

For literature-guide-read:
Copyright (c) 2026 literature-guide-read contributors

For Scientific Agent Skills:
Copyright (c) 2025 K-Dense Inc.

For socratic-tutor:
Copyright (c) 2026 Jane Street Group, LLC <opensource-contacts@janestreet.com>

For learning-coach:
Copyright (c) 2026 Learning Coach Skill contributors

For learn-codebase:
Copyright (c) 2026 Konstantin Taletskiy

For the adapted Superpowers skills:
Copyright (c) 2025 Jesse Vincent

For OpenSpec:
Copyright (c) 2025 FISSION AI INC

For Spec Kit:
Copyright GitHub, Inc.

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
