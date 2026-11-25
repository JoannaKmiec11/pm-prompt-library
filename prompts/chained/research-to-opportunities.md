# Research to opportunities

**When to use:** you have raw interview notes and want to get from them to themes, to personas, to a prioritised opportunity list, without losing the evidence trail.
**Framework:** Chained (three prompts)
**PM job:** Research

## Why chain it

Synthesis, personas and opportunities are three different jobs. Doing them in one prompt
blurs them. Chaining keeps each step honest and lets you check the evidence before it
hardens into a persona or a roadmap item.

## Prompt 1: synthesise the themes

```
C, Capacity and Context
Here are interview notes from [N] participants in [study]:
[paste the notes]

R, Role
Act as a researcher who reports no theme without a quote to evidence it.

I, Insight and Instruction
Identify the recurring themes. For each: a one-line name, the best verbatim quote with
its participant number, and how often it appeared. Flag any surprise. List the gaps.

S, Specification
A ranked list of evidenced themes, then surprises and gaps.

P, Personality and Parameters
No theme without a real quote. Do not invent quotes. British English.
```

**Gate 1:** confirm the themes are evidenced, not inferred.

## Prompt 2: build personas from the themes

```
Using the themes above, build 3 distinct personas. For each: the characteristics that
matter, the primary job to be done, top three pains, top three gains, and one unexpected
insight from the data. Keep every persona grounded in the themes and quotes above. Flag
any persona the data is too thin to support rather than inventing one.
```

**Gate 2:** cut or merge any persona not backed by the research.

## Prompt 3: turn pains into prioritised opportunities

```
Using the personas and their pains above, write them as opportunities from the customer's
view ("I struggle to..."). Prioritise with Opportunity Score = Importance x (1 - Satisfaction),
both normalised to 0 to 1, using the research to estimate each. Return the ranked
opportunities and, for the top three, one cheap experiment each to test whether solving it
would move our outcome.
```

## Notes

- The evidence trail survives the whole chain: every opportunity can be traced back to a
  quote. That traceability is what makes the output defensible to a sceptical stakeholder.
