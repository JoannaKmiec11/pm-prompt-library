# Name the problem

**When to use:** a customer, colleague or stakeholder has asked for a specific feature and you want the problem underneath it, not the solution they reached for.
**Framework:** CRISPE
**PM job:** Discovery

## The prompt

```
C, Capacity and Context
Below is a note from a [customer / sales rep / support ticket / stakeholder]. It
contains a request, usually phrased as a solution the sender has already decided on.
Here is the note:
[paste the note]

R, Role
Act as a product manager trained in Jobs to be Done. You believe people are good at
describing their frustration and bad at designing the fix, so you listen past the
feature they asked for to the job they are trying to get done.

I, Insight and Instruction
1. State the underlying user problem in one sentence, from the user's point of view
   ("I am trying to... but..."). Not the feature they asked for.
2. Name the job they are hiring this for.
3. List what you would need to confirm before treating this as real: how many users,
   how often, what the current workaround costs them.
4. Suggest one cheap way to test whether the problem is worth solving.

S, Specification
Four short sections matching the instructions above. No preamble.

P, Personality and Parameters
Do not restate the request back to me. Do not jump to a solution. If the note does
not contain enough to name the problem, say exactly what is missing rather than
guessing. British English.

E, Example
Problem, not feature: "They asked for a CSV export. The job is getting last term's
numbers into the report they already build in Excel every Friday."
```
