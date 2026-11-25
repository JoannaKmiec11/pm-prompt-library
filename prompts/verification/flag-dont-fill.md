# Flag it, do not fill it

**When to use:** add this to any prompt where the model might invent a missing fact rather than admit it does not have one. It is the cheapest quality control in this library.
**Framework:** Pattern (a Parameters add-on for any prompt)
**PM job:** Writing

## The problem it solves

Models fill gaps by default. Ask for a launch post without a confirmed venue and many will
invent a plausible venue. Ask for a breach email and a bare prompt may invent a cyber
attack, an investigation and third-party experts, none of which happened. The instinct to
complete the picture is exactly what you do not want when the facts are not yours to invent.

## The add-on

Put this in the Parameters section of any prompt:

```
P, Personality and Parameters
Do not invent any fact I have not given you: no names, numbers, dates, quotes, prices or
events. If you want a fact you do not have, do not fill the gap. Instead, at the end,
under a heading "What I could not answer", list each missing fact and why you needed it.
```

## Why it works

It turns the gap-filling instinct into a checklist handed back to you. Instead of guessing,
the model tells you what it would have had to guess, which is often the most useful thing in
the whole output. Giving a model explicit permission to say "I do not know" changes it from
something that guesses into something that checks your work.

## A stronger version

It can also challenge facts you asserted as settled:

```
In "What I could not answer", also flag any fact I stated as certain that you think is
actually an assumption or a judgement I have not established.
```

A real run of this caught two things the author had written as fact: that a breach met the
reporting threshold (a judgement, not a given) and that an email "was recalled" (an
assumption, not a confirmed event). The model was checking the brief, not just following it.

## Notes

- Reuse this in every prompt where accuracy matters more than completeness. It costs one
  paragraph and repeatedly earns it back.
