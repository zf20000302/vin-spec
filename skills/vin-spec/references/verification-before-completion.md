# Verification Before Completion

Support completion claims with evidence appropriate to the work and
the exact scope being claimed.

## Define what needs verification

Identify the requested behavior or deliverable, what changed, and which
checks can establish it.

- **Software:** Check relevant behavior, the original failing case,
  and affected regressions. Build, lint, or run broader tests when
  they bear on the change.
- **Documents and skills:** Check required content, structure, links,
  source fidelity, and the intended file scope.
- **Research results:** Check the reported computation or observation,
  inputs, versions, conditions, and limits of the inference.
- **Remote updates:** Read back the saved content and inspect the
  resulting change scope when applicable.

Use existing meaningful checks where possible. Add tests when they
protect behavior or resolve a real uncertainty. Match effort to the
change rather than imposing a universal test suite.

## Run and inspect

Execute the relevant checks and inspect their output and status.
Record commands or methods, source and environment context, outcomes,
failures, and important limitations.

Check evidence against the actual requirement. A passing formatter,
build, or test supports what it checks; assess remaining requirements
separately.

Evidence must apply to the final changed state. Rerun affected checks
after new changes, input or environment changes, failures, or unresolved
concerns. Once appropriate checks pass, continue toward completion.

If a required check cannot run, state the actual verified scope and
what remains unverified. Do not convert a proposed check into a result.

## Report and keep records

State what changed, why, how it was checked, and any material remaining
gap. Distinguish implementation, verification, remote publication, and
actual runtime use when those are separate outcomes.

Learning attainment follows [paper-guide.md](paper-guide.md) and its
evidence rules. Computational success does not establish the user's
independent understanding.

Keep relevant evidence and next steps in the existing project or
knowledge record, with a short linked journal entry when authorized.
Follow SKILL.md's logging and file-authorization rules.
