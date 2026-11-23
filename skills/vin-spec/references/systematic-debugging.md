# Systematic Debugging

Investigate unexpected behavior, test a causal explanation, make a
scoped correction, and verify the reported outcome.

## Establish the failure

Record expected and actual behavior, relevant inputs, reproduction
steps, source version, environment and configuration, error messages,
and affected scope. Read the complete relevant error or trace.

Use the smallest useful reproduction. For intermittent failures,
record frequency, timing, conditions, and what evidence is still needed.

## Investigate before changing behavior

Inspect recent changes, working comparisons, dependencies, and the
relevant execution path. Trace incorrect values or state back to their
origin and across component boundaries.

Gather targeted evidence that can distinguish causes. State a specific
candidate cause, why the evidence suggests it, and what observation
would challenge it.

Use [learn-codebase.md](learn-codebase.md) when the user wants to learn
the implementation or needs a guided trace.

## Test and correct

Test one explanatory change at a time where practical. Keep observations
and rejected explanations so unsuccessful attempts inform the next step.

Once a cause is supported, explain the intended correction and implement
within the authorized scope. Keep unrelated cleanup separate.

For meaningful behavior fixes, capture the original failure with a
reproduction or regression check where feasible, then rerun after the
fix. Add tests when they protect important behavior; choose checks
proportionate to the change.

If attempts keep failing or reveal broader coupling, reassess the
assumptions and design before stacking more speculative fixes.
State precisely which missing input or environment access blocks a
necessary check, while continuing independent useful work.

## Verify and explain

Use [verification-before-completion.md](verification-before-completion.md)
before reporting the fix complete. Check the original symptom and
relevant affected behavior.

Report the supported cause, change, verification evidence, remaining
uncertainty, and next action. An environmental or external explanation
needs evidence and an explicit scope of what was established.

## Record and resume

Keep the issue, reproduction, evidence, candidate causes, correction,
checks, and remaining work in the relevant project record. Put reusable
lessons in concept notes and short dated activity in the journal.

Resume from the latest successfully synced record and check the current
code and environment before relying on an earlier diagnosis.
Follow SKILL.md's logging and file-authorization rules.
