# Advanced Executive Communication

Amara's first board-adjacent deck — a Marketplace update she prepared for
CEO Lena to bring to the board — came back with a note: "This is a great
PM update. I need a board update." She'd written six slides of roadmap
detail, feature-by-feature progress, and a risk list. None of it was wrong,
and none of it was what a board needs. Executive communication at this
level isn't "the same update, shorter" — it's a different information
architecture built around decisions and risk, not activity.

## The altitude shift in communication

| Audience | What they need first | What they can tolerate | What loses them instantly |
|---|---|---|---|
| Your PMs | Specifics, the "how" | Long discussion of tradeoffs | Vague direction |
| Your Leads | Patterns across their pod, decision criteria | Some ambiguity to resolve themselves | Being told the answer instead of the frame |
| Executive peers (eng/sales/finance leads) | What you need from them, by when | Context on why | A narrative with no ask |
| CEO | The decision or risk, up front | One layer of "why," on request | Getting to the point on slide 5 |
| Board | Trajectory vs. commitment, and what could break it | High-level metrics, not features | Feature lists, org charts, anything operational |

## The inverted-pyramid structure for exec updates

Every level-appropriate update follows the same shape, just with the detail
threshold moving as the audience gets more senior.

| Section | Content | Length at CEO level | Length at board level |
|---|---|---|---|
| Headline | The one sentence that matters | 1 line | 1 line |
| Decision/ask | What you need from them, if anything | 1-2 lines | 1-2 lines |
| Evidence | Why the headline is true | 3-4 bullets | 2-3 bullets, higher altitude |
| Risk | What could invalidate this in 90 days | 2-3 bullets | 1-2 bullets, only material risk |
| Detail (appendix) | Everything a Level 1-2 update would contain | Available on request | Rarely opened |

The discipline is resisting the urge to walk the detail before the
headline "to build up to it." Executives read the headline and decide how
much attention the rest earns — burying it costs you the room's attention
budget on the part that matters least.

## Worked example: rewriting the Marketplace board slide

Amara's original slide (rejected):

> "Marketplace update: shipped carrier-matching v2, load-posting UI redesign
> in progress, 3 P1 bugs fixed, working on API rate limiting, next sprint
> covers notification improvements..."

Rewritten using the inverted pyramid:

> **Headline:** Marketplace match rate is at 61%, on track to hit the 78%
> board threshold by [date] — six weeks ahead of the original plan.
>
> **Ask:** None this cycle — flagging early in case the board wants to
> discuss accelerating the standalone-product decision given the pace.
>
> **Evidence:** Match rate up from 54% to 61% this quarter after
> carrier-matching v2 shipped; two enterprise pilot customers signed against
> a target of three; engineering capacity increased from 12 to 16 (see
> Module 2's portfolio reallocation).
>
> **Risk:** Rate-limiting issue with our largest data partner could cap
> throughput before we hit 78% — mitigation in progress, will flag if
> unresolved by next review.

Same underlying facts as the rejected version. The difference is that the
board can act on the second version in thirty seconds — they know what's
true, what's being asked of them, and what could go wrong — while the
first version required them to synthesize a decision themselves out of
seven bullet points of activity.

## The pre-read vs. the room

At board level, the pre-read and the live discussion serve different
purposes, and conflating them is a common Level 3 mistake:

| | Pre-read (sent 48h ahead) | Live discussion |
|---|---|---|
| Purpose | Transfer information | Make decisions, surface disagreement |
| Content | Full headline/ask/evidence/risk, appendix attached | Only the ask and the risk — assume it's been read |
| Amara's job | Write it so no explanation is needed live | Facilitate, don't re-present |
| Common mistake | Sending it too late for anyone to actually read | Walking through the pre-read slide by slide anyway |

If Amara catches herself re-presenting the pre-read in the room, that's a
signal the pre-read didn't land — worth asking Lena directly whether board
members read materials in advance, rather than assuming and wasting the
room's time as insurance.

## Handling a hostile or skeptical question live

Executive rooms sometimes push back hard, and the instinct to defend every
detail backfires. Amara's framework, used live:

1. **Name the concern back, one sentence.** "You're worried the 78%
   threshold was set before we knew about the rate-limiting risk."
2. **Answer the real question, not a safer one.** Don't pivot to a metric
   that looks better if it's not what was asked.
3. **If you don't know, say so with a date.** "I don't have that number —
   I'll have it to you by Friday," beats a confident guess that turns out
   wrong.
4. **Don't relitigate after the room has moved on.** A worse answer given
   once beats a better answer that reopens a closed topic and eats the next
   agenda item's time.

## Exercise

Take your most recent status update to a manager or exec (an email, a
slide, a doc) and rewrite it using the headline/ask/evidence/risk
structure. Cut it to one-third of its original length. Then identify one
upcoming update where you're tempted to lead with activity instead of the
headline, and write the headline sentence first, before drafting anything
else.
