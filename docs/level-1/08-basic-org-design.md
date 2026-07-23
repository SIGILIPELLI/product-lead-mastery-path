# 08 · Basic Org Design for Product Teams

How you split up product work across squads shapes almost everything
downstream — who talks to whom daily, where dependencies pile up, and how
clean or muddy ownership feels to a customer. This module covers the basic
shapes a small product org can take; Level 3 (Module 3, Org Design at Scale)
returns to this at the multi-team, Head-of-Product level.

## Common ways to slice up a product org

| Model | Squads split by | Strength | Weakness |
|---|---|---|---|
| By customer journey stage | Onboarding, activation, retention, monetization | Matches how users move through the product | Handoffs between stages can get muddy |
| By customer segment | SMB, mid-market, enterprise | Deep expertise in one segment's needs | Duplicate work if segments need similar features |
| By platform | Web, iOS, Android | Deep platform expertise | Feature parity across platforms takes coordination |
| By feature area | Search, checkout, notifications | Clear technical ownership | Can silo teams from the end-to-end user experience |
| Platform vs. product | "Platform" squad building shared infrastructure, "product" squads building user-facing features | Prevents product squads reinventing infra | Platform team can feel disconnected from user impact (see Level 3, Module 8) |

There's no universally "correct" model — the right one depends on your
company's stage, where your biggest risk currently is (coordination
overhead vs. duplicated effort vs. unclear ownership), and how mature your
product is.

## A basic org design worksheet

| Question | Your answer shapes... |
|---|---|
| What's the #1 source of friction today? (Duplicated work? Unclear ownership? Slow handoffs?) | Which model addresses that friction directly |
| How many PMs do you have, and how many can one Lead realistically support (usually 3-6)? | Whether you need one team or multiple sub-teams |
| Where do users cross squad boundaries most? | Where you'll need the strongest alignment rituals (Module 5) |
| What's likely to change in the next 12 months (new market, new platform, new segment)? | Whether your design will need to be revisited soon |

## Worked example: reorganizing around a real friction point

A 4-PM team at a B2B SaaS company is organized by feature area: one PM each
for "reporting," "integrations," "admin settings," and "notifications." The
Product Lead notices a recurring complaint from customers: enterprise
prospects churn during onboarding because integrations, admin settings, and
notifications all need to be configured together for a single enterprise
rollout, and no one PM owns that end-to-end experience. Applying the
worksheet: the #1 friction is unclear ownership of a cross-cutting journey
(enterprise onboarding), not duplicated work or platform fragmentation. The
Lead doesn't fully reorganize (four feature-area PMs is otherwise working
fine) — instead, they designate one PM as the "enterprise onboarding"
owner for a defined project window, with the other three contributing their
piece under that PM's coordination. This is a lightweight, reversible
structural fix rather than a full re-org, appropriate for a friction point
that's specific rather than systemic.

## Cheat sheet — when to consider a re-org

| Signal | What it suggests |
|---|---|
| Multiple squads keep duplicating similar work | Consider consolidating by segment or feature area |
| A cross-cutting user journey has no clear owner | Consider a journey-stage or temporary cross-squad ownership model |
| One squad is a constant bottleneck for others' launches | Consider a platform/product split (Level 3, Module 8) |
| The org design hasn't changed in 2+ years despite major product growth | Worth revisiting even without an acute crisis |

## Exercise

Take a real or hypothetical product org of 4-6 PMs. Write down which of the
five models above currently (or would) best describe how it's organized.
Identify the single biggest friction point this structure creates, and
propose one concrete, reversible change (not a full re-org) that would
reduce it — following the worked example's approach of a targeted fix over a
wholesale restructure.
