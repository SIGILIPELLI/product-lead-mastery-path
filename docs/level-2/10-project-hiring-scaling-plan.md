# Project — Hiring & Team-Scaling Plan

Everything in Level 2 converges here. A team-scaling plan is the document
where your cascaded strategy (Module 5) determines your org shape, your org
shape determines your headcount, your headcount has to survive a budget
conversation (Module 9), your hires have to clear a defensible bar (Module
6), and the people already on the team have to be developed, rated, and in
some cases moved (Modules 3 and 7) rather than simply outnumbered by new
arrivals.

The reason this is one document rather than five is that these decisions are
coupled, and Leads who make them separately produce plans that don't
survive contact with a CFO. Headcount asked for without a strategy problem
attached gets cut. An org redesign without a budget line doesn't happen. A
hiring plan without a ramp model produces four PMs starting the same month
with nobody to onboard them.

What you'll produce is a document you could genuinely take into a planning
round: 4-6 pages, mostly tables, with numbers you can defend without
looking anything up.

## What you'll build

| Section | Source module | The question it answers |
|---|---|---|
| 1. Strategy → problems | Module 5 | What must be true for the company bet to work? |
| 2. Current-state org map | Modules 2, 3 | What have we got, and how good is it really? |
| 3. Target org shape | Modules 2, 5 | What structure does the strategy require? |
| 4. Gap analysis | Modules 3, 9 | Which gaps are hires, which are development, which are exits? |
| 5. Hiring plan & sequence | Modules 6, 9 | Who, in what order, hired against what bar? |
| 6. Budget case | Module 9 | What does it cost, what's the return, what's self-funded? |
| 7. Ramp & onboarding | Modules 7, 9 | How do these people become productive? |
| 8. Risks & the downside plan | Modules 1, 8 | What if we get half of it, or none? |

## Step 1 — Fix the scenario

Use your real team if you have one. Otherwise take this brief, which is
deliberately constrained enough to force real choices:

> A 320-person B2B SaaS. You lead product: 4 PMs across 4 squads, 2
> designers, no dedicated researcher. The company has committed to a new
> primary segment for FY26. Product-org budget is £790k; you may request an
> increase but the default answer is flat. Engineering is growing 20% and
> your peer eng director expects product coverage to match.

Whichever you use, write down three things now: the company bet in one
sentence, your current total spend, and your current PM-to-engineer ratio.
Everything downstream is derived from those.

## Step 2 — Strategy to problems

Write the product-strategy layer from Module 5: the 2-3 problems that must
be solved for the bet to work, each with a line of evidence. Then run the
coverage check — map every existing squad to a problem.

Do not skip the orphan finding. A squad that maps to no strategy problem is
either the funding source for your entire plan or the first thing a CFO
cuts, and it's much better to be the one who proposes it.

## Step 3 — Current-state org map

One row per squad. Be honest in the last two columns; a scaling plan built
on flattering assessments falls over in month two.

| Squad | PM (level) | Strategy problem | Metric + current value | Eng count | PM capacity used | Honest capability read |
|---|---|---|---|---|---|---|
| Onboarding | Ravi (PM) | P1 churn | Time-to-live 11d (target 7) | 6 | 100% | Strong delivery; discovery developing (active coaching contract) |
| Pricing | Sofia (Senior PM) | P2 pricing gap | 2 pilots live (target 5) | 5 | 130% — 60% on pilot support | Strongest PM; over-extended |
| Integrations | Tom (PM) | P3 silent failures | P1s 4/qtr (target 2) | 4 | 80% | Reliable; low influence with partners |
| Internal Tools | Priya (PM, 6mo) | None | Handle time −6% | 3 | 90% | New; no baseline data; unclear mandate |

The two columns people fudge are capacity and capability. A PM at 130% is
not a resilient plan; a PM you privately doubt is not a hire you can defer.

## Step 4 — Target org shape

Design the shape the strategy needs, not the shape that preserves everyone's
current scope. State the model and the reason.

| Target squad | Strategy problem | PM required (level) | Why this shape | Change from today |
|---|---|---|---|---|
| Onboarding | P1 | PM | Owns the highest-value churn surface end to end | Unchanged |
| Pricing — core | P2 | Senior PM | Pilot support and product build are two jobs; splitting them is the whole point | New hire |
| Pricing — expansion | P2 | PM (Sofia) | Sofia moves to the strategic half | Rescoped |
| Integrations | P3 | PM | Irreversible partner deprecation; can't be starved | Unchanged |
| Support tooling | P1 (indirect) | 0.5 PM | Folds into Onboarding's problem rather than standing alone | Rescoped from Internal Tools |

Write one paragraph on what you deliberately did *not* do — the platform
squad you'd love to stand up, the research function you can't yet fund.
Named non-decisions are what make the plan read as considered rather than
maximal.

## Step 5 — Gap analysis

Every gap has three possible answers, and hiring is only one of them. Leads
who reach for the hire every time get treated as a cost centre.

