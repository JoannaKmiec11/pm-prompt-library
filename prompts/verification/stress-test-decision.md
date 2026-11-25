# Stress-test a decision (show your working)

**When to use:** a model or a colleague gave you an answer, a score or a recommendation, and you want to be able to argue with the reasoning, not just accept the output.
**Framework:** Verification
**PM job:** Execution

## The prompt

```
C, Capacity and Context
Here is a decision, score or recommendation I have been given: [paste it, including any
numbers or rankings]. Here is the reasoning behind it, if I have it:
[paste the reasoning, or say it was not shown]

R, Role
Act as a reviewer whose job is to make the reasoning visible and testable, so I can
challenge the inputs rather than take the output on trust.

I, Insight and Instruction
1. Reconstruct the logic step by step. What inputs and assumptions produce this output?
2. Identify which inputs the conclusion is most sensitive to: the ones where a small
   change flips the answer.
3. For each sensitive input, say how confident we really are in it and how to check it.
4. Give the one input most worth verifying before acting on this.

S, Specification
The reconstructed logic, the sensitive inputs, a confidence read on each, and the one to check.

P, Personality and Parameters
Attack the inputs, not the person. A precise-looking number can rest on a shaky guess, so
separate what is known from what is assumed. If the reasoning is genuinely sound, say so.
British English.

E, Example
"The RICE ranking puts this first, but that depends entirely on a Confidence of 90% that
was never justified. Drop it to 50% and it falls to fourth. Verify the confidence first."
```

## Notes

- This is the generalised version of "score these and show your working so I can argue with
  it". The value of any score is in the inputs you can contest, not the number itself.
