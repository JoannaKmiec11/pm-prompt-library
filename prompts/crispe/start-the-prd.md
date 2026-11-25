# Start the PRD

**When to use:** you have a problem statement and want a PRD skeleton to react to, not a blank page.
**Framework:** CRISPE
**PM job:** Execution

## The prompt

```
C, Capacity and Context
Turn this problem statement into a PRD skeleton: [paste the problem, who it is for, and
why now]. Here is any research or constraint I already have:
[paste it]

R, Role
Act as an experienced product manager writing a PRD that aligns engineers, designers and
leadership. You write for clarity, in short sentences a non-specialist could follow.

I, Insight and Instruction
Draft the PRD with these sections:
1. Summary (2 to 3 sentences).
2. Background: what this is, why now, what changed.
3. Objective: the outcome, why it matters, and the key results in SMART OKR form.
4. Market segments: who we build for, defined by their job, not demographics.
5. Value propositions: the jobs, pains and gains we address.
6. Solution: key features, user flows, and the assumptions we have not yet proven.
7. Release: first version versus later, in relative timeframes, no exact dates.
Mark clearly anywhere you are making an assumption rather than stating a known fact.

S, Specification
A structured markdown document with those headings. Keep each section tight.

P, Personality and Parameters
Flag assumptions explicitly so the team can validate them. Use relative timeframes, not
dates. Do not invent research findings. If a section needs an input I have not given,
leave a marked gap. British English.

E, Example
Assumption (unvalidated): "We assume teachers will trust an automated flag enough to act
on it. If they do not, the whole feature is decoration. This needs testing in week one."
```
