# Budget & Resourcing for Product Teams

Most Product Leads meet budget for the first time as a form to fill in, and
treat it as an administrative tax on the real job. It isn't. Budget is where
strategy either gets funded or quietly doesn't, and a Lead who can't argue
in money and people will watch their strategy get decided by whoever can.

The uncomfortable arithmetic: a single squad — one PM, one designer, five
engineers — costs somewhere around £700k-£900k a year fully loaded in most
Western markets. When you ask for a squad, you are asking for the price of a
house. When you defend one, you are defending the same. Once you internalise
that, the conversation changes from "we need more people" to "here is what
that spend returns and here is what we'd stop doing instead."

## Know what you actually cost

Before any planning conversation, build this table. Use your finance team's
real loaded-cost multiplier if you can get it; otherwise assume salary ×
1.3-1.4 for employment costs, and add tooling separately.

| Line item | Basis | Meridian example (annual) |
|---|---|---|
| Product headcount | Loaded cost per PM | 4 PMs × £110k = £440k |
| Design headcount | Loaded cost per designer | 2 × £95k = £190k |
| Research / data | Shared or dedicated | 0.5 researcher = £45k |
| Contractors | Rate × expected weeks | 12 weeks @ £3k/wk = £36k |
| Tooling | Per-seat and platform | Analytics £28k, research tools £9k, roadmap tool £6k |
| Customer research costs | Incentives, travel, panels | £12k |
| Discretionary / experiments | Unallocated buffer | £25k |
| **Total product-org spend** | | **£791k** |

Two habits that separate Leads who get funded from those who don't:
**know your numbers without looking them up**, and **know your cost per
squad**, because that's the unit executives actually think in.

## Headcount planning that survives scrutiny

A headcount request built on "the team is stretched" loses to one built on
demonstrated throughput and a named outcome. Fill every row before you ask.

| Field | What it must contain | Weak vs. strong |
|---|---|---|
| Role and level | Specific | "Senior PM, Pricing" not "another PM" |
| The problem it owns | From the strategy cascade | Must map to a named company-level problem |
| Evidence of need | Throughput data, not feelings | "Pricing has 3 initiatives and one PM at 60% on pilot support" beats "Sofia is busy" |
| What happens without it | The concrete cost | "Pricing bet decision slips from July to January" |
| What we'd stop instead | The self-funding option | "Or we fold Internal Tools and redeploy" |
| Ramp time | When it produces value | "Hire in Q1, productive Q2, outcome visible Q3" |
| Downstream costs | The hidden multiplier | "One PM implies design capacity and 4-6 engineers to be useful" |

The downstream-costs row is where credibility is won. A Lead who says "and
this PM is only useful if Engineering also funds four roles" is trusted on
every subsequent request. A Lead who lets that surprise everyone in month
two is not.

## Resourcing trade-offs across initiatives

When demand exceeds capacity — always — score openly rather than deciding by
whoever escalated most recently.

| Initiative | Strategy problem | Est. cost (squad-quarters) | Expected outcome | Confidence | Reversible? | Decision |
|---|---|---|---|---|---|---|
| Onboarding migration tooling | P1: 30-day churn | 1.5 | Time-to-live 14d → 7d | High | Yes | Fund fully |
| Pricing pilot expansion | P2: pricing gap | 1.0 + £18k contractor | 5 pilots → FY26 decision | Med | Yes | Fund with contractor |
| Integrations v1 migration | P3: silent failures | 0.75 | Forced by partner deprecation | High | No | Fund — non-negotiable |
| Internal support tooling | P1 (indirect) | 0.75 | Handle time −20% | Low | Yes | Defer, review in Q3 |
| Enterprise SSO | None | 0.5 | Unblocks 2 deals | Med | Yes | Decline — not in strategy |

**Squad-quarters** is the unit worth adopting: one squad, one quarter. It
converts arguments about priority into arithmetic about capacity, and it
makes "we can do all of this" visibly false in a way that a ranked list
never does.

The **Reversible?** column decides ties. Between two initiatives of equal
value, fund the irreversible one first — a partner deprecation date doesn't
negotiate, and a deferred reversible bet can be picked up next quarter at
roughly the same cost.

## Defending the budget

