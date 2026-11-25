# Role priming, and its trap

**When to use:** any time you set a Role in a prompt. This is a pattern to reuse, plus the one mistake that quietly corrupts output.
**Framework:** Pattern (applies to the R in CRISPE)
**PM job:** Writing

## The pattern

A good Role does more than name a job title. It names the expertise, the bias, and what
the persona cares about, so the model adopts a point of view rather than a costume.

```
R, Role
Act as [specific expertise, not just a title]. You [the belief or bias that shapes how
they work]. You care about [what matters to them], not [what they ignore].
```

Compare:
- Weak: "Act as a marketer."
- Strong: "Act as a senior marketer who has launched sustainable food brands in London.
  You build communities around independent brands. You care about honesty before sales."

The strong version changes what the model prioritises, not just its vocabulary.

## The trap: the biography leaks

A Role with invented experience can leak that invention into the output as if it were true.

A real example. A prompt set the role as "a community organiser with over 20 years of
experience" and asked for a launch post for a first-ever event. One model opened with
"Throughout my career I have seen the power of shared experiences". That is a fabricated
biography, written in the first person, presented as fact. The role instruction leaked
out of the brief and into the copy.

## The fix

When the Role gives the persona experience the real author does not have, add a guardrail
in Parameters:

```
P, Personality and Parameters
The role is a lens for how you write, not a biography to claim. Do not write anything
about my experience, history or track record that I have not given you. Do not open with
"excited" or "thrilled" or imply a past I do not have.
```

## Notes

- Use a Role to borrow a way of thinking, never to borrow a past. The longer, more careful
  version of a prompt keeps this guard. The short version drops it, and the fabrication is
  the first thing that comes back.
