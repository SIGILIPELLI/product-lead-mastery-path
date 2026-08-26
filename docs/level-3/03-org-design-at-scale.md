# Org Design at Scale

Meridian's product org has grown from Amara's original four-squad team to
eighteen PMs across five Leads in under two years. The org chart Amara
inherited was drawn to fit the people in the room at the time, not the
product's actual structure — and it's starting to show: two PMs on
different pods both "own" carrier pricing, a customer escalation bounces
between three pods before landing anywhere, and Sofia's Marketplace pod has
to route every data request through Tom's Integrations pod, creating a
queue neither of them controls. Org design at this scale is the discipline
of deciding how to cut up the product surface area so ownership is
unambiguous and dependencies are minimized — and re-cutting it deliberately
as the business changes, instead of letting it drift.

## The four org design patterns

| Pattern | Cut along | Strength | Weakness | Meridian fit |
|---|---|---|---|---|
| **By product/feature area** | What the product does (pricing, onboarding, integrations) | Deep expertise, clear roadmap ownership | Customer journeys cross boundaries; duplicated infra work | Current Core Carrier Ops structure |
| **By customer segment** | Who the product serves (enterprise, SMB, self-serve) | End-to-end ownership of a customer's experience | Duplicated feature work across segments | Would fit if Marketplace splits shipper vs. carrier customers |
| **By platform layer** | Technical layer (platform/infra vs. product surface) | Clean reuse, no duplicated plumbing | Product pods depend on a platform team they don't control | Emerging need as Integrations becomes shared infrastructure |
| **By journey/workflow** | An end-to-end user journey (get a load matched, get paid) | Matches how the customer experiences the product | Cuts across existing team boundaries, painful to introduce later | The fix for the escalation-bouncing problem below |

Most orgs past a certain size are a blend, not a pure pattern — the design
skill is choosing which pattern governs the *primary* cut, since that's
what determines who owns the messy, cross-cutting problems.

## Diagnosing the current structure

Before redesigning anything, Amara maps every recurring cross-pod
friction point against its root cause:

| Symptom | Root cause type | Fix category |
|---|---|---|
| Two pods claim the same feature | Boundary ambiguity | Clarify or redraw ownership lines |
| A request queues indefinitely between pods | Missing owner for shared dependency | Create an explicit platform team or an SLA contract |
| Customer escalation bounces between pods | Journey cuts across the org's cut | Consider a journey-based re-cut, or a named journey owner without moving people |
| Two pods build the same infra independently | No shared-services layer | Carve out a platform layer |
| A pod is overloaded relative to its peers | Cut doesn't match actual workload | Rebalance scope, not headcount |

Meridian's escalation-bouncing problem is a journey cut-across: a
carrier's "get onboarded, get priced, get paid" journey touches Ravi's,
Tom's, and a third pod, and no single PM owns the customer's experience of
that journey end to end.

## The org design decision framework

Redesigning an org is disruptive — every redraw costs weeks of confusion
and at least one good person questioning whether to stay. Use this before
committing to a change:

| Question | If the answer favors change |
|---|---|
| How many escalations/quarter trace to this boundary problem? | More than 2-3 substantive ones — a pattern, not an anecdote |
| Can the fix be a named owner or interface contract instead of a re-org? | If yes, do that first — it's reversible and cheap |
| Does the current structure actively block a strategic bet (like Marketplace)? | Strategic blockage outweighs local friction |
| What's the cost of doing nothing for two more quarters? | If tolerable, wait for more signal before disrupting people |

## Worked example: fixing the carrier-journey escalation

Amara doesn't reorganize Meridian's whole product team. She runs the
decision framework: three escalations last quarter, each costing a week of
cross-pod finger-pointing and one near-miss with a mid-market customer.
That's a pattern. But a full journey-based re-org would touch eighteen
people and take a quarter to stabilize — too disruptive for a problem this
narrow.

Her fix, cheapest-first:

1. **Interface contract, not re-org.** She writes a one-page RACI for the
   onboarding→pricing→payments journey: Ravi's pod is Responsible for the
   handoff quality at each boundary, a named PM on each pod is Accountable
   for their leg, and Amara is the Escalation path if the contract is
   violated twice in a quarter.
2. **Named journey owner, part-time.** One of Ravi's senior PMs is given an
   explicit (not full-time) charter: track the end-to-end journey metrics
   across all three pods and flag drift monthly. No headcount moves.
3. **Review date, six weeks out.** If escalations continue, the next step
   is a real re-org — likely carving a small "carrier journey" pod that
   pulls one PM from each of the three current pods.

Six weeks later, escalations drop from three that quarter to zero — the
interface contract was sufficient. Amara notes in her own record that the
cheap fix worked, and resists the temptation to reorganize anyway just
because the analysis was interesting.

## Span of control planning

As Amara adds Leads, she checks span of control isn't silently degrading
quality of coaching:

```python
python3 -c "
leads = {'Ravi': 4, 'Sofia': 3, 'Tom': 3, 'Priya': 4, 'Dana': 4}
total_pms = sum(leads.values())
avg_span = total_pms / len(leads)
print('total PMs:', total_pms, 'Leads:', len(leads), 'avg span:', round(avg_span, 2))
# if a 6th pod of 4 PMs is added, does it need a new Lead or fit under an existing one?
new_total = total_pms + 4
print('with new pod, total PMs:', new_total, 'implied avg span if same Lead count:', round(new_total/len(leads),2))
"
```

That comes out to 18 PMs across 5 Leads (avg span 3.6), and adding a
6th pod of 4 without adding a Lead pushes the average to 4.4 — still inside
Meridian's stated ceiling of 5 direct reports per Lead, so Amara can absorb
one more pod under an existing Lead before she needs to hire a sixth.

## Exercise

Map your own org (or the org one level above you, if you don't yet run
one) against the four patterns — which one governs the primary cut today?
Find one recurring friction point, classify its root cause using the
diagnosis table, and run it through the decision framework. Write down the
cheapest fix you'd try before reaching for a re-org.
