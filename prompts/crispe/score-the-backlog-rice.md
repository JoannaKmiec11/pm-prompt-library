# Score the backlog (RICE)

**When to use:** you need a defensible prioritisation of features or ideas, with the working shown so stakeholders can argue with the inputs, not the output.
**Framework:** CRISPE
**PM job:** Execution

## The prompt

```
C, Capacity and Context
Score these against RICE: [paste the list of features or ideas]. For each, here is what
I know about reach, impact, confidence and effort:
[paste any data; say where you have none]

R, Role
Act as a product manager who uses RICE to make the trade-offs visible, not to hide a
decision behind a number. You remember RICE prioritises bets, and that the real argument
is about the inputs.

I, Insight and Instruction
1. For each item, estimate Reach (users affected per period), Impact (value per user),
   Confidence (0 to 100%) and Effort (person-months).
2. Score = (Reach x Impact x Confidence) / Effort. Show the numbers behind every score.
3. Rank the list.
4. Call out the items where the ranking is driven by a shaky Confidence or Effort guess,
   because those are where the ranking could flip.
5. Note where I should prioritise the problem, not the feature, before scoring at all.

S, Specification
A table: item, R, I, C, E, score, rank. Then the shaky-input call-outs.

P, Personality and Parameters
Show your working so I can argue with it. Where I gave you no data, mark the input as a
guess rather than presenting it as known. Do not let a precise-looking score imply
false certainty. British English.

E, Example
"Export-to-PDF ranks third, but only because I guessed Confidence at 80%. If it is really
50%, it drops to seventh. That guess is the thing to check, not the score."
```
