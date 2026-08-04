# Managing Multiple Product Squads

One squad is a job you can do by being present. Three or four squads is a
job you can only do by *allocating* presence — deliberately, unevenly, and
with a written rationale. The failure mode is predictable: you drift toward
the squad that is loudest, most interesting, or closest to your old area,
and one quiet squad starves for six weeks before anyone notices.

This module gives you an attention model, a portfolio view, and early-warning
signals that tell you a squad is in trouble before its metrics do.

## The attention allocation model

Your leadership time is a portfolio, not a fairness exercise. Equal time
across squads is almost always wrong. Rate each squad monthly on two axes:

- **Stakes** — how much does the company outcome this quarter depend on this
  squad succeeding?
- **Self-sufficiency** — how reliably does this squad make good decisions
  without you in the room?

| Stakes ↓ / Self-sufficiency → | High self-sufficiency | Low self-sufficiency |
|---|---|---|
| **High stakes** | *Monitor closely, intervene rarely* — weekly written check, join reviews, keep your hands off the decisions | *Your main investment* — 40-50% of your squad time; sit in discovery, review artefacts, pair on hard calls |
| **Low stakes** | *Leave alone* — monthly check-in, stay reachable, resist the urge to add value | *Coach or restructure* — the PM needs development or the squad needs a different setup; decide which, don't drift |

Rules that follow:

1. No squad gets zero. The floor is a monthly 30-minute review plus a read of
   their written update. That's your starvation insurance.
2. Reassess monthly, not quarterly. Self-sufficiency moves fast when a PM is
   new; stakes move fast when strategy shifts.
3. Publish the allocation to your PMs. A PM in the "leave alone" cell should
   know they're there *because they earned it*, not wonder whether you've
   lost interest in their squad.

## The squad portfolio table

Keep one table for all squads, refreshed monthly. This is the artefact that
makes multi-squad leadership legible — to you, to your manager, and to your
PMs.

| Squad | PM | Mission (1 line) | Quarter goal + metric | Stakes | Self-suff. | My time | Top risk | Dependency owed / owing |
|---|---|---|---|---|---|---|---|---|
| Onboarding | Ravi | Get new carriers live in under 7 days | Median time-to-live 14d → 7d | High | Med | 40% | Data-migration tooling unscoped | Owes API contract to Integrations |
| Pricing | Sofia | Let ops price lanes without spreadsheets | 3 pilot customers live | High | High | 20% | Pilot customers not yet signed | Needs design capacity |
| Integrations | Tom | Keep partner APIs boring and reliable | P1 incidents 6/qtr → 2/qtr | Med | High | 10% | Partner deprecating v1 API | Owed API contract from Onboarding |
| Internal Tools | Priya (new) | Cut support handle time | Handle time −20% | Low | Low | 30% | New PM, no baseline data yet | None |

Two things this table catches that nothing else does: a dependency listed by
one squad with no matching entry on the other side (a silent collision), and
a squad whose stakes are High while your time on it is 10%.

## Early-warning signals per squad

Metrics tell you a squad is in trouble one to two months after it happened.
These signals tell you in one to two weeks.

| Signal | What you observe | Likely cause | First move |
|---|---|---|---|
| **Roadmap goes vague** | Next-quarter items titled "platform improvements" | The PM has lost the thread on why the work matters | Ask them to state the customer problem for each item, out loud, in the next 1:1 |
| **Discovery stops** | No customer conversations logged for 3+ weeks | Squad has slipped into pure delivery mode | Reinstate a fixed weekly discovery slot; attend it once |
| **The eng lead answers product questions** | In reviews, the PM defers on scope calls | The PM isn't earning decision credibility | Coach the PM on preparation; privately ask the eng lead to redirect |
| **Estimates slip by the same ratio every time** | Everything runs 1.5× over | Systematic scoping gap, not bad luck | Review the last five items together and find the missing category — migration? QA? rollout? |
| **The PM stops escalating** | Everything is "fine" for weeks | Either genuinely fine, or trouble being hidden | Ask for their top two risks by name; a PM with none is a signal, not a comfort |
| **Cross-squad meetings get skipped** | The squad stops attending the sync | They see no value — usually because there is none | Fix the sync's agenda or kill it; don't just mandate attendance |

