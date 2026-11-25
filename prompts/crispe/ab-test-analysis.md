# A/B test analysis

**When to use:** a test has run and you need a ship / extend / stop call backed by whether the result is real, not just which bar is taller.
**Framework:** CRISPE
**PM job:** Data

## The prompt

```
C, Capacity and Context
Analyse this A/B test. Hypothesis: [what we expected]. Variant: [what changed]. Primary
metric: [metric]. Guardrails: [metrics that must not degrade]. Duration and split:
[days, traffic split]. Here is the data:
[paste or attach the numbers]

R, Role
Act as an experimentation analyst with statistical rigour. A winning primary metric with
a wrecked guardrail is not a win, and an underpowered test proves nothing.

I, Insight and Instruction
1. Validate the setup: is the sample large enough for the expected effect, did it run at
   least one to two full business cycles, any sign of sample ratio mismatch, any novelty
   effect still washing out?
2. Calculate conversion for control and variant, relative lift, p-value (two-tailed), and
   the 95% confidence interval. Flag if p is below 0.05, and whether the lift is
   practically meaningful, not just statistically significant.
3. Check the guardrail metrics for degradation.
4. Give the recommendation: ship / extend / stop / investigate, with the reasoning.

S, Specification
A results table (metric, control, variant, lift, p-value, significant?), the guardrail
check, and the recommendation with next steps. If I give raw data, write the calculation.

P, Personality and Parameters
Do not declare a winner on an underpowered or too-short test. Distinguish statistical from
practical significance. If the data cannot support a conclusion, say "extend" and why,
rather than forcing a call. British English.

E, Example
"Variant lifted signups 4% (p=0.03), but time-on-task guardrail degraded 11%. Do not ship
yet. Investigate whether the faster signup is pushing work downstream."
```
