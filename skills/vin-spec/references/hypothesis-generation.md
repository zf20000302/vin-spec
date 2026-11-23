# Hypothesis Generation

Develop research questions, candidate explanations, and verification
plans from literature, observations, and mathematical reasoning.

## Ground and frame the question

Read relevant project, paper, and derivation records. Keep author
claims, checked reasoning, the user's interpretation, and open
conjectures distinct. Preserve source versions, locations,
assumptions, contrary evidence, and uncertainties.

Frame the question through the target system, conditions, proposed
change, comparator, outcome, and scope where applicable. Explain what
answer would change theoretical understanding or a practical choice.

For literature-dependent claims, document the search boundary.
Treat novelty as unresolved until the available search and appraisal
justify the claim.

Use [literature-review.md](literature-review.md) for an evidence map
and search boundary, [citation-management.md](citation-management.md)
for source identity and support, and
[scientific-critical-thinking.md](scientific-critical-thinking.md)
for the reliability of premises and validation.

## Compare candidate explanations

Invite the user's explanation in their own words. Follow requests
for idea generation and add plausible rivals or missing conditions.

Include relevant alternatives such as another mechanism, resource
or tuning differences, measurement or processing effects, selected
conditions, and random variation. Candidates may coexist.

Compare evidence, research value, feasibility, and remaining gaps.
Let the user choose priorities. Use a suitable number of candidates
and discuss trade-offs without automatic quality scores or rankings.

## Derive discriminating predictions

For each candidate, identify:

- Assumptions and boundary conditions.
- The observable, measurement, and expected pattern.
- Expected patterns under plausible rivals and whether the test
  can distinguish them.
- A result that would challenge the candidate under those assumptions.
- Outcomes that would remain indeterminate.

Connect predictions to the actual derivation. A bound or conditional
result needs an argument before it can predict observed performance
or rank methods.

Match the strength of the claim to the design. Predictive improvement
alone does not establish a mechanism or causal effect.

## Match verification to the target

- **Theory:** Specify the proposition and assumptions; seek a proof
  or counterexample. Numerical examples can guide the search.
- **Implementation:** Check the mapping from formulas to code using
  hand-computable cases, known solutions, boundary cases, and
  justified numerical tolerances.
- **Method performance:** Use suitable baselines, removal or
  perturbation of key components, and condition changes to
  distinguish explanations under comparable resource and tuning
  budgets.

Use the agreed comparison structure: evaluation dimension; metric
purpose, formula, units, direction, and aggregation; and actual data,
conditions, baselines, resources, repetitions, uncertainty, and
result locations.

Choose the smallest informative next test. Specify independent test
units and any needed separation of development, tuning, and evaluation
data. Justify measurement sensitivity, repetitions, meaningful
differences, and interpretation rules. Agree unresolved thresholds
with the user using evidence or a stated practical rationale.

Record data and code versions, configurations, seeds where relevant,
and the assumptions connecting the test to the question. Keep
simulation conclusions within the tested model and conditions.
Explain the planned validation and its logic before implementation.

## Interpret results and revise transparently

Before viewing target results, record the candidates, predictions,
measures, analysis, exclusions, stopping rules, and interpretation
criteria relevant to the test.

Record what data or results have already informed the plan.
Label later data-informed ideas as exploratory. Use untouched data
or a new independent check for confirmatory testing where feasible.

Interpret whether results are consistent with, challenge, or fail
to distinguish candidates under the stated assumptions. Consider
measurement failures, uncertainty, and mixed or unknown explanations.

Preserve original plans and results. Date material changes and state
their reasons and whether the target result was already known.

Keep learning attainment separate from research evidence. Use the
existing [whiteboard-derivation standard](paper-guide.md#understanding-and-whiteboard-derivation)
for understanding a named derivation, and record scientific support
from the relevant proof, counterexample, or validation results.

## Record and resume

In the relevant project record, summarize the question, candidates,
predictions, current test stage, results and limitations, and next
verification action. Link to stable paper, derivation, and concept
records. Keep dated decisions and changes in the journal.

Resume from the latest successfully synced records, preserving source
locations, unresolved questions, prior result access, and the current
plan version. Use [learning-coach.md](learning-coach.md) when the next
verification task changes the learning route.

Follow SKILL.md's logging authorization and approval rules before
saving updates or creating any file or folder.
