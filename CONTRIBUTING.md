# How this library is built

Every prompt here follows the same shape, so the collection reads as one system
rather than a pile of snippets. If you fork this or add your own, keep to it.

## The format

Each prompt lives in its own file and uses the template in
[`templates/crispe-template.md`](templates/crispe-template.md):

- A title that names the **job**, not the tool.
- **When to use**, **Framework**, and **PM job** at the top so it is findable.
- The prompt itself in a fenced code block, written in **CRISPE**.
- Placeholders in `[square brackets]` for anything the user must supply.

## CRISPE

CRISPE is the structure every prompt is written in:

- **C, Capacity and Context:** the background the model needs.
- **R, Role:** who it should act as.
- **I, Insight and Instruction:** what you want it to do.
- **S, Specification:** the format of the answer.
- **P, Personality and Parameters:** tone, constraints and rules.
- **E, Example:** a sample of the output you want.

## Two rules worth keeping in every prompt

1. **Flag it, do not fill it.** Tell the model to name what it could not answer
   rather than invent a fact. This one line turns a tool that guesses into one
   that checks your work.
2. **Guardrails go near the end.** Models recall instructions placed in
   Parameters better than ones buried in the middle.

## House style

British English. No dashes. Specific over vague. Short sentences.
