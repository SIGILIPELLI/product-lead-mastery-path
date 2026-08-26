# Capstone — Full CPO-Level Strategy Document

Amara decides to stay at Meridian and take the General Manager stretch
assignment (Level 4 Module 9) while continuing as CPO, and Lena asks for
one final deliverable before the board meeting that approves it: a
complete CPO-level strategy document for Meridian's next three years,
covering the whole company's product organization, not just Marketplace.
This capstone assembles every tool from Level 3 and Level 4 into the single
document a real CPO produces once a year — the deliverable this entire
curriculum has been building toward.

## 1. Belief, position, and bets (Level 4 Module 1)

**Belief:** Mid-market carrier consolidation around unified software
continues, and the next differentiator is AI-assisted decision-making
(pricing, matching, routing) layered on that unified base — carriers will
choose whichever platform makes the fewest decisions require their own
manual judgment, not just whichever has the most features.

**Position:** Meridian owns the mid-market carrier segment end-to-end
across three regions (US, Europe, Southeast Asia); Meridian does not
compete for enterprise carriers with in-house tooling, and does not expand
into new verticals outside logistics.

**Bets for the next 3 years:**
1. Carrier-journey unification, extended globally (Level 3 Module 3, Level
   4 Module 6)
2. Marketplace as an independent, P&L-owned product line (Level 3 Module
   2, now under GM structure per Module 9)
3. AI-assisted pricing and matching, resumed post-turnaround (Level 4
   Modules 3 and 7)
4. Regional platform consolidation — evaluating whether Europe/SEA need
   their own Platform pods or can depend on the US Platform team as
   dependency latency and self-service tooling improve (Level 3 Module 8,
   Level 4 Module 7)

## 2. Organization design supporting the bets

| Bet | Owning structure | Headcount need |
|---|---|---|
| Journey unification | Ravi's Onboarding pod + Kai's Journey pod (Level 3 Module 10's target structure) | No new headcount — already the target structure |
| Marketplace as independent line | Sofia as GM-track Lead, Dana as proven backup (Level 4 Module 5) | 2 additional PMs over the plan period |
| AI pricing/matching | Reconstituted from the paused turnaround team (Level 4 Module 3) | 3 PMs, re-funded from the platform tax re-evaluation (Level 4 Module 7) |
| Regional platform | Tom's US Platform pod, extended mandate | 2 additional platform engineers, funded via tax-rate adjustment |

```python
python3 -c "
current_total = 46  # post-turnaround headcount (Level 4 Module 3)
new_hc = {'marketplace': 2, 'ai_pricing': 3, 'platform_regional': 2}
total_new = sum(new_hc.values())
target_total = current_total + total_new
print('current:', current_total, 'new hires:', total_new, 'target total:', target_total)
# check against a stated growth ceiling of 15% headcount growth for the plan period
growth_ceiling = round(current_total * 1.15)
print('15% growth ceiling:', growth_ceiling, 'within ceiling:', target_total <= growth_ceiling)
"
```

## 3. Leadership pipeline supporting the plan (Level 4 Module 5)

| Seat | Successor readiness |
|---|---|
| CPO (Amara, partially stepping into GM role) | No 90-day-ready internal successor yet; explicit gap, flagged to Lena and the board rather than hidden |
| Marketplace GM/Lead | Dana, exposure-tested per Level 4 Module 5's worked example |
| Regional Platform Lead | Gap remains; Tom to document and rotate a successor candidate within 3 quarters |

## 4. Risk register

| Risk | Likelihood | Mitigation |
|---|---|---|
| CPO succession gap during GM transition | Medium | Amara remains CPO of record during the stretch year; board informed explicitly (Level 4 Module 4's candor standard) |
| AI-pricing bet repeats prior pause if market softens again | Medium | Reversibility window built in (Level 4 Module 1's three-bet tests); resume/pause decision points set quarterly |
| Regional platform consolidation increases cross-region dependency risk | Low-medium | Self-service test (Level 3 Module 8) re-run before committing to consolidation vs. duplicate regional platform teams |

## 5. Board communication plan (Level 3 Modules 5, 9; Level 4 Module 4)

Pre-wire the lead investor's rep (unit economics of the GM/Marketplace
structure) and the founder-friendly director (risk of CPO attention
splitting across CPO and GM roles) individually, a week ahead. Present
using headline/ask/evidence/risk: headline is the three-year belief and
position; ask is board approval of the GM structure and the associated
headcount growth; evidence is the bet-by-bet structure above; risk is the
register in section 4, led with the CPO-succession gap rather than burying
it, consistent with the candor standard from the turnaround chapter.

## Stretch goals

- Write the actual one-page pre-read (Level 3 Module 5 format, under 300
  words) that would accompany this document to the board, and test it on
  someone unfamiliar with Meridian: can they state the ask and the top risk
  after reading only the pre-read, not the full document?
- Extend the headcount growth-ceiling check above to model a scenario where
  the AI-pricing bet's reversibility window (Level 4 Module 1) triggers a
  pause at month 9 — recompute the target headcount and platform tax rate
  (Level 3 Module 8, Level 4 Module 7) under that scenario.
- Using the legacy-audit framework (Level 4 Module 8), assess which parts
  of this very strategy document's authorship process would survive if
  Amara moved fully into the GM role and stepped back from CPO duties
  within the plan period — and name who would need to inherit strategy
  co-authorship for it to hold.
