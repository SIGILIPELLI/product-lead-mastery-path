# 05 · Cross-Team Alignment Basics

Once you lead more than one PM, misalignment stops being an occasional
annoyance and becomes a structural risk: two squads can quietly build
competing solutions, or one squad's roadmap can depend on another's without
anyone flagging it until a launch is blocked. This module covers the basic
mechanics of keeping several squads pointed the same direction — the
deeper, multi-team version of this shows up again in Level 2 (Module 4,
Cross-Functional Leadership) and Level 3 (Module 3, Org Design at Scale).

## Where misalignment actually comes from

| Source | Example | Typical fix |
|---|---|---|
| Hidden dependencies | Squad A's Q3 feature silently needs an API only Squad B is building | A shared dependency log, reviewed at planning |
| Duplicate effort | Two squads both start solving "improve onboarding conversion" independently | A visible initiative list, checked before kickoff |
| Conflicting metrics | Squad A is measured on speed-to-checkout, Squad B on fraud reduction — they optimize against each other | Metrics reviewed together at the Lead level; make trade-offs explicit rather than let squads fight it out silently |
| Stale information | A PM makes a decision based on a plan that changed weeks ago in another squad's planning | A regular (not ad hoc) cross-squad sync |

## The dependency log — a lightweight tool

A simple shared table, reviewed at every planning cycle, prevents most
silent collisions:

| Initiative | Owning squad | Depends on | Status of dependency | Risk if late |
|---|---|---|---|---|
| One-click reorder | Checkout | Saved Payment Methods (Payments squad) | On track for Sprint 14 | Reorder launch slips 2 sprints |
| Bulk seller onboarding | Onboarding | New KYC API (Trust & Safety squad) | At risk — no ETA yet | Cannot commit to a launch date |

As Product Lead, you don't need to track every task — you need to catch
the handful of cross-squad dependencies that could silently blow up a
commitment, and surface them before they do.

## Running a cross-squad alignment sync

| Element | Recommendation |
|---|---|
| Cadence | Biweekly is usually enough; weekly only if squads are tightly coupled right now |
| Attendees | One PM per squad (not full squads) — keep it small enough to move fast |
| Agenda | (1) Dependency log review (2) Any new overlapping initiatives (3) One roadblock each squad needs help with |
| Length | 30 minutes, hard stop — this is a sync, not a planning meeting |
| Anti-pattern to avoid | Turning it into status theater where each PM reads their roadmap aloud with no cross-squad content |

## Worked example: catching a collision before it ships

At a biweekly sync, the Onboarding PM mentions in passing that they're
building an in-app "getting started" checklist. The Growth PM, previously
silent, realizes their team shipped something similar six months ago that
quietly got no adoption because it launched with no promotion. Because this
surfaced in the sync rather than after both were built, the Product Lead
redirects: Onboarding will extend the existing Growth-owned checklist
component rather than build a second one, and the two PMs agree on which
team owns it going forward. Cost of catching it here: one sync. Cost of not
catching it: a duplicated feature and an awkward conversation about which
one users see.

## Cheat sheet

| Symptom | Diagnosis | Tool to use |
|---|---|---|
| "I didn't know they were also building that" | No shared initiative visibility | Dependency log + alignment sync |
| A launch slips because another squad's piece wasn't ready | Dependency wasn't tracked/flagged early | Add it to the dependency log at planning, not after |
| Two squads are quietly working against each other's metrics | Conflicting incentives, not a communication problem | Resolve the trade-off explicitly at the Lead level |

## Exercise

For a team of 2-3 squads (real or hypothetical), build a dependency log with
at least 3 real or plausible cross-squad dependencies, following the table
format above. Then draft a 30-minute alignment-sync agenda for that team
using the cadence/attendees/agenda structure above, and write two sentences
on the single most likely collision you'd expect between these squads in
their next quarter — and how the sync would catch it.
