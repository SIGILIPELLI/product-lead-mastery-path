# Platform vs Product Team Structures

Tom's Integrations pod has quietly become something other than a product
pod. Every other pod at Meridian depends on the carrier-data pipeline his
team built — Ravi's onboarding flow reads from it, Sofia's Marketplace
matching engine reads from it, and now RouteWise's route-optimization
engine needs it too. Tom still reports to Amara as a peer Product Lead with
his own roadmap and customers, but in practice his backlog is 80% requests
from other pods, and he has no product of his own that ships to an external
customer. Meridian has a platform team wearing a product team's org
structure, and the mismatch is producing exactly the symptoms you'd expect:
Tom's roadmap gets deprioritized against pods with visible customer
deadlines, even though his work blocks all of them.

## Product team vs. platform team: the real distinction

| Dimension | Product team | Platform team |
|---|---|---|
| Customer | External (carriers, shippers) | Internal (other product teams) |
| Success metric | Customer/business outcome (match rate, conversion) | Adoption, reliability, developer velocity of consumers |
| Roadmap driver | Market and customer discovery | Internal demand plus platform-health investment |
| Funding logic | Justified by revenue/growth impact | Justified by multiplied leverage across product teams — harder to show directly |
| Common failure if mis-structured as the other | Platform work starved because it has no visible external customer | Product decisions made by committee of consumer teams, nobody owns outcomes |

## The self-service test

The single best diagnostic for whether something should be a platform team:
can a product team consume the capability without a Slack message to a
human on Tom's team? If every consumption event requires bespoke work from
Tom's pod, it isn't a platform yet — it's a product team with unusually
technical customers, and it should be funded and evaluated that way until
it's actually self-service.

| Capability | Self-service today? | Implication |
|---|---|---|
| Carrier-data pipeline read access | No — requires Tom's team to build each new integration | Still a product-team-with-internal-customers model; fund against internal SLA commitments, not a platform budget |
| Rate-limiting/API gateway | Yes — documented, any pod can configure it themselves | True platform; success metric should be adoption + uptime, not features shipped |

## Restructuring Tom's pod: the decision

Amara doesn't relabel Tom's team "Platform" and call it done — that's a
title change, not a structural fix. She works through three real
decisions:

1. **Funding model.** Instead of competing for portfolio share against
   pods with external revenue stories (Module 2's problem), platform work
   gets funded as a fixed "tax" — a percentage of total product-eng
   capacity reserved before the portfolio allocation happens, justified by
   multiplier effect rather than direct revenue.
2. **Prioritization mechanism.** Rather than Tom's roadmap being decided by
   whichever consuming pod escalates loudest, Meridian adopts an internal
   SLA: platform requests get a committed response time by priority tier,
   and consuming pods can buy priority with their own engineering capacity
   (send an engineer to pair on the integration) rather than just asking.
3. **Success metric change.** Tom stops being measured on "features
   shipped" and starts being measured on adoption (how many pods
   self-serve without his team's involvement) and reliability (incident
   rate on the pipeline). This changes what Tom optimizes for — building
   documentation and self-service tooling becomes valuable work instead of
   a distraction from "real" roadmap items.

## The tax rate, checked against reality

Amara proposes a 20% platform tax on total engineering capacity. Verify
against Module 2's numbers before committing:

```python
python3 -c "
eng_total = 40
platform_tax = 0.20
platform_hc = round(eng_total * platform_tax)
remaining = eng_total - platform_hc
print('platform headcount:', platform_hc)
print('remaining for product-line portfolio:', remaining)
# re-run Module 2's target allocation against the remaining pool
target = {'core': 0.45, 'marketplace': 0.40, 'tools': 0.15}
for k, v in target.items():
    print(k, round(remaining * v))
print('sum check:', sum(round(remaining*v) for v in target.values()), 'vs remaining', remaining)
"
```

This yields a platform headcount of 8, leaving 32 for the portfolio —
core 14, marketplace 13, tools 5, summing to 32. Amara flags the
rounding gives tools one fewer than a clean 15% would (4.8 rounds to 5,
actually fine) and takes the whole-number split to her Leads as a starting
point, adjustable at the next quarterly review rather than treated as
exact science.

## When to un-platform something

The reverse mistake also happens: a "platform" that only ever serves one
consuming team was never really a platform, and treating it as one adds
process overhead (SLA tickets, roadmap negotiation) to what should just be
a direct product-to-product relationship. If Tom's pipeline is only ever
consumed by Ravi's pod a year from now, Amara's plan is to fold it back
into a product-team relationship rather than protect a platform structure
that no longer earns its overhead.

## Exercise

Identify a team in your org (or a function within your own team) that has
drifted toward serving internal customers rather than external ones. Run
the self-service test against its top three capabilities. If it qualifies
as a real platform, sketch a funding model and a success metric that isn't
"features shipped." If it doesn't qualify, name the one product team it
should be re-attached to instead.
