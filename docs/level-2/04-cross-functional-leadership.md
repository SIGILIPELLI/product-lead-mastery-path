# Cross-Functional Leadership

At Level 1, engineering and design were stakeholders you aligned with. At
Level 2 they are *peers* — an engineering manager and a design lead with
their own headcount, their own quarterly commitments, their own manager, and
their own view of what your team should be doing. You have no authority over
them, and they have none over you, which means every disagreement escalates
to a shared boss unless the three of you have built machinery to resolve it
yourselves.

That machinery is what this module builds: a decision-rights map that covers
all three functions, an escalation ladder, and a way to run conflict that
doesn't leave scar tissue.

## The tri-functional decision-rights map

Level 1 taught you to map decisions inside your product team. This version
maps them across the leadership trio. Fill it in *with* your eng and design
counterparts, in one 90-minute session — writing it alone and circulating it
is how you get polite agreement and zero adherence.

| Decision | Product | Engineering | Design | Notes |
|---|---|---|---|---|
| What problem we solve next quarter | **Decide** | Consult | Consult | Product owns the why; both functions get a real veto window before it's locked |
| Whether a solution is good enough to ship | Consult | Consult | **Decide** | Design owns quality bar for user-facing surfaces |
| Technical approach and architecture | Consult | **Decide** | Inform | Product may state constraints (time, cost), never the approach |
| Scope cut under deadline pressure | **Decide** | Consult | Consult | Product decides *what* is cut; eng states what cutting costs |
| Whether to take on tech debt now or later | Consult | **Decide** | Inform | With a standing budget — see below |
| Hiring bar and headcount split within the trio | Consult | Consult | Consult | Escalates to shared manager by design |
| Whether the team hits its date | Consult | **Decide** | Inform | Eng owns the estimate; product owns the consequence |
| Research priorities and methods | Consult | Inform | **Decide** | Product supplies the questions, design owns the method |

**Decide** = makes the call and is accountable for it. **Consult** = must be
asked, and their objection must be recorded before the call. **Inform** =
told before it's public.

The two rows that prevent most cross-functional wars: *technical approach*
(product stating constraints, never approach) and *scope cut* (product picks
what goes, engineering costs it). Teams that get those two backwards spend
every quarter re-litigating them.

## The standing tech-debt budget

The single most reliable source of product-engineering conflict is debt
work, because it's negotiated fresh every sprint and the PM wins by default
under deadline pressure. Kill the negotiation with a standing allocation.

| Model | How it works | Best when |
|---|---|---|
| Fixed percentage | 20% of every sprint is eng-directed, no product approval needed | Steady-state teams; simplest to hold |
| Rotating theme | One full sprint in five is eng-directed | Debt items too big for a 20% slice |
| Debt-on-touch | Any surface you build on gets cleaned as part of the story | Legacy areas being actively developed |
| Incident-triggered | Every P1 buys a mandatory follow-up sprint slice | High-incident platforms |

Whichever you pick, the rule is: **the allocation is not renegotiated
mid-quarter.** The Product Lead's job is to defend it upward when a
stakeholder wants the 20% back, which is the single fastest way to earn an
engineering manager's trust.

## The escalation ladder

Most cross-functional conflict is escalated too early (undermining the peer)
or too late (after the damage). Publish the ladder with your counterparts so
escalation stops feeling like betrayal.

| Rung | When | Who's involved | Timebox |
|---|---|---|---|
| 1. PM ↔ EM/designer, direct | Any disagreement, first instance | The two ICs | 48 hours |
| 2. Leads' triad | ICs are stuck, or the disagreement recurs across squads | You + eng manager + design lead | One week |
| 3. Written decision memo | The triad is split and the call is expensive | Triad writes one memo: options, each function's position, recommendation | One week |
| 4. Shared manager | Memo can't converge | Shared boss decides from the memo, not from a debate | Same week |

Rung 3 is what makes rung 4 healthy. Executives asked to arbitrate a live
argument decide based on who is more persuasive in the room. Executives given
a written memo with both positions stated fairly decide based on the
substance — and, importantly, both leads look competent rather than
squabbling.

## Peer-relationship maintenance

Cross-functional trust is built in the boring weeks, not in the crisis.

