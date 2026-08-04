# Advanced Product Team Leadership

At Level 1 you learned to lead a team when the direction was reasonably
clear. Level 2 starts where that breaks: a reorg lands mid-quarter, two of
your PMs both need the same engineering squad, your best PM gets an offer
elsewhere, and the strategy you cascaded eight weeks ago is now half wrong.
Advanced team leadership is mostly about **operating well when the inputs
are unstable** — and doing it at a team size where you can no longer be in
every room.

## The four conditions you lead through

Most Product Leads have one default leadership style. That style works in
exactly one of the four conditions below and quietly fails in the other
three. Diagnose the condition first, then pick the behaviour.

| Condition | What it feels like on the team | What the team actually needs | Your dominant behaviour |
|---|---|---|---|
| **Fog** — direction unclear, no crisis | "We're busy but I can't tell if any of it matters" | A decision, even a provisional one, plus an explicit review date | Decide out loud: "We're betting on X for six weeks; we revisit on the 15th" |
| **Storm** — clear direction, acute pressure (outage, churn spike, hard deadline) | Everyone reacting, PMs pulled into firefighting | One owner, a scoped-down goal, and air cover from noise | Narrow scope, name the single owner, absorb stakeholder traffic yourself |
| **Drift** — things are fine, standards slipping | Meetings feel routine, quality dips nobody mentions | A raised bar with a concrete example attached | Point at one specific artefact and say what "good" looks like |
| **Grind** — direction clear, work is long and unglamorous | Motivation fading on a two-quarter migration | Visible progress markers and public credit | Break into milestones, celebrate each one specifically |

The classic failure is applying Storm behaviour (take over, scope down,
direct) to a Fog problem — you produce urgency without direction — or
applying Fog behaviour (more discovery, more discussion) during a Storm.

## Ambiguity triage: what you resolve vs. what you hand down

You cannot resolve every open question, and you shouldn't. Run each piece of
ambiguity that lands on you through this test.

