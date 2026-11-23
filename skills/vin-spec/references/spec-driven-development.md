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

## Plan and implement within the confirmed scope

Break work into small tasks tied to behavior and acceptance criteria.
For each task, identify the approved paths, purpose, dependencies,
implementation steps, and relevant verification.

Proceed within the confirmed arrangement and task authorization.
Explain important logic and how changes serve the project.
Use [learn-codebase.md](learn-codebase.md) for guided implementation
understanding and mathematical connections.

When a failure needs investigation, use
[systematic-debugging.md](systematic-debugging.md).
Use [hypothesis-generation.md](hypothesis-generation.md) when uncertain
scientific or performance claims require a discriminating test.

## Verify and keep the project coherent

Use [verification-before-completion.md](verification-before-completion.md)
to check delivered behavior against acceptance criteria and report
the actual verified scope.

Keep requirements, design, tasks, code, and checks aligned.
When new information changes the intended behavior or design, record
what changed and why. Preserve decisions and unresolved questions.

## Separate shared methods from project records

- vin-spec holds reusable collaboration methods.
- The actual project repository holds the authoritative requirements,
  design, task details, implementation, and verification evidence.
- vin-log holds personal understanding, decision reasons, and progress
  summaries linked to project documents and versions.

Use [learning-coach.md](learning-coach.md) when a prerequisite learning
route is needed. Reuse existing knowledge and journal records under
SKILL.md's logging authorization.

## Select tooling after the method and arrangement

Compare OpenSpec, Spec Kit, or a project-specific document workflow
against the user's confirmed needs, document volume, and change process.

Any generated files and tool-specific arrangement must be included
in the proposal the user confirms before setup or initialization.
