# Project — Org Design for a 20+ Person Product Org

Meridian's product org has crossed 22 people (18 PMs plus Amara and the
four other Leads counted separately from their pods, plus Kai from the
RouteWise acquisition now folded in as a Senior PM under Ravi). CEO Lena
asks Amara for a full org design document ahead of next year's planning —
not a status update, a real structural proposal she can take to the board
alongside the budget ask. This project is the full deliverable: the kind of
document a VP Product actually produces once a year, built from every tool
in this level.

## 1. Current-state map

| Pod | Lead | PMs | Product line(s) | Posture (Module 2) |
|---|---|---|---|---|
| Onboarding & Journey | Ravi | 5 (incl. Kai) | Core Carrier Ops | Core |
| Pricing | (vacant — Sofia covering) | 3 | Core Carrier Ops | Core |
| Integrations/Platform | Tom | 3 | Shared infrastructure | Platform (Module 8) |
| Marketplace | Sofia | 4 | Marketplace | Growth |
| Internal Tools | Priya | 3 | Internal Tools | Seed/Harvest |

That's 18 PMs across 5 Leads (one Lead role currently double-covered by
Sofia), consistent with Module 3's span-of-control numbers.

## 2. Diagnosis: three structural problems

| Problem | Root cause (Module 3 diagnosis) | Evidence |
|---|---|---|
| Sofia is overloaded — Lead of Marketplace and covering Pricing | Growth-bet Lead absorbed a vacant Core role without capacity planning | Sofia's 1:1s with her own PMs have slipped from weekly to biweekly per her own report |
| Tom's Integrations pod is structurally a platform team wearing a product-team org shape | Never formally re-typed after organic growth into shared infrastructure | 80% of Tom's backlog is cross-pod requests (Module 8) |
| Onboarding & Journey pod is oversized relative to peers | Kai's RouteWise team folded in without a re-split | 5 PMs vs. peer pods' 3-4, pushing average span toward the ceiling (Module 3) |

## 3. Target structure

```python
python3 -c "
current = {'Ravi': 5, 'Pricing(vacant)': 3, 'Tom': 3, 'Sofia': 4, 'Priya': 3}
total = sum(current.values())
print('current total PMs:', total, 'across', len(current), 'pods')

# Target: split Ravi's oversized pod, hire dedicated Pricing Lead,
# formalize Tom as Platform with its own tax-funded headcount (Module 8)
target_pods = {
    'Onboarding': 3,      # Ravi keeps onboarding core
    'Journey/RouteWise': 2,  # Kai promoted to lead this narrower scope, per M&A leveling plan
    'Pricing': 3,          # new dedicated Lead hired
    'Platform (Tom)': 3,   # unchanged headcount, re-typed funding model
    'Marketplace': 4,      # Sofia back to single-pod focus
    'Internal Tools': 3,
}
print('target total PMs:', sum(target_pods.values()), 'across', len(target_pods), 'pods')
print('avg span:', round(sum(target_pods.values())/len(target_pods), 2))
"
```

Result: 18 PMs currently across 5 pods (avg span 3.6) become 18 PMs
across 6 pods (avg span 3.0) — the same headcount, redistributed, plus one
new Lead hire (Pricing) and one internal promotion (Kai, per the M&A
leveling plan from Module 7).

## 4. The three decisions this proposal asks the board/CEO to make

1. **Approve one external Lead hire (Pricing)** — cost: one Product Lead
   salary, no net PM headcount change since the pod is a split of existing
   scope, not new scope.
2. **Approve Kai's promotion to Product Lead of the RouteWise-derived
   Journey pod**, contingent on the two-quarter evidence review from
   Module 7's leveling plan completing on schedule.
3. **Approve re-typing Tom's pod as Platform** with a 20% engineering-tax
   funding model (Module 8), removing it from portfolio competition against
   revenue-generating lines.

## 5. Risk and rollback plan

| Risk | Mitigation | Rollback trigger |
|---|---|---|
| New Pricing Lead hire takes >1 quarter to fill | Sofia continues covering with an explicit end-date and reduced Marketplace targets during the gap | If unfilled after 2 quarters, reassess whether Pricing needs a dedicated Lead at all |
| Kai's promotion evidence doesn't clear the bar in 2 quarters | Kai remains Senior PM under Ravi, Journey pod folds back into Onboarding | Explicit review date already set (Module 7) |
| Platform tax model creates funding resentment from product Leads | Amara reviews tax rate quarterly against actual platform adoption metrics (Module 8) | Adoption metrics flat or declining for 2 straight quarters |

## 6. Communication plan

Following Module 5's structure, Amara pre-wires (Module 9) the two board
members most likely to have questions — the lead investor's rep (unit
economics of the new hire) and the founder-friendly director (whether this
dilutes focus) — before the planning meeting, then presents the proposal
to the full board using headline/ask/evidence/risk, not a walkthrough of
this full document (which goes out as the pre-read).

## Stretch goals

- Build the actual career-ladder leveling packet (Module 4 format) you
  would use to evaluate Kai's promotion at the two-quarter review point,
  with named evidence criteria decided now, before the outcome is known.
- Draft the board pre-read slide (Module 5/9 format) for this proposal,
  under 200 words, and have someone unfamiliar with Meridian read only the
  headline and ask — check whether they can correctly state what's being
  requested.
- Extend the target-structure headcount model to simulate what happens if
  Marketplace hits its growth targets a year early and needs to split into
  two pods — re-run the span-of-control math and identify which existing
  Lead is the natural candidate to lead the split-off pod.
