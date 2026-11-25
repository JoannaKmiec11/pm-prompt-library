# Cohort analysis

**When to use:** you want to know whether retention is actually improving over time, or whether a headline number is hiding a leaky bucket.
**Framework:** CRISPE
**PM job:** Data

## The prompt

```
C, Capacity and Context
Analyse retention by cohort for [product]. A cohort is [how you group, e.g. by signup
month]. Retention means [the action that counts as retained, e.g. logged in that week].
Here is the data:
[paste or attach the cohort table]

R, Role
Act as a product analyst who reads cohort curves. You know a flat total user count can
hide strong acquisition masking strong churn, and that the shape of the curve matters
more than any single week.

I, Insight and Instruction
1. Describe the retention curve: where it drops fastest, and whether it flattens (a
   stable core) or keeps declining (no product-market fit yet).
2. Compare cohorts over time: is retention improving for newer cohorts, or are we just
   acquiring more to replace churn?
3. Identify the make-or-break moment: the step where most users are lost.
4. Name the one intervention most likely to bend the curve, and what to measure to know.

S, Specification
The curve read, the cohort-over-cohort comparison, the critical drop-off, and the one
intervention.

P, Personality and Parameters
Do not celebrate a growing total if newer cohorts retain worse. Say when the data window
is too short to judge flattening. Do not invent cohorts the data does not contain. British
English.

E, Example
"Newer cohorts retain worse, not better. Total users are up only because marketing spend
is up. The product is a leaky bucket and we are paying to keep it full."
```
