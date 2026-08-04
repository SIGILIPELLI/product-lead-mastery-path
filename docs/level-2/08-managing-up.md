# Managing Up

Managing up has a reputation problem: it sounds like politics, so competent
people avoid it and then wonder why their team's work keeps getting
reprioritised by someone who doesn't understand it. The actual definition is
duller and more useful — managing up is making it easy for the people above
you to make good decisions about your area, and making sure the information
they act on is accurate.

You are the only person who can do this for your squads. Your PMs don't have
the exec relationships; your executives don't have the ground truth. If you
don't translate in both directions, decisions about your team get made on
whatever fragment reached the room — usually the loudest customer escalation
of that week. This module covers what executives actually need from you, how
to frame trade-offs so a decision is possible, how to deliver bad news, and
how to run the relationship with your own manager deliberately.

## What executives actually need

Most updates fail because they're written for the writer — a record of
effort — rather than for the reader, who needs to decide something or needs
not to worry.

| They need | Why | What that means in practice |
|---|---|---|
| The headline first | They read the first two lines and skim the rest | Conclusion in sentence one, evidence after |
| To know if anything requires them | Their scarce resource is decisions, not attention | Label every item: FYI, or Decision needed by [date] |
| Predictability over optimism | They plan other things around your dates | A confidently-held slipped date beats a cheerfully-missed one |
| No surprises, ever | Being blindsided in front of *their* boss is the trust-killer | Bad news travels up within 24 hours, from you |
| Trade-offs, not requests | "More headcount" isn't decidable; "A or B" is | Always present options with consequences |
| Your recommendation | They're paying for judgement, not a menu | Name your pick and why, then be genuinely open |

## The weekly upward update

Six lines, same shape every week. The consistency is the feature — it lets
your manager scan for the delta rather than re-reading the format.

| Line | Content | Meridian example |
|---|---|---|
| Headline | The one thing to know | "Onboarding is on track for the 7-day target; pricing pilot slips two weeks" |
| Metrics | Number, direction, vs. target | "Time-to-live 11d (from 14, target 7). P1 incidents 4/qtr (target 2)" |
| Shipped | What actually landed | "Field-mapping validation live for all new carriers" |
| Risks | Named, with owner and mitigation | "Data-migration tooling unscoped — Ravi + Platform, scoping doc by Friday" |
| Decisions needed | What you need from *them*, with a date | "Approve contractor spend for pricing (£18k, 6 weeks) — need answer by 12 Feb" |
| Watching | Early signals, not yet risks | "Partner v1 deprecation date may land inside Q2" |

The "Decisions needed" line is the one that changes your working life. A
manager who sees a dated, specific ask every week starts responding to them;
a manager who receives narrative updates learns that nothing is required.

## Framing a trade-off so a decision can happen

Executives don't decline requests because they're hostile. They decline
because the request has no visible shape.

| Framing | Example | What it produces |
|---|---|---|
| Request (weak) | "We need another engineer on pricing" | Deferral, or a debate about headcount policy |
| Complaint (worse) | "We're under-resourced" | Sympathy, no decision |
| **Trade-off (strong)** | "Pricing pilot lands in March with current staffing, or February if we move two engineers off Integrations — which costs us the v1 migration buffer. I recommend March; the deprecation risk is the bigger exposure." | An actual decision, in one meeting |

The structure: **option A with its cost, option B with its cost, your
recommendation, and the one fact that decides it.** Two options, not five.
Five options is a research report; two is a decision.

## Delivering bad news

| Rule | Detail |
|---|---|
| Within 24 hours | Speed is the entire signal; a late accurate report reads as concealment |
| From you, first | If they hear it from sales or from their own boss, you've spent trust you can't quickly re-earn |
| Lead with the impact | "The pricing pilot slips to March" — not three paragraphs of causal build-up |
| Then the cause, briefly | One or two sentences, mechanical, no blame allocation |
| Then what you've already done | Shows the situation is being managed, not just reported |
| Then what you need | Decision, cover, or nothing — say which |
| Never bundle it with good news | Sandwiching reads as spin and devalues the good news too |

A usable four-sentence template: *"The pricing pilot moves from February to
March. The cause is the customer's data warehouse migration, which we didn't
know about at planning. I've re-sequenced the squad onto the analytics work
that was queued for Q2, so we don't lose the weeks, and I've moved the pilot
customer's expectations myself. I don't need anything from you, but you'll
want this before Thursday's board prep."*

## Running the relationship with your manager

This is a working relationship with mechanics, and most people leave all of
them to chance.