## Designing your multi-squad ritual stack

Running four squads with four separate ritual sets means 4× the meetings and
zero shared context. Collapse instead.

| Ritual | Cadence | Attendees | Output it must produce | What it replaces |
|---|---|---|---|---|
| Written squad update | Weekly, async | Each PM writes; you read all | Five lines: shipped, next, risk, decision needed, metric move | Four separate status meetings |
| Portfolio review | Monthly, 60 min | You + all PMs | Refreshed portfolio table and reallocated attention | Ad hoc "how's it going" checks |
| Dependency sync | Biweekly, 30 min | PMs + eng leads | Updated dependency log with dates and owners | Cross-team surprises |
| Squad deep-dive | Weekly, rotating | You + one squad | Real decisions on that squad's hardest open call | Attending every squad's review shallowly |
| PM 1:1 | Weekly, 45 min | You + one PM | Growth, feedback, blockers — explicitly not status | Status conversations disguised as 1:1s |

The rotating deep-dive is the key move. Attending all four squads' reviews
every week gives each squad 25% of a distracted you. Attending one squad
fully each week gives each squad 100% of an engaged you once a month, and
your calendar stops being the constraint on team size.

## Worked example: rebalancing a four-squad portfolio

Amara at Meridian runs the four squads above. Her January portfolio review
embarrasses her: 55% of her squad time is going to Pricing (High stakes,
High self-sufficiency) and 10% to Internal Tools (Low stakes, Low
self-sufficiency, a PM eight weeks into the job). The honest reason is that
Pricing is the interesting problem and Sofia is fun to work with.

The model says the opposite. Sofia belongs in "monitor closely, intervene
rarely." Priya — new, no baseline data, no working relationship with her eng
lead — is the squad that either gets coached or gets restructured.

The rebalance:

- **Pricing drops to 20%.** Amara tells Sofia exactly why: "You're the most
  self-sufficient PM I have and I've been over-involved because I like this
  problem. I'm moving to a monthly deep-dive and reading your weekly update.
  Escalate anything that crosses a pricing-policy line." Framing it as earned
  autonomy rather than withdrawal is the whole ballgame.
- **Internal Tools goes to 30%, with an end date** — eight weeks, then
  reassess. Open-ended investment in a low-stakes squad is how Leads lose
  their quarters.
- **Onboarding holds at 40%.** High stakes, medium self-sufficiency, and it
  owes a dependency that Integrations is blocked on.
- **Integrations stays at 10%,** and Amara writes down what would change
  that: the partner's v1 deprecation date landing inside the quarter.

Six weeks later the early-warning table earns its keep. Tom's Integrations
squad — the one on 10% — stops attending the biweekly dependency sync. Under
the old regime Amara would have noticed at quarter end. Instead she asks Tom
directly and learns the sync had degenerated into a status readout with no
decisions, so he had rationally opted out. She rebuilds the agenda around
open dependency decisions only, and attendance recovers without a mandate.

## Cheat sheet

| Symptom | Diagnosis to check first |
|---|---|
| One squad feels neglected | Where does it sit on the stakes × self-sufficiency grid, and does your calendar agree? |
| Calendar is full but nothing feels decided | You're attending shallowly everywhere instead of deeply in rotation |
| A cross-squad surprise landed | Was the dependency listed on *both* sides of the portfolio table? |
| A PM has gone quiet | Ask for their top two risks by name |
| You're 55% on your favourite squad | You are, and you know it — rebalance with a written rationale |
| A heavy coaching push has no end date | Set one now, or it becomes your permanent job |

## Exercise

Build the portfolio table for your own squads (or a realistic set of 3-4).
Fill every column honestly, including your *actual* time split over the last
month — estimate it from your calendar, not from memory.

1. Plot each squad on the stakes × self-sufficiency grid. Circle any squad
   where your actual time contradicts the cell it lands in.
2. Write the rebalanced allocation with a one-sentence rationale per squad,
   and an end date on any squad whose share you're increasing.
3. Write the exact sentence you'd say to the PM whose allocation you're
   *reducing*, framed as earned autonomy rather than withdrawal.
4. Scan the dependency column for any entry that appears on one squad's row
   but not the matching squad's row. That asymmetry is your most likely
   quarter-end surprise — go confirm it this week.
