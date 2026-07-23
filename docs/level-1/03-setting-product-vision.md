# 03 · Setting Product Vision for a Team

An IC PM sets vision for a feature or product area. A Product Lead sets
vision for a *team* — a shared narrative that helps three or four PMs, each
owning a different slice, understand how their work fits together and why it
matters. Without this, every PM optimizes locally and the team's combined
output is less than the sum of its parts.

## Vision vs. strategy vs. roadmap

These three get used interchangeably and shouldn't be — mixing them up is
the single most common reason a "vision" doc reads like a to-do list.

| Term | Answers | Time horizon | Changes how often |
|---|---|---|---|
| Vision | Why does this team exist, and what does success look like? | 2-3 years | Rarely (yearly at most) |
| Strategy | Which bets get us there, and why these over the alternatives? | 6-12 months | Quarterly/half-yearly |
| Roadmap | What are we building, in what order? | Weeks to a quarter | Continuously |

A team vision doc should almost never mention a specific feature by name —
if it does, you've probably written a roadmap wearing a vision's clothes.

## The one-page team vision template

| Section | Prompt | Length |
|---|---|---|
| Mission (1 sentence) | Why does this team exist? What would break if it didn't? | 1 sentence |
| Who we serve | Which users/customers/internal stakeholders depend on this team? | 2-3 bullets |
| 2-3 year picture | If we're wildly successful, what's different about the world/product? | 1 short paragraph |
| Why now | What's changed (market, company, technology) that makes this the moment? | 2-3 bullets |
| What we will NOT do | Explicitly out of scope, to prevent scope creep from adjacent teams | 2-3 bullets |
| How each squad ladders up | One line per PM/squad: how their roadmap serves the mission | 1 line per squad |

That last row is the piece unique to a *team* vision (an IC PM's vision
doesn't need it) — it's the thing that turns three independent roadmaps into
one coherent story.

## Worked example: a payments team's vision doc

**Mission:** Make it as easy to get paid as it is to pay — for every seller
on our marketplace, regardless of size or country.

**Who we serve:** Sellers processing their first transaction; established
sellers scaling into new markets; internal support teams handling payment
disputes.

**2-3 year picture:** A seller in any supported country can start accepting
payments in under 5 minutes, with dispute resolution times cut by 70% through
automation, and payment failure rates below 1% globally.

**Why now:** We're expanding into 3 new countries this year, and payment
failures are currently our #1 driver of seller churn in month one.

**What we will NOT do:** We are not building a general-purpose banking
product; we are not solving invoicing or accounting — only the pay-in/pay-out
transaction itself.

**How each squad ladders up:**

| Squad | PM | How it serves the mission |
|---|---|---|
| Onboarding | Maria | Cuts time-to-first-transaction |
| Reliability | Sam | Drives payment failure rate down |
| Disputes | Jordan | Automates resolution, cuts support load |

Any PM on this team can now explain, in one sentence, how their work connects
to the other two squads' work — that's the test of whether the vision doc
did its job.

## Common failure modes

| Symptom | Likely cause | Fix |
|---|---|---|
| PMs can't explain the vision in their own words | It's too abstract, or too long | Cut it to fit on one page; workshop the mission sentence with the team, don't hand it down |
| Vision reads identically to last year's | No "why now" — it's generic instead of tied to a real moment | Anchor to a specific market/company change |
| Squads' roadmaps don't obviously connect to the mission | Vision was written without mapping it to actual current initiatives | Rewrite the "how each squad ladders up" section with real, current squad names |

## Exercise

Write a one-page team vision doc using the template above for a team you
lead (or a hypothetical 3-squad team of your choosing — e.g., a "search and
discovery" team with squads for search relevance, recommendations, and
browse/category pages). Then test it: read only the mission sentence and the
"how each squad ladders up" table to someone unfamiliar with the team, and
ask them to explain back, in their own words, what the team is trying to
achieve. If they can't, revise the mission sentence until they can.
