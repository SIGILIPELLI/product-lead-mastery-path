# Performance Management for PMs

Performance management is the part of the job most Product Leads do badly,
because it's the only part where the cost of avoidance is invisible in the
short run and enormous in the long run. A PM who has been underperforming
for three quarters without ever being told is not a performance problem —
it's a management failure with a person's career attached to it.

PM performance is also genuinely harder to assess than most functions. A PM
who shipped nothing may have correctly killed a bad bet. A PM who shipped a
lot may have been handed an easy roadmap. This module gives you a rubric
that separates outcomes from behaviours, a calibration process that survives
contact with other managers, and a script for the conversation you're
avoiding.

## The PM performance rubric

Rate on four dimensions, not one overall gut feeling. Use behavioural
descriptors, not adjectives — "communicates well" is unratable; the rows
below are.

| Dimension | Below bar | At bar | Above bar |
|---|---|---|---|
| **Outcomes** | Ships, but can't connect output to a metric or customer change | Owns a metric, moves it, and can explain the causal chain | Moves a metric *and* the result changes what the wider team does next |
| **Judgement** | Escalates decisions that were theirs; or makes calls outside their remit without telling anyone | Makes the calls they own, escalates the ones they don't, on time | Reliably right on close calls; their reasoning gets reused by other PMs |
| **Craft** | Specs are ambiguous; discovery is thin or absent; engineers reverse-engineer intent | Clear problem statements, real customer evidence, decisions documented | Sets the artefact standard others copy |
| **Influence** | Needs you in the room to get cross-functional agreement | Runs their own stakeholder relationships and lands hard trade-offs | Changes the mind of people senior to them, without you |

Two rules for using it:

- **Rate against the level, not the person's tenure.** A senior PM at bar and
  a junior PM at bar receive the same rating word and different expectations
  behind it.
- **Every rating needs two written examples.** If you can't produce two, you
  don't have a rating, you have an impression.

## Setting expectations before the cycle, not after

Half of all performance disputes are actually expectation disputes. Write
this at the *start* of the cycle, one page per PM:

| Section | What it contains | Example |
|---|---|---|
| Scope | What this PM owns, and what they don't | "Owns carrier onboarding end to end; does not own pricing surfaces" |
| Outcomes | 2-3 measurable results, with the metric and the target | "Median time-to-live from 14 to 7 days by 31 March" |
| Behaviours | 1-2 rubric dimensions they're being stretched on | "Influence: run the ops-team relationship directly; I'll stop attending" |
| Constraints | What's outside their control, so it can't be held against them | "Data-migration tooling depends on Platform; a slip there is not on you" |
| What 'above bar' would look like | A concrete, specific picture | "Onboarding playbook adopted by the support org without you pushing it" |

The Constraints row is the one most managers skip and the one PMs remember.
It's how you avoid grading someone on a dependency they never controlled.

## Running calibration with other managers

Calibration exists to make ratings comparable across managers, not to force
a distribution. Come prepared, or your PMs get rated on your articulacy
rather than their work.

| Step | What you bring | What you say |
|---|---|---|
| 1. Pre-read | One page per PM: rubric ratings, two examples per dimension | Nothing — send it 48h ahead |
| 2. Open with the hardest case | Your most contested rating, first, while attention is high | "I have Sofia at above bar on judgement; here's the call she made in January and why it was hard" |
| 3. Anchor on evidence | Specific artefacts and decisions | "This is the doc. Compare it to what we'd expect from a senior PM" |
| 4. Test for scope inflation | Roadmap difficulty, not volume | "Was this an easy roadmap? Who handed it to them?" |
| 5. Absorb the challenge | Other managers' counterexamples | "Fair — that changes my read on influence; I'll take it to at bar" |
| 6. Leave with commitments | Final ratings plus what each PM will be told | Write the message before you leave the room |

Warning signs in a calibration room: ratings that track how much a manager
talks; a PM being downgraded for a dependency failure; "potential" being
used to raise a rating (potential belongs in a promotion case, not a
performance rating for work already done).

## Handling underperformance

The sequence matters. Skipping straight to formal documentation is unfair;
never getting there is cowardice.

