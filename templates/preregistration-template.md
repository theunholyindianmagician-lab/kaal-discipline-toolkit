# Pre-Registration Template

**Use this template** BEFORE any empirical test, simulation, hardware run, or data-gathering operation. Commit the pre-registration FIRST. Then run the test. Then publish the result regardless of outcome.

---

## Pre-Registration: `<short-test-name>`

### Date sealed (BEFORE submission)
*(YYYY-MM-DD HH:MM · commit hash before any test execution)*

### Hash commit
Commit this file BEFORE running the test. The git-commit SHA is the pre-registration anchor.

### Authority
*(operator name + project)*

### Lineage
*(any prior pre-registrations that triggered this one · honest history)*

---

## ◈ The claim under test

> *(state the claim in one paragraph)*

## ◈ Prediction

| Parameter | Predicted value | Confidence interval |
|---|---|---|
| *(metric 1)* | *(prediction)* | *(CI bounds)* |
| *(metric 2)* | *(prediction)* | *(CI bounds)* |

## ◈ Falsification criterion

The claim is FALSIFIED if:
- *(specific observation that would refute it)*
- *(another specific observation)*

**The criterion must be observable BEFORE running the test.** If you cannot state what would falsify the claim, the claim is not pre-registerable.

## ◈ Sample-size pre-specification

| Parameter | Value | Statistical justification |
|---|---|---|
| Sample size (N) | *(value)* | *(why this N is appropriate for the prediction)* |
| Threshold (deviation tolerance) | *(value)* | *(sample-size-aware — see HALAHALA #37 if applicable)* |
| Multiple comparisons correction | *(method)* | *(Bonferroni · Benjamini-Hochberg · etc.)* |

**Common pitfall:** setting a tight threshold (e.g. 5% deviation) that the sample size cannot statistically support. Avoid by:
- 100k+ samples AND p > 0.001 → 10% threshold OK
- 10k samples AND p in [10⁻⁴, 5×10⁻³] → 30% threshold (essentially "is anything 2σ?")
- p < 10⁻⁴ AND 10k samples → NOT TESTABLE at this sample size

## ◈ Honesty commitments (non-negotiable)

- [ ] Result will be reported publicly regardless of outcome
- [ ] HALAHALA entry will be filed at source if criterion fails
- [ ] No post-hoc parameter-tuning
- [ ] All raw data (samples, observations, intermediate values) will be published — including outliers
- [ ] Any deviation from this pre-registration will be noted explicitly in the result-report

## ◈ Pass criterion

The claim is SUPPORTED if:
- *(specific observation OR combination of observations)*
- AND the deviation is within the pre-specified threshold
- AND no significant artifact / outlier dominates the result

## ◈ Possible outcomes (pre-stated)

### Outcome A — claim supported
- Action: *(what follows from confirmation)*
- Publication: *(target venue / next-step paper)*
- Halahala: no new entry

### Outcome B — claim falsified
- Action: file HALAHALA entry pattern-tagged with the error type
- Investigation: *(what would explain the failure)*
- Publication: still published — a negative result with structured reasoning is publishable

### Outcome C — indeterminate
- Action: re-test with larger sample / tighter conditions
- Resource cost: *(what additional resource is needed)*

---

## ◈ Status checklist (update as test progresses)

- [ ] Pre-registration committed to repo (THIS file)
- [ ] Hash recorded: *(SHA after commit)*
- [ ] Test environment verified (versions / dependencies / hardware)
- [ ] Sample / data collected
- [ ] Analysis run per pre-specified protocol
- [ ] Result reported (PASS / FAIL / INDETERMINATE)
- [ ] HALAHALA filed if applicable
- [ ] Result-report committed (separate commit, citing this file's SHA)

---

## Authoritative references

- `REAL-MATHEMATICS/T-MAX-PREREGISTRATION-2026-05-18.md` (KAAL framework Round-1 example)
- `REAL-MATHEMATICS/T-MAX-ROUND2-PREREGISTRATION-2026-05-18.md` (Round-2 with HALAHALA-corrections)
- `REAL-MATHEMATICS/BIPOLAR-PREREGISTRATION-2026-05-18.md` (bipolar hardware test pre-reg)
- Brian Nosek · Center for Open Science · https://osf.io
