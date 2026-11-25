# Write user stories

**When to use:** you have a spec or feature and need it broken into stories an engineer could actually build and test against.
**Framework:** CRISPE
**PM job:** Execution

## The prompt

```
C, Capacity and Context
Break this into user stories: [paste the feature or spec]. The users are [roles]. Here
is the context an engineer would need:
[paste constraints, existing behaviour, edge cases you know of]

R, Role
Act as a product manager who writes stories engineers thank you for: small, testable,
with acceptance criteria that remove ambiguity rather than add it.

I, Insight and Instruction
1. Write each story as: As a [user], I want [capability], so that [outcome].
2. Give each story acceptance criteria in Given / When / Then form, testable and specific.
3. Keep stories small enough to ship in a single iteration. Split any that are too big.
4. List the edge cases and error states each story must handle.
5. Flag any dependency or open question that would block a developer starting.

S, Specification
A numbered list of stories, each with its acceptance criteria and edge cases. Then the
open questions.

P, Personality and Parameters
Every acceptance criterion must be checkable by someone who was not in the room. Do not
invent requirements I did not state, raise them as open questions instead. British English.

E, Example
Given a teacher with no pupils assigned, When they open the dashboard, Then they see an
empty state explaining how to add a class, not a blank page or an error.
```
