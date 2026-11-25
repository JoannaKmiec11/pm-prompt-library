# Problem to PRD to stories

**When to use:** you want to go from a raw problem to a PRD skeleton to buildable user stories in one connected pass, so the thread holds the whole way down.
**Framework:** Chained (three prompts, each takes the previous output as input)
**PM job:** Execution

## Why chain it

Each step inherits the last step's output, so the problem framing you agree in step 1 is
carried into the PRD and then into the stories. You review and correct at each gate before
moving on, which is cheaper than discovering a bad assumption in the stories.

## Prompt 1: frame the problem

```
C, Capacity and Context
Here is a problem I want to work on: [describe it, who has it, the evidence it is real].

R, Role
Act as a product manager who refuses to move to a solution until the problem is sharp.

I, Insight and Instruction
State the underlying problem in one sentence from the user's view. Name the job to be
done, the outcome we want, and the single assumption we are most afraid is wrong.

S, Specification
Four lines: problem, job, outcome, scariest assumption.

P, Personality and Parameters
No solutions yet. If the problem is not evidenced, say so. British English.
```

**Gate 1:** correct the framing before continuing.

## Prompt 2: draft the PRD skeleton

```
Using the problem, job, outcome and assumption above, draft a PRD skeleton: summary,
background, objective with SMART key results, segments (by job, not demographics), value
propositions, solution with the key features, and a release split of first version versus
later in relative timeframes. Mark every assumption explicitly. Do not invent research.
```

**Gate 2:** fix the objective and scope before continuing.

## Prompt 3: break it into stories

```
Using the solution and features in the PRD above, write user stories in the form
As a [user], I want [capability], so that [outcome], each with Given/When/Then acceptance
criteria and the edge cases it must handle. Keep each story shippable in one iteration.
List any open question that would block a developer rather than inventing the answer.
```

## Notes

- Keep a human gate between each step. The point of chaining is to catch a wrong turn
  early, not to run three prompts unattended.
- The "mark every assumption" and "list open questions rather than invent" rules carry the
  honesty down the chain, so the stories do not quietly harden a guess into a requirement.
