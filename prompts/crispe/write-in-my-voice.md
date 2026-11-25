# Write in my voice

**When to use:** you want an AI to draft in your voice instead of its own default register, for posts, messages or application answers.
**Framework:** CRISPE
**PM job:** Writing

## How to use

This prompt works best when you first give the model a short, honest spec of how you
actually write, built from real examples of your own words, not how you wish you wrote.
Fill the voice block below once and reuse it. The example here uses a sparse version;
replace it with yours.

## The prompt

```
C, Capacity and Context
Draft [what: a LinkedIn post / a message to X / an application answer] about [topic]. The
one thing it has to say is [the single point]. Here is the raw material and any facts you
must not get wrong:
[paste it]

R, Role
Act as a writer working from my voice spec below. Match this register, not a cleaned-up
version of it.

My voice:
- [e.g. British English. No dashes anywhere. Short sentences, one idea each.]
- [e.g. Specific over vague: name the company, the tool, the number.]
- [e.g. Lead with the concrete moment, context second.]
- [e.g. Signature move: "I don't X, I Y".]
- Phrases I never use: [list your own banned filler and corporate words].
- Here are three sentences I actually wrote, to match the rhythm of:
  [paste three real sentences of your own]

I, Insight and Instruction
Write the piece. Lead with the specific thing. Say one thing. Answer "so what" before you
finish. If it is a story, name the outcome, including if it failed.

S, Specification
[Length and format, e.g. "Under 150 words. A hook first line. No hashtags."]

P, Personality and Parameters
Do not use any banned phrase above. Do not invent a fact, a number or an outcome I did
not give you. If a sentence sounds quotable or like an aphorism, it is probably wrong,
cut it. Verify every factual claim against what I gave you. British English.

E, Example
[paste one short piece of your own writing as the target to match]
```

## Notes

- The single biggest lever is the three real sentences in the Role block. A model mimics
  rhythm from examples far better than from adjectives like "direct" or "warm".
- Keep an "accuracy" rule in Parameters. Voice prompts drift into invented detail fastest.
