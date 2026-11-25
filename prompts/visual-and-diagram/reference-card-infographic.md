# Reference card infographic

**When to use:** you want a single, legible reference image, a card of items grouped and numbered, that reads at a glance and survives being projected.
**Framework:** CRISPE (visual output)
**PM job:** Writing

## Pick the right tool first

An image that is mostly text (a reference card, a grid of labelled items) should be built
in a design tool, not a diffusion image generator. Diffusion models reliably garble small
type and quietly reword your labels. Use a tool that places real text accurately.

## The prompt

```
C, Capacity and Context
I am building one image: a reference card titled "[title]". It contains [N] items, which
are fixed and listed in the Instruction below. Do not invent, reword or reorder them. The
audience is [who will read it] and it may be [projected / shared / printed].

R, Role
Act as an information designer who builds reference cards for practitioners. You care about
legibility at a glance and when projected, not decoration.

I, Insight and Instruction
Produce a single [landscape/portrait] image: a numbered [N]-cell card titled "[title]",
subtitle "[subtitle]". Each cell contains, in this order: the number, a short label of
three or four words, and the item itself in one line.
[list every item exactly as it must appear]
Group them as [the grouping, e.g. two rows: "taking information in", then "deciding"].

S, Specification
- [Aspect ratio and size, e.g. 16:9, sized for a slide.]
- [Layout, e.g. two rows of five, numbered left to right.]
- Every cell the same size, with clear separation.
- Body text no smaller than the equivalent of 16px at the final width.
- No icons, no stock photography, no decorative illustration.

P, Personality and Parameters
- Colours: [hex values]. Typeface: [name or "a clean geometric sans"].
- Every word spelled correctly and matching the text above exactly. Accurate text matters
  more than visual flourish.
- If anything will not fit legibly, shorten the label and tell me. Do not shrink the type.
- British English.

E, Example
Tone to match: a reference card pinned above a desk, not a marketing infographic. Plenty
of white space, no ornament.
```

## Notes

- The hardest part of this brief is text accuracy. The guardrail that does the most work is
  "accurate text beats flourish" plus "shorten the label rather than shrink the type".
- Write for the reader, not for yourself. One card originally carried internal workflow
  codes on every cell. They meant nothing to anyone but the author, so they were replaced
  with something the reader could use. Put nothing on the card that needs a decoder.
