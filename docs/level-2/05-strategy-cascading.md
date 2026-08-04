# Product Strategy Cascading

Somewhere between the exec offsite and your PM's sprint board, strategy
usually dies. The deck said "become the default system of record for
mid-market carriers." The sprint board says "add CSV export." Nobody lied
and nobody was lazy — the translation just never happened, because
translating is a job and everybody assumed it was somebody else's.

That job is yours. You are the layer where a company-level bet becomes a
set of team-level problems with metrics attached, and where the reality of
what teams learn travels back up before the bet quietly fails. Cascading is
not forwarding. Forwarding takes ten seconds and produces four
interpretations; cascading takes a week and produces one.

## The four-layer cascade

Every layer must be *derivable* from the one above it and *falsifiable* on
its own. If you can't point at a layer and say what evidence would prove it
wrong, it's a slogan.

| Layer | Owner | Horizon | Form it takes | Failure mode |
|---|---|---|---|---|
| Company bet | CEO / exec team | 1-3 years | "Mid-market carriers become our primary segment" | Stated once, never re-stated |
| Product strategy | You (Product Lead) | 2-4 quarters | The 2-3 problems that must be solved for the bet to work | A feature list wearing a strategy costume |
| Squad goal | PM, with you | 1 quarter | One outcome metric with a start value and a target | The goal is an output ("ship the portal") |
| Bets on the board | PM + squad | 1-6 weeks | Specific work, each traceable upward | Work that traces to nothing, unnoticed |

The test that catches most breakage: pick any item on any sprint board and
walk it up three layers out loud. "This CSV export exists because
onboarding takes 14 days, which matters because mid-market carriers churn
during onboarding, which is the bet." If the walk-up breaks, you've found
either a mis-sequenced item or a missing strategy layer — and it's more
often the second.

## The cascade one-pager

One page per squad, written by you and the PM together, refreshed at the
start of each quarter. This is the artefact; the meeting is not.

| Section | Bad version | Good version |
|---|---|---|
| The bet, in the exec's own words | "Grow revenue" | "Mid-market carriers become our primary segment by FY26" |
| Why this squad matters to it | "Onboarding is important" | "Mid-market carriers churn 3× in the first 30 days; onboarding is where they churn" |
| The problem we own | "Improve the onboarding flow" | "A carrier waits 14 days to move their first load" |
| Outcome metric, start, target, date | "Faster onboarding" | "Median time-to-live: 14d → 7d by 31 March" |
| What we will *not* do | (blank) | "No enterprise SSO work; no self-serve billing" |
| Evidence this is the right problem | "Leadership asked" | "22 of 31 churned accounts never completed data migration" |
| What would make us wrong | (blank) | "If time-to-live halves and 30-day churn doesn't move, the problem is elsewhere" |

The last two rows convert a cascade from compliance into thinking. A squad
that has written down what would prove it wrong will tell you when it
happens. A squad that hasn't will defend the roadmap instead.

## Cascade quality checks

Run these before you let a quarter start. Each takes minutes, and each has
saved somebody a quarter.

| Check | How to run it | What a fail looks like |
|---|---|---|
| **Walk-up** | Pick 3 random board items, trace each to the bet | An item traces to "a stakeholder asked" |
| **Uniqueness** | Do any two squads share an outcome metric? | Two squads both own "activation rate" — so nobody owns it |
| **Sum test** | If every squad hits its target, does the bet advance enough? | All targets hit, bet unmoved: the strategy layer is wrong |
| **Non-goal test** | Does each one-pager have a real non-goal? | Non-goals are things nobody wanted to do anyway |
| **Retell test** | Ask an engineer, not the PM, why the squad's work matters | They describe the feature, not the problem |
| **Constraint honesty** | Does any target depend on a team that hasn't agreed? | The dependency owner first hears about it in week 4 |

The retell test is the cheapest and the most brutal. Cascading has worked
when the person furthest from the offsite can state the causal chain
unprompted.

## Cascading back up: the return path

A cascade with no return path is a broadcast. Teams learn things that
should change the strategy, and that information has to travel — but not as
raw noise, or executives learn to tune you out.

| Signal from a squad | What it means upward | How to frame it to leadership |
|---|---|---|
| Metric moves, bet doesn't | The causal assumption is wrong | "Time-to-live halved; 30-day churn is flat. The churn driver isn't onboarding speed. Here's what the data now points at." |
| Metric won't move despite good work | The problem is bigger than one squad | "Three quarters of squad-level effort moved this 8%. Moving it 40% needs a platform change we haven't funded." |
| Squad keeps getting pulled off-plan | The stated strategy isn't the real one | "The roadmap says mid-market; 40% of engineering weeks went to two enterprise accounts. Which is the actual priority?" |
| Falsifier triggered | The agreed disproof happened | "We wrote down in January what would make us wrong. It happened. I'm proposing we stop." |

