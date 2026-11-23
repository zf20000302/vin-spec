# Learn Codebase

Build understanding of an implementation through guided code reading,
execution tracing, and connections to mathematical reasoning.

## Set the direction

Use the user's goal and relevant existing records. Identify the
repository, branch or commit, and relevant local changes. Clarify
only missing information that affects the session.

Choose a useful entry point and execution path tied to the current
question. Explain the roles of the nearby modules as they become
relevant. Work through manageable pieces of reasoning.

## Follow an execution path

Trace where inputs originate, their types, shapes, units and ranges,
and how they change through calls, transformations, state updates,
and outputs. Examine callers, consumers, control flow, side effects,
and relevant failure paths.

Anchor interpretations to actual files, functions, expressions, and
source versions. Use suitable small inputs or execution observations
to check the trace. Mark inferred behavior and unresolved questions.
Use applicable official documentation to check language and library
behavior when needed.

Support claims about design intent with documentation or history.
Keep plausible explanations separate from recorded reasons.

## Connect mathematics and implementation

For a selected formula or derivation, connect:

- Paper or derivation locations to implementation locations.
- Symbols to variables, shapes, units, indices, and coordinate frames
  where relevant.
- Assumptions to configuration, preconditions, checks, and operating
  conditions.
- Derivation steps to functions, operations, update order, and state.
- Theoretical expressions to discretization, approximations, clipping,
  numerical precision, or solver choices in the implementation.
- Results to returned values, recorded outputs, and evaluation metrics.

Use hand-computable cases, known solutions, or boundary cases to check
the correspondence. Identify whether an apparent difference is an
equivalent transformation, an approximation, an implementation issue,
or an unresolved reasoning step.

Use the existing [whiteboard-derivation standard](paper-guide.md#understanding-and-whiteboard-derivation)
for a named mathematical target. Record code understanding through
what the user explains, traces, or predicts and the evidence checked.

## Questions, feedback, and detours

Use the relevant [diagnostic and feedback rules](paper-guide.md).
Ask one focused question and wait for the user's answer. Invite useful
predictions before checking behavior, and ask the user to explain the
trace in their own words.

Identify correct reasoning and the specific gap. Offer a hint or direct
explanation as needed. Honor requests to explain directly or let the
user try again. Teach unfamiliar prerequisites before requiring their
application.

During a detour, preserve the source version, file, function, interrupted
expression or step, question, and return point. Reconnect the explanation
to that point before continuing.

## Move from understanding to changes

During guided exploration, inspect and trace the code. When the user
requests implementation or a fix, explain the intended change and
proceed within the authorized scope. Apply the relevant verification,
logging, and file-approval rules.

Use [hypothesis-generation.md](hypothesis-generation.md) when a claim
about method performance or mechanism needs a discriminating test.
Use [learning-coach.md](learning-coach.md) when the work changes the
learning route.

## Record and resume

Follow the vin-log conventions in SKILL.md:

- In the project README, keep repository and version context, the
  learning goal, current execution path, formula-to-code links, the
  user's explanation, unresolved questions, and next action.
- In stable mathematical records, keep derivations and assessment
  evidence. Reuse paper notes for source passages and concept notes
  for language, algorithm, and numerical ideas.
- In the dated journal, keep a short activity and decision record
  with links.

Prepare updates at meaningful checkpoints or pauses. Preserve the
exact reading position and any open detour. Save under existing
logging authorization or the user's request; apply SKILL.md's rule
before creating any new file or folder.

Resume from the latest successfully synced relevant records. Restore
the goal, source position, and remaining gap. If the implementation
changed, check the relevant code before reusing the previous trace.
