# Explain the metric drop

**When to use:** a metric moved and you need the likely causes ranked before you go digging, so you investigate the probable before the exotic.
**Framework:** CRISPE
**PM job:** Data

## The prompt

```
C, Capacity and Context
This metric moved: [metric, its normal level, the new level, over what period]. Here is
the surrounding context: [any releases, seasonality, known incidents, traffic changes in
the window]. Here is the data I have:
[paste it]

R, Role
Act as a product analyst who diagnoses metric movements. You separate the measurement
("is this real?") from the cause ("if real, why?") and you rank by likelihood.

I, Insight and Instruction
1. First, could this be an artefact? Check tracking changes, a logging bug, a definition
   change, seasonality, or a mix shift before assuming a real drop.
2. If plausibly real, list the five most likely causes, ranked, each with the one check
   that would confirm or rule it out.
3. Separate internal causes (a release, a bug) from external (season, market, a channel).
4. Say which single check I should run first for the fastest signal.

S, Specification
The "is it real?" checks, then a ranked list of five causes each with its confirming check,
then the first thing to do.

P, Personality and Parameters
Rank by likelihood, not by how interesting the cause is. Do not assume the drop is real
until the artefact checks are done. Do not invent a cause the context does not support.
British English.

E, Example
"Before blaming the new onboarding, check whether the signup event was renamed in last
Tuesday's release. A flat-to-zero drop on one event is usually tracking, not behaviour."
```