The falsifier row is why you write it in advance. Killing a bet is a
political act when you argue it in the moment and an administrative one
when the criteria were agreed before anyone was invested.

## Worked example: cascading Meridian's segment shift

Meridian Logistics' CEO commits to mid-market carriers as the primary
segment. Amara has four squads and a deck with three bullet points on it.

**Step 1 — she does not forward the deck.** She spends two hours turning
the bet into a product strategy: three problems, in priority order.
(1) Mid-market carriers churn in the first 30 days, concentrated in data
migration. (2) They can't price lanes without a spreadsheet analyst they
don't employ. (3) Their partner integrations break silently and Meridian
gets blamed. Each problem carries evidence — 22 of 31 churned accounts
never completed migration; 11 of 14 pricing interviews named the analyst
gap.

**Step 2 — she checks coverage before assigning.** Problems 1 and 2 map
cleanly to Onboarding (Ravi) and Pricing (Sofia). Problem 3 maps to
Integrations (Tom). Internal Tools (Priya) maps to nothing. That's the
uncomfortable finding, and the cascade surfaced it in hour two rather than
month three. Amara doesn't disband the squad; she rescopes it to
support-side onboarding tooling — genuinely under problem 1 — and writes
down that if it can't earn a place under a strategy problem by Q3, it gets
folded.

**Step 3 — one-pagers written *with* each PM, not for them.** Sofia's draft
has the outcome metric as "ship pricing tool to 3 pilots." Amara pushes
back: that's an output. It becomes "3 pilot customers pricing lanes without
spreadsheet support, measured by zero analyst tickets from those accounts
across a 30-day window." Sofia resists — it's harder to hit and it depends
on customer behaviour. That resistance is the moment the goal became real.

**Step 4 — the sum test fails, and she's glad it failed early.** All four
targets hit would reduce 30-day churn by roughly 9 points on her modelling.
The company bet needs 20. She takes this to the CEO in week 2 as
arithmetic, not a complaint: either the bet needs a fourth workstream
(sales-side qualification, which isn't a product problem), or 20 points is
a two-year target, not a one-year one. The CEO picks the second. That
re-statement is worth more to Amara's PMs than any amount of motivational
framing, because it makes their goals both achievable and honest.

**Step 5 — the retell test in week 6.** She asks an Onboarding engineer why
the data-migration work matters. He says: "Because mid-market carriers give
up during migration and we lose them in month one." Cascade landed. She
asks a Pricing engineer the same question. He says: "Because it's on
Sofia's Q1 roadmap." Cascade did not land there — so she asks Sofia to open
the next sprint review with the two customer quotes instead of the burndown
chart.

**Step 6 — the return path fires in April.** Ravi's squad gets time-to-live
from 14 days to 6. Thirty-day churn moves 2 points, not the 8 modelled. The
January falsifier said exactly this would mean the churn driver isn't
onboarding speed. Amara brings it to the exec review as agreed evidence
rather than bad news, with the follow-up analysis: churn is now
concentrated in accounts whose first month included an integration failure
— which promotes Tom's problem 3 from third place to first for Q3.

## Cheat sheet

| Trap | Correction |
|---|---|
| Forwarding the strategy deck | Write the 2-3 problems layer yourself; that *is* the job |
| Squad goals that are outputs | Metric, start value, target, date — or it isn't a goal |
| Two squads owning one metric | Split the metric or merge the squads |
| An empty non-goal row | Nothing was actually prioritised; go back |
| Finding an orphan squad in month three | Run the coverage check in hour two |
| Arguing to kill a bet in the moment | Agree the falsifier in writing before the quarter starts |
| Cascade "communicated" via all-hands | Test it with the retell test on someone who wasn't in the room |
| Raw team noise sent upward | Frame upward signals as evidence plus a proposed decision |

## Exercise

Take your real company strategy (or a realistic one) and 3-4 squads.

1. Write the product-strategy layer: the 2-3 problems that must be solved
   for the company bet to work, each with one line of existing evidence. If
   you can't produce evidence for a problem, label it "assumed" — and make
   validating it someone's first task.
2. Run the coverage check. List each squad against a problem. Name every
   squad that maps to nothing, and write what you'd do about it, with a date.
3. Write the full cascade one-pager for one squad, including a genuine
   non-goal and a falsifier you would actually honour.
4. Run the sum test with real arithmetic: if every squad hits its target,
   how far does the company bet actually move? Write the sentence you'd say
   to your CEO if the answer is "not far enough."
5. This week, run the retell test on two engineers from different squads.
   Write down their exact words. The gap between what they said and the
   one-pager is the size of your cascade problem.