| Mechanic | What to do | Why |
|---|---|---|
| Ask how they want to be updated | Explicitly: format, cadence, what they want escalated | Half of "communication problems" are format mismatches |
| Establish an escalation threshold | Agree the size of thing they want to hear about immediately | Otherwise you'll over- or under-escalate for a year |
| Bring one thing you got wrong per month | Voluntarily, with what you changed | Cheapest trust-building move available |
| Ask what they're being asked about you | Once a quarter | Surfaces problems while they're still small |
| Know their pressures | What is *their* manager measuring them on? | You can serve a goal you know about |
| Disagree in private, commit in public | And say so explicitly: "I'd have chosen B; we're doing A and I'm behind it" | Protects your credibility and theirs |
| Never let them be surprised in a room | Pre-brief before any meeting where something contentious will surface | This is the single highest-value habit here |

Skip-levels deserve a note of their own. Your skip-level talking to your PMs
is healthy, not a threat — the failure is only if you're surprised by what
they learn. Brief your manager *and* your skip-level on the same facts, and
never let your PMs be the channel for information you should have delivered.

## Worked example: the contractor ask and the slipped pilot

Amara needs £18k of contractor budget to keep the pricing pilot on track,
and separately she has just learned the pilot will slip regardless. Two
different conversations, deliberately not merged.

**The bad news, Tuesday, within four hours of learning it.** She messages
her VP directly: pilot moves February → March; cause is the pilot customer's
own warehouse migration, discovered in a call that morning; she has already
re-sequenced Sofia's squad onto queued analytics work so the weeks aren't
wasted and has reset the customer's expectations herself; nothing needed
from the VP, but he has board prep on Thursday and should not learn this
there. Total: five sentences, sent before the VP's Thursday.

**The ask, Thursday, framed as a trade-off.** Amara has learned that her VP
declines resource requests and decides trade-offs, so she writes it as two
options. Option A: hold current staffing, pricing goes to three pilot
customers in March, Integrations keeps its v1 migration buffer. Option B:
£18k contractor for six weeks, pricing reaches five pilot customers in March
and generates enough evidence to decide the FY26 pricing bet a quarter
earlier. Her recommendation is B, with the deciding fact stated plainly: the
FY26 pricing decision is scheduled for July, and three customers won't be
enough evidence to make it — so the £18k buys a decision, not a feature.

The VP approves in the meeting. What made it approvable wasn't the money; it
was that the cost of *not* spending it was expressed as a decision the VP
himself would have to make badly in July.

**The pre-brief that mattered more.** Two weeks later the CRO raises the
pilot slip in an exec meeting, framing it as a product-team delivery
problem. Because Amara had sent the note in February, her VP already had the
cause and the mitigation and answered it in the room without her present.
That is the entire return on managing up: your work gets defended accurately
when you aren't there.

**The counter-example, six weeks on.** Amara disagrees with a decision to
move Integrations under a different Lead. She argues it hard in her 1:1 —
with the dependency data — and loses. In the team meeting she says: "I
argued for keeping Integrations with us and I didn't win the argument. Here
is the reasoning behind the decision, and here's how we'll make the handover
work." Her PMs know she fought; they also know the matter is closed. Both
halves are necessary; leaders who only do the first are unmanageable, and
leaders who only do the second are not trusted by their teams.

## Cheat sheet

| Trap | Correction |
|---|---|
| Narrative updates with no ask | Every update carries a dated "decisions needed" line, or explicitly says "none" |
| Requesting resources | Present two options with costs, plus your recommendation |
| Five options | Two. Five is a research report, not a decision |
| Delaying bad news to have a fix ready | 24 hours, with what you've done so far |
| Sandwiching bad news with good | Never; it reads as spin and devalues both |
| Guessing your manager's preferred format | Ask directly, once, and then honour it |
| Being surprised by your skip-level | Brief both on the same facts |
| Public disagreement after a decision | Disagree in private, commit in public, and say you did |
| Never admitting a mistake upward | One voluntary "I got this wrong" per month buys more trust than any win |

## Exercise

Use your real manager and your real current situation.

1. Write this week's six-line update in the exact table format above. If the
   "decisions needed" line is empty, check whether that's true or whether
   you've been absorbing decisions you shouldn't be.
2. Take a resource or priority request you're currently sitting on. Rewrite
   it as a two-option trade-off with costs, your recommendation, and the one
   fact that should decide it.
3. Write the four-sentence bad-news note for the worst thing currently true
   about your area. Notice how long you've been sitting on it, and send it.
4. List what your manager's manager measures *them* on. If you can't, that's
   your next 1:1 question.
5. Book the pre-brief for the next meeting where something contentious about
   your team will come up. That one habit outperforms everything else here.