| Question about the ambiguity | If YES | If NO |
|---|---|---|
| Does resolving it need information only you can get (exec context, budget, other teams' plans)? | You resolve it | Push it down |
| Would two PMs resolve it in contradictory ways that then collide? | You resolve it | Push it down |
| Is it reversible within a sprint? | Push it down, ask to be told the call | You resolve it |
| Does it change who owns what? | You resolve it | Push it down |

When you push ambiguity down, hand it down *with the constraints attached*:
"You own this call. Constraints: must ship before the March renewal cycle,
can't add a new vendor, no more than two engineers on it. Tell me what you
decided, not what the options are."

## Arbitrating competing priorities between your PMs

The most common Level 2 escalation is two PMs wanting the same scarce
resource — a squad, a designer, a data analyst, your time. Do not resolve it
by seniority, volume, or who asked first. Write it down:

| Field | What you write |
|---|---|
| The contested resource | "Platform squad, sprints 14-17" |
| Claim A | PM, initiative, the company goal it serves, cost of a four-week delay |
| Claim B | Same fields |
| Reversibility | Which claim can be delayed and later recovered; which has a hard external date |
| Decision | Who gets it, for how long |
| Compensation | The concrete thing the deprioritised PM receives — earlier slot next quarter, a contractor, scope relief elsewhere |
| Review date | When you revisit — required, not optional |

The compensation row is what stops arbitration from breeding resentment. A
PM who loses a resource fight and gets nothing learns to escalate louder
next time. A PM who loses and gets a named alternative learns the process is
fair.

## Habits that break as the team grows

Every leadership habit has a team size at which it stops working. Knowing
the breakpoint in advance is what separates a Lead who scales from one who
drowns at eight reports.

| Habit | Works at | Breaks at | Replacement |
|---|---|---|---|
| Reading every spec before it ships | 2-3 PMs | 4+ | Read specs only for irreversible-decision work; sample two per month at random |
| Attending every squad's sprint review | 2-3 squads | 4+ | Rotate: one squad per week, on a published schedule so it isn't read as favouritism |
| Being the single point of stakeholder contact | 3 PMs | 4+ | Publish which PM owns which stakeholder relationship; introduce them explicitly |
| Weekly 60-min 1:1 with everyone | ~6 reports | 7+ | 45 min weekly for direct PMs, 30 min biweekly for skip-levels, plus a written status channel |
| Holding priorities in your head | 3 initiatives | 6+ | One written priority stack with numbered ranks, refreshed monthly |
| Giving feedback whenever you happen to notice things | Small team | 5+ reports | Fixed feedback slots — one specific SBI item per PM per month, tracked |

## Worked example: a mid-quarter strategy change

Meridian Logistics, a 320-person B2B SaaS, sells route-planning software.
Amara leads product with four PMs across three squads. In week 6 of the
quarter the CEO announces that mid-market carriers are now the sole growth
priority and the enterprise motion is being de-emphasised. Two of Amara's
four PMs have quarterly goals built entirely on enterprise features.

What Amara does *not* do: forward the email and ask the team to "re-look at
priorities." That produces four interpretations and a month of churn.

What she does, in order:

1. **Names the condition.** This is Fog, not Storm — nothing is on fire, the
   direction is newly unclear. Her job is a provisional decision, fast, not
   a firefight.
2. **Resolves the ambiguity only she can resolve.** Thirty minutes with the
   CEO and CRO gets her three answers her PMs could not have obtained:
   signed enterprise commitments are still honoured; no headcount moves this
   quarter; the segment shift is a 12-month bet, not a six-week experiment.
3. **Rewrites the priority stack herself** — ranks 1 to 6, one page, with
   the two enterprise initiatives explicitly at ranks 5 and 6 rather than
   deleted. Deleting them would signal that six weeks of work was wasted;
   ranking them low signals sequencing.
4. **Runs the arbitration.** Both mid-market initiatives now want the
   platform squad. Ravi's carrier-onboarding rework wins sprints 14-17
   because it gates a contractual go-live date. Sofia's pricing tooling is
   deferred but gets a named contractor for six weeks, first claim on the
   squad in Q3, and a review date of 20 March, written down.
5. **Handles the human half separately.** Sofia's quarterly goals were 80%
   enterprise. Amara rewrites those goals *with* her before the review cycle
   so Sofia isn't graded against a plan the company cancelled. (See Module 3
   — changing the goal and changing the rating are two different
   conversations, and conflating them is how you lose good people.)
6. **Keeps the review date.** On 20 March she reopens the arbitration in a
   20-minute meeting — not as ceremony, but because that promise is the only
   reason Sofia accepted the outcome.

Elapsed time from announcement to a written, ranked, arbitrated plan: nine
days. The number that matters isn't nine — it's that her PMs spent those
nine days executing on rank 1-4 work rather than speculating in Slack.

## Cheat sheet

| Situation | First question to ask yourself |
|---|---|
| New ambiguity lands | Fog, Storm, Drift, or Grind? |
| A PM escalates a decision | Do I have information they don't? If not, hand it back with constraints |
| Two PMs want the same resource | What does the loser get, and when do we revisit? |
| You feel overwhelmed | Which habit have I outgrown at this team size? |
| Strategy changes mid-cycle | Re-rank rather than delete; separate goal changes from performance judgements |
| You're in every meeting | Which of these am I attending out of habit rather than leverage? |

## Exercise

Take your own team (or a realistic one of 4+ PMs across 3 squads).

1. Write the single biggest source of ambiguity your team faces right now,
   in one sentence. Run it through the triage table — do you resolve it or
   hand it down? Write the exact sentence you'd say either way, including
   the constraints if you're handing it down.
2. Identify one real or plausible resource conflict between two of your
   people and fill in the whole arbitration table — including the
   compensation row and a specific review date. If you can't name a
   compensation, your decision isn't finished.
3. Go through the "habits that break" table and mark every habit you're
   still running past its breakpoint. Pick one and write the replacement
   you'll adopt this month, with the specific cadence.
