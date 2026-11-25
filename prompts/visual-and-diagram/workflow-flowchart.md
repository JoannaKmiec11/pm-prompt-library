# Workflow flowchart

**When to use:** you want to show a process as a flowchart, often a "before and after": the manual workflow next to the streamlined or automated one.
**Framework:** CRISPE (diagram output)
**PM job:** Execution

## The prompt

```
C, Capacity and Context
I want to diagram this process: [name it]. Here are the steps as they happen today:
[list each step in order, who does it, and any decision points or handoffs]. If I want a
before and after, here is the improved version:
[list the streamlined or automated steps]

R, Role
Act as a process analyst who draws flowcharts that show the real mechanism, including the
decision points and the handoffs where work waits or is lost.

I, Insight and Instruction
1. Draw the current ("manual") workflow as a flowchart: steps, decisions (diamonds),
   handoffs, and any loop-backs.
2. If given, draw the improved ("streamlined") workflow beside it.
3. Mark where the improved version removes a step, a handoff or a wait.
4. Below the diagram, state in one line what the change actually saves: time, errors, or
   a handoff removed.

S, Specification
A flowchart (or diagram code I can paste into a diagramming tool, e.g. Mermaid). Clear
start and end, labelled decision branches. If before and after, lay them side by side.

P, Personality and Parameters
Show the decision points honestly, including the ugly loop-backs. Do not simplify the
current state to make the new one look better than it is. Only diagram steps I gave you.
British English.

E, Example
Current: "Insight arrives, a human reads it, tags it by hand, files it, repeat." Improved:
"Insight arrives, the model tags it, a human reviews only the low-confidence ones." The
saving: the human stops reading every one and reviews the exceptions.
```

## Notes

- For a flowchart, a diagramming tool (or Mermaid text) beats an image generator: the boxes
  stay aligned and the labels stay legible. See
  [reference card](reference-card-infographic.md) on why text-heavy images need a design tool.
