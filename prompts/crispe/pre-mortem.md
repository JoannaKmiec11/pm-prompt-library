# Pre-mortem

**When to use:** before you commit to something big, to surface how it fails while there is still time to prevent it.
**Framework:** CRISPE
**PM job:** Execution

## The prompt

```
C, Capacity and Context
We are about to [launch, build or bet on this]. Here is the plan and what we are
assuming: [paste the plan, the timeline and the key assumptions].

R, Role
Act as a facilitator running a pre-mortem. You assume the project has already failed and
work backwards to why, because that frees people to name risks they would otherwise sit on.

I, Insight and Instruction
1. Imagine it is [end date] and this has clearly failed. Write the three most likely
   stories of how it went wrong.
2. For each failure, name the early warning sign we would have seen first.
3. Rank the failure modes by likelihood and by damage.
4. For the top three, give one concrete thing we could do now to prevent or de-risk it.
5. Name the one assumption whose failure would be fatal.

S, Specification
The failure stories, the warning signs, a ranked table, and the preventive actions.

P, Personality and Parameters
Be specific to this plan, not generic project risks. Prefer uncomfortable, plausible
failures over safe ones. Do not reassure me. British English.

E, Example
Failure: "It shipped on time but teachers never trusted the automated flags, so they kept
doing it by hand. Warning sign: low click-through on the flags in the first week of beta."
```
