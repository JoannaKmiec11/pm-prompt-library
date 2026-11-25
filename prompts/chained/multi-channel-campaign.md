# Multi-channel campaign

**When to use:** you are launching something and need copy across several channels that all sound like one brand, because the facts and voice are declared once and inherited.
**Framework:** Chained (three prompts)
**PM job:** GTM

## Why chain it

The brand facts and voice go in Prompt 1. Every channel after it inherits them, so the
voice holds across the blog, the social posts and the partner email instead of drifting.
Declare the guardrails once, near the end of Prompt 1, where the model recalls them best.

## Prompt 1: the anchor piece (a blog post)

```
C, Capacity and Context
We are launching [product or event]: [what it is, who it is for, why it matters].
Brand facts (use only these, do not invent others):
[list the facts: what is true, and nothing more]

R, Role
You are [a named marketer persona with relevant experience and a described voice:
e.g. warm, confident, plain, a light touch of wit].
Priorities in order: [e.g. honesty, community, then sales].

I, Insight and Instruction
Write a [length] blog post that [goal, e.g. builds trust and excitement]. Lead with
[the hook or the reassurance, not the information].

S, Specification
[Length, a headline and hook, short paragraphs, a call to action, any SEO keywords.]

P, Personality and Parameters
[Tone.] No invented statistics, certifications, quotes or prices. Avoid clichés like
"game-changer". If you make any assumption, list it at the end. British English.

E, Example
Tone to match: "[one sentence in the exact register you want]"
```

**Gate 1:** check the facts and the voice. This output becomes the input for everything else.

## Prompt 2: repurpose for social

```
Using the blog post above, repurpose it for:
1. A LinkedIn post ([length], professional, for [B2B audience]), 3 to 5 hashtags.
2. An Instagram caption (under [length], playful, for [audience]), a one-line hook,
   a few emojis, a call to action, 5 to 8 hashtags.
Keep the same brand voice, adapted to each channel. Suggest one visual idea for each.
```

## Prompt 3: the partner or sales email

```
Now write a [length] email to [partners or prospects] about the launch. Include a clear
subject line plus one alternative, what makes us different (from the brand facts only),
and a specific call to action. Same brand voice. No invented prices, stats or claims.
```

## Notes

- The most useful line in Prompt 1 is "if you make any assumption, list it at the end". It
  turns the model's gap-filling into a checklist you can review before anything is published.
- A chain does not travel between tools. If you move from a chat model to an image tool or
  a site builder, you re-establish the context there.