| Challenge you'll hear | Weak answer | Strong answer |
|---|---|---|
| "Can you do it with 10% less?" | "That would be very difficult" | "Yes — here's the specific thing that stops. 10% is roughly the Internal Tools squad's PM; handle-time work pauses. Confirm and I'll action it." |
| "Why is tooling this expensive?" | "It's what we've always spent" | "£28k analytics, used by 40 people daily; the alternative is 2 days/month of manual reporting per PM, which costs more." |
| "Other teams manage with fewer PMs" | Defensiveness | "Our ratio is 1 PM : 6 engineers. Below 1:8 quality drops; here's the incident data from when we ran at 1:9." |
| "Cut the contractor line" | Silent compliance | "That's the pricing pilot's fifth customer. Cutting it means the FY26 pricing decision is made on 3 data points in July." |
| "Just prioritise better" | "We already do" | Show the squad-quarters table. Prioritisation already happened; this is the residue. |

The move that works in every row: **never say no, say what stops.** A Lead
who answers cuts with a specific, costed consequence gets treated as a
partner in the trade-off. A Lead who resists gets overridden.

## Worked example: Meridian's FY26 planning round

Amara is asked for a flat-budget FY26 plan, then — two weeks later — a
version with a 10% cut, which is how most planning rounds actually go.

**Preparation.** She builds the cost table above (£791k) and computes her
unit economics: roughly £198k of *product-org* cost per squad, and — with
engineering loaded in from her eng peer's numbers — about £820k fully loaded
per squad-year. This second number is the one she uses with executives,
because it's the number they think in.

**The flat plan.** Demand for FY26 is 6.5 squad-quarters per quarter against
a capacity of 4. She builds the trade-off table, and it does the arguing for
her: Integrations v1 is irreversible and funded first despite being the
lowest-visibility work; Enterprise SSO is declined outright with a written
reason, because it maps to no strategy problem — and a declined item with a
stated reason is far more defensible than an item that silently never
happens.

**The 10% cut, arriving in week 3.** £79k. Amara does not spread it thinly
across every line, which is the instinct and the mistake — a 10% haircut on
everything degrades all five initiatives and kills none, which is the worst
available outcome. She proposes one concentrated cut: fold the Internal
Tools squad's PM role into support-side ownership, saving £110k, and
redirect £31k of it back into the pricing contractor. The support handle-time
work stops, explicitly and on the record.

**The defence.** The COO asks why the tooling line can't absorb it instead.
Amara has the answer costed: cutting the analytics platform saves £28k and
costs roughly two days per PM per month in manual reporting — about 96
PM-days a year, which is more than £28k of PM time. She's not defending the
tool; she's showing the cut is negative-value arithmetic. It survives.

**The headcount ask, made in the same meeting.** Amara asks for the Senior
PM on Pricing anyway, using the planning table: Pricing has three
initiatives and one PM who is 60% consumed by pilot support; without the
hire the FY26 pricing decision slips from July to January; the self-funding
option is exactly the Internal Tools fold she has already proposed. She also
states the downstream cost unprompted — the hire needs 0.5 of a designer and
three engineers to be worth anything. The role is approved for Q2, not Q1,
which is a normal outcome and worth taking.

**What she does in month two, which most Leads skip.** She tracks actuals
against the plan. The pricing contractor runs 8 weeks instead of 6 (£6k
over); research incentives come in £4k under. She reports both, unprompted,
in her monthly update. Nobody asked. The reason to do it is that the next
time Amara says a number, finance believes it — and being believed is the
whole of budget power.

## Cheat sheet

| Trap | Correction |
|---|---|
| Not knowing your own numbers | Memorise total spend and cost per squad-year |
| Asking for "more people" | Ask for a named role owning a named strategy problem |
| Hiding downstream costs | State the design and engineering implications unprompted |
| Spreading a cut evenly | Concentrate it; degrade one thing fully rather than everything partly |
| Answering a cut with "that's difficult" | Answer with the specific thing that stops |
| Ranked lists as capacity planning | Squad-quarters — arithmetic, not ordering |
| Ties broken by who escalated loudest | Break ties on reversibility; fund the irreversible first |
| Items that silently never happen | Decline explicitly, in writing, with a reason |
| Never reporting actuals | Report variance unprompted; it's how numbers become trusted |

## Exercise

Use your real team, or a realistic 3-4 squad org.

1. Build the full cost table, including tooling and research. Compute cost
   per squad-year with engineering loaded in. If you can't get real
   multipliers, use salary × 1.35 and say so.
2. Build the squad-quarters trade-off table for next quarter's demand. If
   demand doesn't exceed capacity, you've under-collected demand — go back.
3. Take your single most-wanted headcount and fill in all seven planning
   rows, including the "what we'd stop instead" and downstream-cost rows.
4. Simulate a 10% cut. Write the *concentrated* proposal, name exactly what
   stops, and write the sentence you'd say when asked to spread it instead.
5. Pick the line item you'd most struggle to defend. Cost out the
   alternative in hours or risk. If the arithmetic doesn't favour you, cut
   it yourself before someone else does — and get the credit.
