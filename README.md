# The PM Prompt Library

A working library of the prompts a product manager actually uses, from naming a problem to
shipping release notes. Every prompt is written to be copied, filled in and run. Nothing
here is theoretical. Each one started as a prompt used on real product work.

Built and maintained by Joanna Kmiec.

## How to use it

1. Find the prompt by the **job you are doing** (the table below) or by **framework** (the
   folders).
2. Open it, copy the block in **The prompt**, and paste it into your AI tool of choice.
3. Replace everything in `[square brackets]` with your own context.
4. Run it. Read the output as a draft to react to, not an answer to accept.

Every prompt is written in **CRISPE** (explained at the bottom), so they read as one
system rather than a pile of snippets.

## Find by the job you are doing

### Discovery
- [Name the problem](prompts/crispe/name-the-problem.md) — get the problem under the feature request
- [Opportunity solution tree](prompts/crispe/opportunity-solution-tree.md) — map the opportunity space before committing
- [Identify risky assumptions](prompts/crispe/identify-risky-assumptions.md) — find what is most likely to kill the idea
- [Discovery interview script](prompts/crispe/interview-script.md) — ask about behaviour, not opinions

### Research
- [Synthesise research into themes](prompts/crispe/synthesise-research.md) — patterns out of notes, with the evidence attached
- [User personas from research](prompts/crispe/user-personas.md) — personas grounded in data, not invented
- [Competitor analysis](prompts/crispe/competitor-analysis.md) — map the field and find the gap you could own
- [Market sizing (TAM, SAM, SOM)](prompts/crispe/market-sizing.md) — a defensible size, bottom up
- [Customer journey map](prompts/crispe/customer-journey-map.md) — the lows that are really opportunities
- [Watch the sector](prompts/crispe/watch-the-sector.md) — the week's news filtered to what affects you
- [Research to opportunities (chained)](prompts/chained/research-to-opportunities.md) — notes to themes to personas to opportunities

### Strategy
- [Product vision](prompts/crispe/product-vision.md) — a vision people commit to, not a slogan
- [SWOT analysis](prompts/crispe/swot-analysis.md) — the value is in the crossing, not the four lists
- [Lean canvas](prompts/crispe/lean-canvas.md) — one page, weakest box exposed
- [Value proposition](prompts/crispe/value-proposition.md) — why you beat the alternative for a job
- [Pricing strategy](prompts/crispe/pricing-strategy.md) — priced on value, not cost-plus
- [USP Venn diagram](prompts/visual-and-diagram/usp-venn-diagram.md) — find the USP in the overlap
- [Red-team my thinking](prompts/personas-and-roles/red-team-review.md) — attack a plan before you commit

### Execution
- [Start the PRD](prompts/crispe/start-the-prd.md) — a PRD skeleton to react to
- [Write user stories](prompts/crispe/write-user-stories.md) — small, testable, with real acceptance criteria
- [Score the backlog (RICE)](prompts/crispe/score-the-backlog-rice.md) — prioritise with the working shown
- [Plan OKRs](prompts/crispe/plan-okrs.md) — outcomes, not a list of launches
- [Outcome roadmap](prompts/crispe/outcome-roadmap.md) — Now / Next / Later around problems
- [Pre-mortem](prompts/crispe/pre-mortem.md) — surface how it fails while you can still prevent it
- [Stakeholder map](prompts/crispe/stakeholder-map.md) — who to involve, when, and how
- [Run a retro](prompts/crispe/retro.md) — owned actions, not a wall of sticky notes
- [Write release notes](prompts/crispe/write-release-notes.md) — what changed for the user, in plain words
- [Problem to PRD to stories (chained)](prompts/chained/problem-to-prd-to-stories.md) — one connected pass
- [Stress-test a decision](prompts/verification/stress-test-decision.md) — argue with the reasoning, not the output
- [Workflow flowchart](prompts/visual-and-diagram/workflow-flowchart.md) — a process, before and after

