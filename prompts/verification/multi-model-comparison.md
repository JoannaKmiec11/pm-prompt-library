# Multi-model comparison

**When to use:** you want to compare several AI models on a real task and decide which output to use, on evidence rather than on which one "feels" best.
**Framework:** Verification / evaluation harness
**PM job:** Data

## The idea

Comparing AI outputs on whether they feel good proves nothing. Build the prompt so that
most of what it asks for is checkable, then score each model against the same checklist.
Two additions make a comparison real:
- A **trap**: ask for something that does not exist (a detail you genuinely do not have),
  and count which models invent it rather than leave the gap.
- A **self-report**: ask each model for something you can verify independently (its own
  word count), and check whether it is accurate.

## The prompt to run across models

```
Act as [role]. Produce [the deliverable: type, length, topic]. It must include [the
checkable requirements, listed]. Do not invent [the detail you do not actually have]; I do
not have it yet. At the end, give me [a self-reported, verifiable fact, e.g. your word count].
```

To run it side by side, use a tool that puts models in parallel columns, or paste the same
prompt into each model's own free tier and compare by hand.

## The scoring table

One row per thing the prompt asked for, one column per model. Mark pass or fail, then count.

| # | Criterion | How to check it | Model A | Model B | Model C | Model D |
|---|---|---|---|---|---|---|
| 1 | Met the length, verified in a counter (not the model's own claim) | | | | | |
| 2 | Reported its own count | | | | | |
| 3 | That count was accurate | | | | | |
| 4 | Did not invent the detail it was told it lacked | | | | | |
| 5 | [requirement] | | | | | |
| 6 | [requirement] | | | | | |
|   | **Score** | | | | | |

Then one line the table cannot give you: **which output would you actually use, and why.**
The highest score and the best writing are often different models, and that gap is the most
interesting finding.

## Notes

- A short prompt is cheaper and easier to compare. A longer, fully specified prompt gets
  closer to usable on the first pass but costs more to run across several models. That trade
  is itself worth recording.
- Free tiers run out. If a tool blocks you, compare the cheaper small models instead. They
  are often the ones companies actually deploy at scale, so the comparison is arguably more
  useful, not less.
- Watch for a fabricated biography: a role like "20 years of experience" can leak into the
  output as a false first-person claim. See
  [role priming](../personas-and-roles/role-priming-pattern.md).
