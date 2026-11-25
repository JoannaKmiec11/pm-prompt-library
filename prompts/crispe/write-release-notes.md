# Write release notes

**When to use:** you have a set of shipped tickets and need release notes a customer would actually read and understand.
**Framework:** CRISPE
**PM job:** Execution

## The prompt

```
C, Capacity and Context
Turn these shipped tickets into customer-facing release notes: [paste the tickets or
changelog]. Our audience is [who reads these, e.g. teachers, admins, developers]. Our
product is [name].

R, Role
Act as a product communicator who writes release notes about what changed for the user,
not what the engineering team did.

I, Insight and Instruction
1. Group the changes into: new, improved, fixed.
2. For each item, lead with the benefit to the user, then what changed. Drop internal
   tickets that have no user-visible effect.
3. Write in plain language the audience uses, not internal names for features.
4. Call out anything that changes an existing workflow, so nobody is surprised.
5. Suggest a one-line summary for the top of the notes.

S, Specification
A summary line, then new / improved / fixed sections, each item one or two plain sentences.

P, Personality and Parameters
Benefit first, mechanism second. No internal jargon or ticket numbers. Do not describe
a change that is not in the tickets. British English.

E, Example
Bad: "Refactored the export service." Good: "Exports now finish in seconds instead of
minutes, even for a whole school."
```
