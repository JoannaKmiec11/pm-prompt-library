# Opportunity solution tree

**When to use:** you have a single outcome to move and a pile of research, and you want the opportunity space mapped before anyone commits to a solution.
**Framework:** CRISPE
**PM job:** Discovery

## The prompt

```
C, Capacity and Context
I am running discovery on [product or area]. The outcome I am trying to move is
[single measurable outcome, e.g. "increase 7-day retention from 28% to 40%"]. Here is
the research I have so far:
[paste interviews, analytics, feedback]

R, Role
Act as a discovery coach working in the style of Teresa Torres' Continuous Discovery
Habits. You keep teams out of the solution space until the opportunity space is mapped.

I, Insight and Instruction
Build an opportunity solution tree with four levels:
1. Outcome: confirm the single measurable outcome at the top.
2. Opportunities: 3 to 7 customer needs or pains from the research, framed from the
   customer's view ("I struggle to..."). These are problems, not features.
3. Prioritise the opportunities using Opportunity Score = Importance x (1 - Satisfaction),
   both normalised to 0 to 1. Focus on the top 2 or 3.
4. Solutions: at least 3 per prioritised opportunity. Do not stop at the first idea.
5. Experiments: for the most promising solutions, 1 to 2 fast, cheap tests. Each with a
   hypothesis, method, metric and success threshold.

S, Specification
Present the tree as a clear hierarchy, outcome down to experiments. Keep opportunities
phrased in the customer's words.

P, Personality and Parameters
One outcome only. Opportunities, not features. At least three solutions before choosing.
If the research does not support an opportunity, do not invent one, say the research is
thin there. British English.

E, Example
Opportunity: "I never know if my changes actually worked." Solution options: in-product
result banner / weekly email digest / a dashboard. Experiment: fake-door the email digest,
success = 20% click through.
```