| Practice | Cadence | Why it works |
|---|---|---|
| Leads' weekly triad, 30 min, no ICs | Weekly | A private room to disagree before disagreeing publicly |
| Shared quarterly goals, not parallel goals | Quarterly | If eng has an uptime goal and product has a ship goal, you're structurally opposed |
| One joint artefact per quarter | Quarterly | Co-authoring a plan makes ownership real; reviewing each other's does not |
| Public credit reassignment | Continuous | Attribute the win to the function that actually drove it, especially when it wasn't yours |
| Pre-brief before any exec meeting | Before each | No lead should ever hear your position for the first time in front of your shared boss |

That last one is close to an absolute rule. The fastest way to destroy a
peer relationship is to surprise an engineering manager in front of the VP.

## Worked example: the re-platform standoff

Meridian's onboarding squad has a hard external date: three enterprise
carriers go live on 1 June, contractually. In February, Karim — the
engineering manager — says the existing onboarding service can't take the
load and wants an eight-week re-platform starting immediately. Ravi, the PM,
says a re-platform makes the June date impossible and pushes back. Two weeks
of trench warfare in sprint planning follow. Ravi asks Amara to "tell Karim
no."

Amara does not tell Karim no. That would settle a technical-approach
decision from the product side — a row Karim owns — and would cost her the
relationship for a year.

Instead:

1. **Rung check.** The disagreement recurred over two weeks at rung 1, so it
   belongs at rung 2. She convenes the triad — herself, Karim, and Jules
   (design) — for one hour.
2. **Separate the two decisions.** She names them explicitly on a whiteboard:
   (a) is a re-platform technically necessary — *Karim decides*; (b) what
   scope ships by 1 June — *she decides*. The fight had been so ugly because
   both people thought they were arguing about one thing.
3. **Convert the technical claim into a costed constraint.** She asks Karim
   the only question a product person should ask about an architecture call:
   "What breaks, when, if we don't?" His answer is specific — at roughly 4×
   current volume, onboarding jobs start timing out, and the three new
   carriers put them at 3.5×. That's not a preference; that's a date-bearing
   risk.
4. **Uses her own decision right.** Given that constraint, she cuts scope:
   two of the six planned onboarding features are dropped from the June
   release, and the re-platform runs in parallel on a narrow critical path —
   the job runner only — rather than the whole service. Karim owns whether
   that narrow path is technically coherent; he says it is.
5. **Writes the memo anyway.** Even though the triad converged, Amara writes
   the one-page decision memo — options considered, each function's position,
   what was decided and why, what would change the decision. When the CRO
   asks in April why two features slipped, the memo answers it in ninety
   seconds without anyone relitigating.
6. **Protects the debt budget.** In April, with June looming, the CRO asks
   to suspend the 20% engineering allocation "just until go-live." Amara
   says no in front of Karim. That single public act does more for the
   product-engineering relationship at Meridian than any offsite.

Outcome: the June date holds with reduced scope, the job runner is
re-platformed, and — the durable part — the next disagreement between Ravi
and Karim gets resolved at rung 1 in a day, because both now know the map.

## Cheat sheet

| Situation | Move |
|---|---|
| Eng wants a re-platform you think is unnecessary | Ask "what breaks, when, if we don't?" — convert opinion into a costed constraint |
| Design says a flow isn't ready to ship | Their call on user-facing quality; your call is what that costs and what gets cut |
| Your PM asks you to overrule the EM | Check the map first — is it even your decision? |
| A stakeholder wants the debt budget back | You defend it upward; that's the job |
| The triad is deadlocked | Write the memo before escalating |
| You're about to present to the VP | Pre-brief your peers; never surprise them in the room |
| A cross-functional win lands | Give the credit to the function that drove it |

## Exercise

With your own team in mind (or a realistic trio setup):

1. Fill in the tri-functional decision-rights map for at least ten decisions
   your team actually faces. Mark any row where you *think* you have Decide
   but your counterpart would disagree — those rows are your agenda for the
   next triad meeting.
2. Pick the tech-debt model you'd run and write the sentence you'd use to
   defend it to an executive asking for it back mid-quarter. Be specific
   about what you'd trade instead.
3. Take one live or recent cross-functional conflict on your team. Identify
   which rung it's currently at, whether it got there too fast or too slow,
   and draft the rung-3 decision memo — both positions stated fairly enough
   that your counterpart would sign it.
