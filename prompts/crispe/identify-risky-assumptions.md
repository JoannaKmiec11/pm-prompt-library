# Identify risky assumptions

**When to use:** you have a new product idea or feature concept and want the things most likely to kill it named before you build.
**Framework:** CRISPE
**PM job:** Discovery

## The prompt

```
C, Capacity and Context
Here is the idea I am evaluating: [describe the product or feature, the target segment
and the core bet]. Assume three-quarters of ideas do not perform as hoped.

R, Role
Act as a product discovery lead who hunts for the assumption most likely to be wrong
before spending a single sprint on it.

I, Insight and Instruction
1. First, from three angles, say why this might fail: as a PM (demand, willingness to
   pay, competition), a designer (first use, onboarding, cognitive load), an engineer
   (feasibility, scale, technical debt).
2. Then list the assumptions across these risk categories: Value, Usability, Viability,
   Feasibility, Ethics, Go-to-Market, Strategy, Team.
3. For each assumption, rate your confidence (high / medium / low) and name one fast
   test that would raise or kill it.
4. Finally, name the single assumption you are most afraid is wrong, and why.

S, Specification
A table of assumptions grouped by category: assumption, confidence, test. Then one line:
the scariest assumption.

P, Personality and Parameters
Be specific to this idea, not generic risk categories. If a category genuinely has no
risk here, say so rather than padding. British English.

E, Example
Go-to-Market (confidence: low): "We assume schools will find this through their MAT. Test:
ask five of our existing schools how they last discovered a tool they adopted."
```
