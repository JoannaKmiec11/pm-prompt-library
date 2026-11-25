# Sensitive stakeholder email, with a review gate

**When to use:** you have to send something consequential, an apology, a breach notice, bad news, a correction, and the cost of a wrong or invented detail is high.
**Framework:** Human in the loop (CRISPE, with a mandatory review list)
**PM job:** Writing

## Why a review gate

For sensitive comms, the danger is not bad prose, it is a confident, invented detail: a
cause that did not happen, advice that does not apply, a claim you cannot stand behind. So
the prompt does two things: it forbids invention, and it ends by handing you a list of
things to check before you send. You are the gate. The model drafts, you decide.

## The prompt

```
C, Capacity and Context
I need to send [what, to whom] about [what happened]. Here are the facts, and only these
are true:
[what happened, plainly; the real cause; what is and is not affected; what you have
already done]
The audience is [who they are and your relationship to them].

R, Role
Act as a [domain]-aware communications adviser who has handled messages like this for
[context], advising someone who has to send it personally.

I, Insight and Instruction
Write the message. It must:
- Say plainly what happened, in the first two sentences, without softening it.
- State exactly what is and is not affected.
- Name who is responsible in the active voice. No "mistakes were made".
- Give an honest assessment of the risk, neither minimised nor inflated.
- [Any domain requirements: e.g. regulatory steps, deadlines, the recipient's rights.]
- Apologise once, properly, for the actual thing. Not for "any inconvenience caused".
- Give a named contact and a clear next step.

S, Specification
A subject line, then the body under [length]. After the message, list in bullets
everything I should check or confirm before sending.

P, Personality and Parameters
Warm, direct, human. [Banned phrases: e.g. no "we take your privacy seriously", no "out of
an abundance of caution".] Do not invent any fact not given above. If a fact is missing,
put it in the check-before-sending bullets rather than filling the gap. Do not give advice
that does not apply here. British English.

E, Example
Opening tone to match: "[one plain, human sentence, the opposite of a corporate notice]"
```

## Notes

- The most valuable output is the check-before-sending list. Giving the model permission to
  say "I am not sure, confirm this" turns it from something that guesses into something that
  checks your work. In one real run it flagged a fact the author had asserted as settled but
  had never actually established.
- List the specific phrases to ban. "Avoid corporate language" is weaker than naming the
  three phrases the model will otherwise reach for.
- If this is a real regulated event, not a draft, start from the official guidance as your
  Context rather than from memory.
