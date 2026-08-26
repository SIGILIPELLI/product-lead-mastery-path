# Multi-Product Portfolio Leadership

Meridian Logistics now runs three distinct product lines under Amara: Core
Carrier Ops (Ravi's and Tom's pods — onboarding, integrations, pricing),
Marketplace (a newer bet connecting carriers to spot-market loads, led by
Sofia), and Internal Tools (Priya's pod, serving Meridian's own ops staff).
Each has a different maturity, a different growth rate, and a different
claim on the same finite engineering budget. Amara's job is no longer to
have an opinion on any one roadmap — it's to decide how much of the company
each product line deserves, and to defend that allocation when a Lead
argues (correctly, from their seat) that their line deserves more.

## Classify before you allocate

Every product line falls into one of four postures. Misclassifying one is
the single most common portfolio mistake — treating a Growth product like a
Core product starves it just as it's proving out, and treating a Core
product like a Growth bet starves the revenue that funds everything else.

| Posture | Signal | Investment logic | Meridian example |
|---|---|---|---|
| **Core** | Established, funds the company, customers expect stability | Protect reliability, invest in efficiency, resist scope creep | Core Carrier Ops |
| **Growth** | Proving product-market fit, metrics trending but not proven | Fund aggressively, tolerate higher risk, short review cycles | Marketplace |
| **Harvest** | Mature, declining relevance, still has revenue | Minimize investment, extend life cheaply, plan the sunset | (none yet at Meridian) |
| **Seed** | Pre-PMF, small team, exploring | Cap the spend, set a kill/scale decision date, protect from Core's process overhead | Internal Tools' newest ops-forecasting feature |

## The allocation model

Amara builds a simple portfolio table each quarter and takes it to the CEO,
Lena, before finalizing headcount. The percentages are engineering-capacity
share, not headcount, since pods vary in size.

| Product line | Posture | Current % of eng capacity | Revenue/strategic weight | Target % next quarter |
|---|---|---|---|---|
| Core Carrier Ops | Core | 55% | Funds 90% of company revenue | 45% |
| Marketplace | Growth | 30% | 0% of revenue, board's #1 growth bet | 40% |
| Internal Tools | Seed/Harvest mix | 15% | Cost-saving, no revenue | 15% |

Let's verify this allocation is internally consistent with headcount.

```python
python3 -c "
eng_total = 40  # total product-eng headcount
current = {'core': 0.55, 'marketplace': 0.30, 'tools': 0.15}
target = {'core': 0.45, 'marketplace': 0.40, 'tools': 0.15}
for k in current:
    cur_hc = round(eng_total * current[k])
    tgt_hc = round(eng_total * target[k])
    print(k, 'current_hc=', cur_hc, 'target_hc=', tgt_hc, 'delta=', tgt_hc - cur_hc)
print('current total', sum(round(eng_total*v) for v in current.values()))
print('target total', sum(round(eng_total*v) for v in target.values()))
"
```

Running this gives: core 22→18 (-4), marketplace 12→16 (+4), tools 6→6 (0),
current and target both summing to 40. The move is a clean four-engineer
swap from Core to Marketplace — small enough to execute without a
reorg, large enough for Sofia to feel the difference in her pod.

## The three questions that decide reallocation

Before moving capacity between lines, Amara forces every request through
the same three questions, in this order:

1. **What decision does more capacity unlock that less capacity doesn't?**
   Not "we'll go faster" — a specific milestone that flips from "next year"
   to "this quarter."
2. **What does the losing line stop doing, specifically?** If nobody can
   name the thing that stops, the "loss" wasn't real capacity, it was slack
   that shouldn't have existed — a finding in itself.
3. **What's the review date to re-litigate this?** Every reallocation is
   time-boxed. Nothing is permanent without a second decision.

## Worked example: Sofia's case for more capacity, Ravi's case against

Sofia comes to Amara with data: Marketplace's match rate (loads matched to
carriers within 24 hours) is at 61%, and her model says two more engineers
gets it to 78% within a quarter — the threshold the board set for
green-lighting Marketplace as a standalone product line. Ravi pushes back:
Core Carrier Ops has a customer-committed SLA migration due the same
quarter, and losing two engineers risks missing it, which risks actual
contracted revenue.

Amara's process, not instinct:

- She asks Ravi the loss question directly: what specifically slips? Ravi
  names it — the SLA migration moves from "on track" to "50/50," with a
  named enterprise customer whose contract renews on that timeline.
- She asks Sofia: is 78% match rate the actual board threshold, or her
  own stretch goal? Sofia checks — it's the actual threshold, documented in
  the board deck from two quarters ago.
- The reversibility test breaks the tie: Marketplace's board threshold has
  a hard external decision date (the next board meeting, six weeks out).
  The SLA migration has a customer relationship that can absorb a two-week
  slip with an early warning call. Marketplace can't absorb slipping past
  the board meeting.
- Decision: two engineers move for six weeks only, with an explicit return
  date, and Ravi gets a customer-communications assist from Amara to manage
  the SLA slip risk. Both Leads leave knowing the criteria, not just the
  verdict.

## Portfolio review cadence

| Cadence | Who's in the room | What's reviewed |
|---|---|---|
| Weekly | Amara + whichever Lead has an active fire | Tactical only, not allocation |
| Monthly | All five Leads | Cross-line dependencies, early-warning metrics per line |
| Quarterly | All five Leads + CEO Lena | Full portfolio table, reallocation decisions, posture reclassification |

## Exercise

Build a portfolio table for the product lines or major initiatives you
oversee (or, if you're not yet managing a portfolio, use two projects your
own team runs as a stand-in). Classify each by posture, estimate current
capacity share, and write the three-question test output for one
reallocation you're currently being asked to make or are considering
making yourself.