| Gap | Hire / Develop / Restructure / Exit | Rationale | Timeline |
|---|---|---|---|
| Pricing over-extended | Hire (Senior PM) | Two jobs in one role; no internal candidate at level | Q2 |
| Ravi's discovery depth | Develop | Active coaching contract, checkpoint 15 March | 6 weeks |
| Tom's partner influence | Develop + restructure | Coaching plus you attend the first two partner reviews | Q2 |
| Internal Tools has no mandate | Restructure | Fold into Onboarding; Priya takes support tooling under P1 | Q1 |
| No research capability | Neither — accept | Not fundable this year; PMs run their own discovery | Reviewed Q4 |

An honest plan has at least one "accept" row. A plan where every gap is
solved is a wish list.

## Step 6 — Hiring plan and sequence

Sequence matters as much as count. Every hire consumes onboarding capacity —
yours — and two PMs starting the same month means neither gets it.

| # | Role | Quarter | Why this order | Onboarding owner | Self-funded by |
|---|---|---|---|---|---|
| 1 | Senior PM, Pricing core | Q2 | Gates the FY26 pricing decision in July | You | Internal Tools PM fold |
| 2 | PM, Onboarding depth | Q4 | Only if Ravi's coaching checkpoint fails or eng growth lands | Ravi | New budget |

Then attach the Module 6 scorecard for hire #1 — mission, three must-haves,
nice-to-haves, and the explicit non-requirements row — plus the four-person
panel with one signal per interviewer. A hiring plan without a written bar
is a headcount request wearing a hiring plan's clothes.

## Step 7 — The budget case

| Line | Amount | Note |
|---|---|---|
| Current product-org spend | £790k | Baseline |
| Internal Tools PM fold | −£110k | Self-funding source; support handle-time work stops |
| Senior PM, Pricing (from Q2) | +£83k | 9 months of £110k loaded |
| Pricing contractor, 6 weeks | +£18k | Bridges to the hire's start date |
| Research incentives increase | +£6k | Discovery load moves onto PMs |
| **Net FY26 change** | **−£3k** | Effectively flat |

Then write the two-option trade-off from Module 8 — what the plan delivers
funded, what it delivers if declined, your recommendation, and the single
fact that should decide it. If your plan is net-flat, say so in the first
line; a flat plan gets read differently from a growth plan, and you want it
read the right way.

## Step 8 — Ramp and the downside plan

A ramp table stops "when will they be productive?" from being answered with
optimism.

| Milestone | Week | Observable evidence |
|---|---|---|
| Context loaded | 2 | Can state the strategy problem and the metric unprompted |
| First decision owned | 4 | Makes a scope call in review without deferring to you |
| First discovery cycle | 8 | Five customer conversations, one item killed or reshaped |
| Owning the metric | 13 | Presents the pricing pilot outcome to the exec review themselves |

Then the downside plan, which is the section that most distinguishes a
senior plan from a junior one:

| Scenario | Response |
|---|---|
| Hire approved but slips a quarter | Contractor extends 6 more weeks; pilot target drops from 5 to 4 |
| Hire declined outright | Sofia sheds pilot support to Ravi's squad; FY26 pricing decision moves to January, stated in writing now |
| Budget cut a further 10% | Concentrated: Integrations coverage goes to 0.5 PM, with the deprecation risk named and accepted by the exec who cuts it |
| Ravi's coaching checkpoint fails | Coaching converts to a Module 3 performance conversation; the Q4 hire moves to Q3 |

## Cheat sheet — what a reviewer will check

| Section | The question they'll actually ask |
|---|---|
| Strategy → problems | Can every squad be traced to a company-level bet? |
| Current state | Is the capacity column honest, or diplomatic? |
| Target shape | What did you decide *not* to build, and why? |
| Gap analysis | Is every gap a hire? (If yes, the plan isn't credible) |
| Hiring sequence | Who onboards each hire, and do two start at once? |
| Budget | Is there a self-funding source, and do you know your numbers cold? |
| Ramp | Is productivity defined by an observable, or by a feeling? |
| Downside | What happens if you get none of this? |

## Stretch goals

Once the core document is assembled, take it further:

1. **Run the sum test on the whole plan.** If every squad in the target
   shape hits its metric, does the company bet actually advance far enough?
   Write the arithmetic. If it doesn't, your plan is under-scoped and you
   should say so before someone else notices.
2. **Write the three-year version.** Same strategy, but 12 squads instead of
   5. At what headcount does your current management span break, and what's
   the first management layer you'd add? Name who you'd promote into it and
   what they'd need to develop first.
3. **Cost your own time.** Map your attention across the target org using
   the Module 2 stakes × self-sufficiency model. If the plan leaves you at
   130% capacity, it's the same mistake you flagged in Sofia's row.
4. **Write the internal comms.** One paragraph each for: Priya, whose squad
   is being folded; Sofia, whose scope is being split; and the
   partner-success director, who loses the Internal Tools intake queue.
   These are the conversations the plan will actually be judged by.
5. **Pre-mortem it.** It's twelve months later and the plan failed. Write
   the three most likely causes and, for the most likely one, the leading
   indicator you'd watch for in month two.
6. **Take it to a real reviewer.** Give it to your manager or a peer Lead
   with one instruction: find the number I can't defend. There is always
   one, and finding it in a rehearsal is much cheaper than finding it in the
   planning round.

Completing this project means you're ready for **Level 3 · Advanced**.