| Stage | Trigger | What you do | Timebox |
|---|---|---|---|
| 1. Direct feedback | You've seen the pattern twice | SBI in a 1:1: situation, behaviour, impact. Name it as a pattern, not an incident | Immediately |
| 2. Explicit expectation | No change after 3-4 weeks | Write down the specific change required and how you'll both know it happened | 30 days |
| 3. Structured support | Change is partial | Weekly checkpoint, one skill focus, concrete artefacts to produce | 30-60 days |
| 4. Formal plan | No meaningful change | Written plan with HR, unambiguous success criteria, stated consequence | Per company policy |
| 5. Decision | End of plan | Meets bar → close it out explicitly. Doesn't → transition, handled with dignity | Firm date |

Language that makes stage 1 land, from a real 1:1 script:

> "I want to name a pattern, not a one-off. In the last two roadmap reviews
> — the January one and last Thursday's — you presented a list of features
> without a customer problem attached to each. The impact is that engineering
> can't sequence the work, so they sequence it by whatever's easiest, and
> then we ship the wrong thing first. What I need to see in the next review
> is one sentence of customer evidence per item. Where do you think the gap
> is coming from?"

Note what that does: names two specific instances, states the downstream
impact mechanically rather than morally, defines the observable change, and
ends with a question that leaves room for a cause you don't know about.

## Worked example: the "ships a lot, moves nothing" PM

Tom has been a PM at Meridian for two years. He is well-liked, ships
consistently, and his squad's velocity is the highest in the org. His
manager Amara has rated him at bar for four cycles. This cycle she looks
harder and finds: incident count — Tom's stated quarterly metric — has not
moved in a year, and every shipped item traces back to a request from the
partner-success team rather than from customer evidence.

Rubric read: Outcomes below bar (ships, metric flat), Judgement at bar,
Craft at bar, Influence below bar (he takes requests rather than shaping
them). Overall: below bar — after four cycles of "at bar."

Amara's honest problem is that *she* created this. Tom was never told his
job was to move incident count rather than to satisfy the partner-success
queue. So the sequence is:

1. **Reset expectations before rating.** She rewrites his one-pager: the
   outcome is P1 incidents from 6 to 2 per quarter, and the constraint row
   explicitly says intake volume from partner-success is not a measure of
   success. She says out loud: "This is a change in what I'm asking for. The
   old expectation was mine to set and I set it badly."
2. **Rate this cycle honestly but attribute fairly.** In calibration she
   argues Tom at bar for this cycle — flagging that the outcome miss stems
   from an expectation she never set — and states plainly that next cycle
   will be rated against the new one-pager. Calibration accepts it because
   she brought the written evidence.
3. **Start stage 1 feedback immediately,** not at the next review. The SBI
   is about intake behaviour: "In the last three planning sessions you took
   the partner-success list as the roadmap. The impact is we spend the
   quarter on symptoms and the incident rate doesn't move."
4. **Give one structural help,** because feedback without changed conditions
   rarely works: she moves the partner-success intake to a monthly triage
   *she* attends, so Tom has cover to say no.
5. **Sets a checkpoint at 45 days.** At the checkpoint, Tom has killed two
   requested features, shipped one retry-logic change, and incident count is
   at 4. Amara records that as evidence in the next cycle's file — good
   performance evidence needs writing down at the moment it happens just as
   much as bad does.

## Cheat sheet

| Trap | Correction |
|---|---|
| One overall gut rating | Four rubric dimensions, two written examples each |
| Grading on output volume | Grade on metric movement and decision quality |
| Punishing a dependency failure | Put it in the Constraints row before the cycle starts |
| "Potential" raising a rating | Potential belongs in promotion cases, not performance ratings |
| Surprise at review time | Stage 1 feedback happens the week you see the pattern twice |
| Documenting only bad performance | Write down good evidence when it happens, too |
| Conflating a cancelled strategy with a PM's failure | Rewrite the goal; rate against the rewritten one |

## Exercise

Pick two real people you manage (or two realistic PM profiles: one strong,
one struggling).

1. Rate each on all four rubric dimensions, and write the two supporting
   examples per dimension. Note any dimension where you *can't* produce two
   — that gap is your homework this month, not theirs.
2. Write the start-of-cycle one-pager for the struggling PM, including a
   genuinely honest Constraints row.
3. Write the stage-1 SBI script you would say to them, out loud, in your next
   1:1 — two named instances, mechanical impact, observable required change,
   and a closing question.
4. Prepare the calibration opener for your strongest PM: the single hardest
   decision they made this cycle and why it was hard. If you can't name one,
   your "above bar" rating is not yet defensible.
