# Spec-Driven Development

Develop a new project or a scoped project version through clear
behavior, a confirmed arrangement, actionable tasks, and verification.

## Start with one useful flow

Use the user's context to clarify the intended user, problem, first
complete workflow, inputs, outputs, constraints, and desired outcome.
Ask only for missing information that affects the work.

Describe normal and exceptional behavior with concrete acceptance
examples. Keep unresolved assumptions visible and distinguish the
first useful version from possible later work.

Use an example for discussion when no actual project has been selected.

### Clarify goals and compare approaches

Read the user's context, relevant code, and prior decisions before
asking questions. Ask only when an answer would change the work and
the available context does not already answer it.

When a material design choice is open, compare viable approaches in
concrete terms: behavior, fit to the goal, dependencies, cost, risks,
and what each gives up. Recommend a direction with reasons and let
the user decide choices they have reserved.

Preserve agreed choices and distinguish the user's requirements from
Codex proposals. Scale the design detail to the task. Reuse the project
document and its confirmed location. Algorithm adoption still follows
the proposal requirements below.

## Keep three kinds of project information

For a small project, begin with one project document containing:

1. **Requirements and acceptance:** Goals, scope, behavior, constraints,
   examples, and completion criteria.
2. **Design and arrangement:** Algorithm proposals, module roles,
   interfaces, data flow, dependencies, and the confirmed folder
   and code placement.
3. **Tasks and verification:** Small steps, affected paths, prerequisites,
   expected checks, outcomes, and remaining work.

Confirm the document's filename and location with the user.
Propose any later split or reorganization before changing it.

## Algorithm proposal

When recommending an algorithm for actual adoption, include a proposal
with the recommendation. Present it before implementing the algorithm
or a material change to its architecture.

The proposal must include:

- The problem, intended role, and reason for recommending the algorithm.
- An architecture diagram showing the real subsystems, their inputs
  and outputs, data and state flow, and feedback where applicable.
- A subsystem explanation or table: responsibility, inputs, outputs,
  main calculation or equations, and important assumptions or limits.
- The relevant trade-offs, unresolved questions, and a concise plan
  for checking correctness and the claimed benefit.

Use the actual logical decomposition and scale detail to the algorithm.
Connect mathematical reasoning to each relevant block when needed.

Prefer an inline diagram, such as Mermaid, and a subsystem table in
the conversation or an already approved design document. A separate
proposal or diagram file requires confirmation of its filename and path.

Let the user review the proposal and establish the algorithm choice
before proceeding with an unapproved selection or implementation.
Reuse relevant approval for an unchanged proposal. Material changes
to the algorithm or architecture return to proposal review.

Algorithm approval and confirmation of the folder and code arrangement
are separate decisions. Record both where applicable.

## Confirm the arrangement before creating it

Present the proposed directory tree and exact file paths. Explain each
file or module's responsibility, inputs and outputs, dependencies,
relationship to the rest of the project, and reason for its placement.
Include data shapes, units, or mathematical assumptions where relevant.

Wait for the user's confirmation before creating folders or files or
changing code organization. Record the arrangement actually approved.

Approval of the workflow or automatic content integration does not
approve unspecified file locations. Moves, renames, splits, merges,
or other arrangement changes return to this confirmation step.
Continue independent authorized work while those changes await approval.

## Isolate work when needed

Inspect the current checkout, branch state, relevant local changes,
and any existing suitable worktree before proposing a new workspace.

Create a new worktree only when the user requests or explicitly approves
it. Include the intended path, branch or base, purpose, and integration
plan in the arrangement proposal. Reuse a suitable existing workspace.

Prefer available native workspace tools; use a Git fallback only when
appropriate tools are unavailable and the arrangement is confirmed.
Run relevant setup and baseline checks, and record existing failures
without treating them as regressions from the new work.

Preserve local and untracked work. Cleanup and branch deletion follow
explicit user authorization and host ownership rules.

## Plan and implement within the confirmed scope

### Write an actionable plan

Break work into small, coherent tasks tied to requirements and acceptance
criteria. Identify each task's approved paths, purpose, dependencies,
interfaces, important fixed values, implementation steps, and the checks
and observations that establish completion.

Check coverage of requirements and consistency between producer and
consumer interfaces. Keep the plan focused on decisions needed to
implement correctly. Explain uncertainty instead of filling gaps with
unexamined assumptions.