### Data
- [Explain the metric drop](prompts/crispe/explain-the-metric-drop.md) — likely causes ranked before you dig
- [A/B test analysis](prompts/crispe/ab-test-analysis.md) — ship / extend / stop, backed by whether it is real
- [Cohort analysis](prompts/crispe/cohort-analysis.md) — is retention really improving, or is the bucket leaking
- [Write a SQL query](prompts/crispe/write-sql.md) — the query, with the logic explained
- [Multi-model comparison](prompts/verification/multi-model-comparison.md) — compare AI models on evidence

### GTM
- [Beachhead segment](prompts/crispe/beachhead-segment.md) — the smallest winnable first market
- [Ideal customer profile](prompts/crispe/ideal-customer-profile.md) — who to chase, and who to walk away from
- [Competitive battlecard](prompts/crispe/competitive-battlecard.md) — a one-pager a rep can use live
- [Multi-channel campaign (chained)](prompts/chained/multi-channel-campaign.md) — one voice across every channel

### Growth
- [North star metric](prompts/crispe/north-star-metric.md) — one customer-centric metric, and its drivers
- [Positioning statement](prompts/crispe/positioning-statement.md) — choose the frame you compete in

### Writing
- [Leadership update](prompts/crispe/leadership-update.md) — progress, risk, and the one decision you need
- [Change the audience](prompts/crispe/change-the-audience.md) — same message, retuned for each reader
- [Write in my voice](prompts/crispe/write-in-my-voice.md) — draft in your register, not the model's
- [Steelman the counterargument](prompts/verification/steelman-counterargument.md) — answer the strongest objection first
- [Role priming, and its trap](prompts/personas-and-roles/role-priming-pattern.md) — set a Role well, without faking a past
- [Flag it, do not fill it](prompts/verification/flag-dont-fill.md) — stop the model inventing missing facts
- [Reference card infographic](prompts/visual-and-diagram/reference-card-infographic.md) — a legible card that reads at a glance
- [Sensitive stakeholder email](prompts/human-in-the-loop/sensitive-stakeholder-email.md) — high-stakes comms with a review gate

## Browse by framework

The folders group prompts by the prompt-engineering pattern they use, so the craft is on show.

| Folder | What is in it |
|---|---|
| [`prompts/crispe/`](prompts/crispe/) | Single-shot prompts written in the CRISPE structure. The bulk of the library. |
| [`prompts/chained/`](prompts/chained/) | Multi-step prompts, where each step takes the last step's output as input. |
| [`prompts/personas-and-roles/`](prompts/personas-and-roles/) | Role-priming patterns, and using a persona to get a sharper point of view. |
| [`prompts/verification/`](prompts/verification/) | Prompts that check work: stress-test a decision, compare models, answer the counterargument. |
| [`prompts/visual-and-diagram/`](prompts/visual-and-diagram/) | Prompts whose output is an image or a diagram, and which tool to use for it. |
| [`prompts/human-in-the-loop/`](prompts/human-in-the-loop/) | Prompts with a deliberate review gate for high-stakes output. |

## How these are built: CRISPE

Every prompt is written in CRISPE, a structure that makes a prompt reliable and reusable:

- **C, Capacity and Context** — the background the model needs, facts declared once.
- **R, Role** — who it should act as, including the expertise and the bias.
- **I, Insight and Instruction** — what you want it to do.
- **S, Specification** — the format of the answer.
- **P, Personality and Parameters** — tone, constraints and the hard guardrails.
- **E, Example** — a short sample of the output you want.

Two rules show up in almost every prompt here, because they are what separate a useful
output from a confident wrong one:

1. **Flag it, do not fill it.** Tell the model to name what it could not answer rather than
   invent a fact. It is the cheapest quality control there is, and it has its own
   [write-up](prompts/verification/flag-dont-fill.md).
2. **Guardrails go near the end.** Models recall rules placed in Parameters better than
   ones buried in the middle.

The blank structure is in [`templates/crispe-template.md`](templates/crispe-template.md),
and [`CONTRIBUTING.md`](CONTRIBUTING.md) covers the house style if you fork this or add
your own.

## Licence

[MIT](LICENSE). Use them, change them, share them. Attribution is welcome but not required.
