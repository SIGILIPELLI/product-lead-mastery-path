# Product Culture & Rituals at Scale

When Meridian's product org was eight people, culture was whatever Amara
modeled in the room — she showed up prepared, admitted when she was wrong,
and everyone absorbed it by osmosis. At eighteen people across five pods,
osmosis stops reaching the back rows. Dana's newest PM has never seen Amara
run a retro. Sofia's Marketplace pod, under growth pressure, has quietly
started skipping postmortems because "we're moving too fast." Culture at
scale has to become a set of deliberately designed rituals, because
implicit culture decays at the edges of the org first and nobody notices
until it's already gone.

## Rituals as culture infrastructure

A ritual is a repeated, structured practice that encodes a value so it
survives without a founder in the room. Each one should trace to a
specific value Amara wants to protect as Meridian scales.

| Ritual | Cadence | Value it encodes | Failure mode if dropped |
|---|---|---|---|
| Blameless postmortem | After every P1/P2 incident | Learning over blame | Root causes hide, same failure repeats |
| Cross-pod demo | Monthly, all pods present | Visibility, shared context | Pods drift into silos, duplicate work |
| Decision log review | Quarterly, per pod | Explicit reasoning over gut calls | Decisions become untraceable, hard to audit |
| New-PM culture onboarding | Week 1 for every hire | Deliberate culture transfer | New hires absorb whatever their immediate pod happens to model |
| "What did we kill" review | Quarterly, org-wide | Honest prioritization over sunk cost | Zombie projects accumulate, nobody owns closing them |

## Diagnosing culture drift before it's visible in metrics

Culture problems show up in engagement scores only after they've already
cost real damage. Amara watches leading indicators instead:

| Leading indicator | What it signals | Source |
|---|---|---|
| Postmortems getting shorter/skipped | Blame culture creeping back, or just burnout | Ritual attendance logs |
| Cross-pod demo attendance dropping | Pods siloing | Calendar data, informal check |
| New PMs asking Amara things their Lead should have covered | Onboarding ritual not landing | 1:1s with new hires at 30/60/90 days |
| Decision logs getting vaguer ("team decided") | Accountability diffusing | Spot-check of decision logs per pod |
| Same idea killed and revived by different pods | No shared memory of past decisions | Post-hoc pattern noticing |

## Worked example: Sofia's pod skipping postmortems

Amara notices Marketplace hasn't logged a postmortem in six weeks, despite
two incidents in that window. She doesn't send a policy reminder — that
fixes compliance, not the culture. Instead:

1. **Diagnoses the real driver.** In a 1:1, Sofia admits the postmortems
   felt like overhead against an aggressive growth timeline, and the last
   one before that turned into finger-pointing about the API rate-limiting
   incident, which made the team dread the next one.
2. **Fixes the actual failure, not the symptom.** The problem isn't
   Sofia's pod being lazy — it's that the last postmortem wasn't actually
   blameless, so the ritual now carries a cost the team wants to avoid.
   Amara re-trains the format with Sofia: postmortems open with "what did
   the system/process allow to happen," never "who did this."
3. **Models it herself once.** Amara joins the next Marketplace postmortem
   as a participant, not an observer, and explicitly redirects one comment
   that starts drifting toward blaming an individual engineer.
4. **Makes the value visible in a decision that costs something.** Two
   weeks later, an engineer on Sofia's pod admits a mistake that caused a
   near-miss, unprompted, in a postmortem. Amara publicly credits the
   disclosure rather than treating it as a confession — because how she
   reacts to the first honest mistake after a culture fix is the actual
   test of whether the value is real.

## Culture at scale requires designed redundancy

At eight people, if the value only lives in Amara's head, that's fine —
she's in every room. At eighteen-plus, any value that isn't written down,
modeled by multiple Leads independently, and checked for in hiring will
silently narrow to "whatever Amara personally polices," which doesn't
scale past her calendar. The fix is redundancy:

| Layer | Mechanism |
|---|---|
| Written | A short (one-page) product culture doc — actual behaviors, not aspirational adjectives |
| Modeled by multiple people | Every Lead, not just Amara, visibly practices each ritual |
| Hired for | Interview loops probe for it explicitly (see Level 2 hiring module) |
| Reinforced in review | Career ladder evidence packets (Module 4) include a culture-fit section with specifics |
| Protected under pressure | Leadership doesn't quietly waive rituals during crunch — that's when they matter most |

## Exercise

List the three rituals your team or org currently runs (formally or
informally) and name the value each one is supposed to protect. Pick one
that's decaying — attendance dropping, going through the motions, or
already dead — and diagnose the real driver using the approach above, not
the surface symptom. Write the specific intervention you'd try before
reaching for a policy reminder.