Use the existing project document's tasks and verification section.
A plan that needs new paths or a changed arrangement returns to the
user's confirmation step before that part is implemented.

### Test behavior before implementation

For important new behavior and meaningful regressions where tests add
confidence, use a focused test-first cycle:

1. Express an observable requirement or failing case.
2. Run the check and establish that it fails for the intended reason.
3. Implement the smallest coherent correction or behavior.
4. Run the relevant checks and refine the code while preserving behavior.

Test actual behavior with independently justified expected results.
For numerical algorithms, use hand-computable or known solutions,
boundary cases, and tolerances justified by the problem.

Preserve existing code and user work. Choose useful checks for the
actual change; reversible prose or low-impact changes do not require
a new test suite. Obtain approval for new test-file paths or arrangement
changes as required above.

### Execute with checkpoints

Read the current requirements, design, task state, and source version.
Resume at the next unfinished task whose dependencies are satisfied.

Implement within the confirmed arrangement and task authorization.
Compare actual results with the planned checks. At meaningful checkpoints,
record what changed, evidence, decisions and reasons, remaining gaps,
and the next task.

If a plan conflicts with the requirements, make a scoped correction
that preserves the agreed intent and record why. Return choices that
change the requested behavior, algorithm, or arrangement to the user.
Continue independent authorized work while those decisions are pending.

Explain important logic and use
[learn-codebase.md](learn-codebase.md) for guided code understanding.
Use [systematic-debugging.md](systematic-debugging.md) for failures and
[hypothesis-generation.md](hypothesis-generation.md) when scientific
or performance claims need discriminating tests.

Additional agents or parallel work require explicit user authorization;
they are not an automatic consequence of planning or review.

## Request and handle review

Use review when requested or at an agreed engineering checkpoint.
Prepare the intended behavior and constraints, relevant specification
and plan, exact change range or source versions, verification evidence,
and unresolved questions.

Assess the actual change against requirements, interfaces, failure
cases, and affected behavior. Findings identify the source location,
evidence, practical consequence, uncertainty, and suggested next check.
Distinguish demonstrated defects, open questions, and preferences.

Use authorized review resources. Keep findings in the requested
conversation or artifact; external posting and agent delegation need
the user's authorization.

Read feedback fully, restate the technical issue, and check it against
the current implementation and project decisions before changing code.
Clarify consequential ambiguity. Prioritize supported issues by impact,
correct and verify them, and explain any disagreement with evidence.
Record remaining or deferred findings and their consequences.

## Verify and keep the project coherent

Use [verification-before-completion.md](verification-before-completion.md)
to check delivered behavior against acceptance criteria and report
the actual verified scope.

Keep requirements, design, tasks, code, and checks aligned.
When new information changes the intended behavior or design, record
what changed and why. Preserve decisions and unresolved questions.

## Finish and deliver

Check the final state against requirements and acceptance criteria,
including relevant test, build, review, and unresolved-issue evidence.
State the exact completed and unverified scope.

Identify the actual branch or workspace, integration target, and
authorized delivery method. If the method is already specified,
carry it out within that authorization. Otherwise present concrete
options, such as keeping the branch, preparing a PR, or merging to
the confirmed target, for the user's decision.

Verify the resulting remote or integrated state when applicable.
Report the delivery location, relevant versions, checks, remaining
work, and how to resume.

Preserve branches, worktrees, and local work until cleanup is explicitly
authorized. Use host-managed lifecycle tools where applicable and verify
the exact target before any removal. An implementation-complete report
does not authorize discarding work.

## Separate shared methods from project records

- vin-spec holds reusable collaboration methods.
- The actual project repository holds the authoritative requirements,
  design, task details, implementation, and verification evidence.
- vin-log holds personal understanding, decision reasons, and progress
  summaries linked to project documents and versions.

Keep the detailed task state and verification evidence authoritative in
the project document. In vin-log, summarize personal understanding,
decision reasons, blockers, and next actions with links and dates.

Use [learning-coach.md](learning-coach.md) when a prerequisite learning
route is needed. Reuse existing knowledge and journal records under
SKILL.md's logging authorization.

## Select tooling after the method and arrangement

Compare OpenSpec, Spec Kit, or a project-specific document workflow
against the user's confirmed needs, document volume, and change process.

Any generated files and tool-specific arrangement must be included
in the proposal the user confirms before setup or initialization.
