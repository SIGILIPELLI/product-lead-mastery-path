# Product Leadership in Turnarounds

Eighteen months into Amara's CPO role, Meridian's biggest customer segment
softens as a competitor undercuts pricing, growth stalls, and the board
tells Lena to cut costs by 20% this quarter — with product headcount the
largest lever available. This is not a portfolio reallocation (Level 3
Module 2, moving capacity between healthy bets); it's a turnaround, where
the organization itself is under threat and morale, trust, and runway are
all simultaneously at risk. Turnaround leadership requires a different
posture than growth leadership: less "which bet gets more," more "what do
we protect no matter what, and what do we let go of even though it hurts."

## Growth leadership vs. turnaround leadership

| Dimension | Growth mode | Turnaround mode |
|---|---|---|
| Default answer to "should we invest" | Yes, if the case is good | No, unless the case is exceptional |
| Communication cadence | Quarterly is often enough | Weekly, sometimes daily during acute phases |
| What earns trust | Vision and ambition | Candor and predictability |
| Risk tolerance on bets | High on 1-2 growth bets | Near-zero on new bets; protect what's proven |
| Leader's emotional job | Inspire toward upside | Absorb anxiety, project calm without denial |

## The triage framework

When capacity must shrink, Amara doesn't cut evenly across pods (which
protects nothing well) or cut the newest bets by default (which sometimes
kills the thing closest to proving out). She triages every initiative
against two axes:

| | Proven revenue/retention impact | Unproven / speculative |
|---|---|---|
| **Protect at current level** | Core Carrier Ops, Marketplace (past its threshold, Level 3 Module 2) | — |
| **Cut or pause** | — | Internal Tools' newer forecasting features, AI-pricing exploration (Level 4 Module 7, paused not killed) |

The distinction between "cut" and "pause" matters enormously for morale and
for future optionality — a paused bet has a stated resume condition; a cut
bet is closed and its people are reassigned or, if unavoidable, part of the
layoff.

## Verifying the cut is actually 20%

```python
python3 -c "
eng_total = 46
target_cut_pct = 0.20
target_cut_hc = round(eng_total * target_cut_pct)
remaining = eng_total - target_cut_hc
print('total:', eng_total, 'target cut:', target_cut_hc, 'remaining:', remaining)

# Proposed cuts by initiative
cuts = {'Internal Tools forecasting': 3, 'AI-pricing exploration (paused)': 4, 'Platform tax reduction': 2}
total_cut = sum(cuts.values())
print('proposed cut total:', total_cut, 'vs target:', target_cut_hc)
print('shortfall/excess:', total_cut - target_cut_hc)
"
```

At 46 total headcount, a 20% cut targets 9 people. The proposed
combination (3+4+2=9) matches exactly — a coincidence Amara doesn't rely
on; she builds the list to hit the number deliberately rather than backing
into it, and always checks arithmetic before it reaches the board or
affected employees, since a target that's off by even one person becomes a
credibility problem in a moment when credibility is the scarcest resource.

## Communicating a turnaround: the candor test

Every turnaround communication gets run through one test before it goes
out: **if this turns out to be wrong in three months, will people say I was
honestly wrong, or that I was managing them?** The second reads as
manipulation in hindsight and destroys trust for years after the crisis
passes.

| Message | Fails the test | Passes the test |
|---|---|---|
| On the cuts | "This positions us for exciting growth ahead" (if you don't actually know that) | "This protects our core business through a harder market; I can't promise growth timing, only that we're not cutting the things customers depend on" |
| On job losses | Vague euphemism, delayed disclosure | Direct, timely, with real support details, delivered by the person with the actual decision authority |
| On what's next | Silence until things improve | Regular, even repetitive, honest updates — "still the same plan, still tracking" is a valid and needed update |

## Worked example: keeping Tom's platform team intact

Amara's hardest internal argument during the cut is protecting Tom's
Platform team (Level 3 Module 8) from a proportional cut. The instinct
from finance is "every team takes 20%." Amara's counter-argument, made
directly to Lena: platform headcount is a multiplier on every remaining
product team's velocity — cutting it proportionally makes the recovery
slower for every surviving initiative, the opposite of what a turnaround
needs. She protects Platform at a 10% cut and takes the other 10%
disproportionately from paused/speculative work instead, and states this
tradeoff explicitly in her communication to the org rather than letting
people infer favoritism.

## Exercise

Imagine (or recall) a scenario where your team or org must cut capacity by
a defined percentage. Triage your current initiatives on the proven-impact
vs. speculative axis, verify your proposed cut list sums to the actual
target with real arithmetic, and draft the one paragraph you'd use to
communicate it — then run that paragraph through the three-month candor
test yourself.
