---
title: "Final Quiz"
description: "Test what you have learned across all four levels of Product Lead Mastery Path with a 19-question final quiz."
---

# Final Quiz

19 questions drawn from all four levels of this course. You need **70% (14 out of 19)** to pass —
you can retake it as many times as you like. Your best result is saved in this browser.

<div id="mp-quiz-root"></div>

<script type="application/json" id="mp-quiz-data">
[
  {
    "question": "A PM's ratings are based on 'good attitude' and 'strong communicator'. What is wrong?",
    "options": [
      "They are impressions, not behaviours with evidence; use a rubric with two written examples",
      "Too detailed",
      "Too formal",
      "Nothing"
    ],
    "correctIndex": 0,
    "explanation": "Behavioural descriptors."
  },
  {
    "question": "A PM underperformed for three quarters and has never heard it from you. Whose failure is it first?",
    "options": [
      "HR",
      "Team",
      "PM",
      "Yours: timely feedback is part of the lead's job"
    ],
    "correctIndex": 3,
    "explanation": "Management failure."
  },
  {
    "question": "Your two best PMs disagree on a roadmap trade-off and escalate to you. What do you do?",
    "options": [
      "Delay",
      "Pick one",
      "Vote",
      "Bring them together, anchor on the goal and metric, and clarify who decides"
    ],
    "correctIndex": 3,
    "explanation": "Decision rights."
  },
  {
    "question": "You delegated a pricing test and disagree with the PM's call after the fact. What do you do?",
    "options": [
      "Coach on reasoning and learn from results unless it breaches guardrails",
      "Blame",
      "Reverse",
      "Ignore"
    ],
    "correctIndex": 0,
    "explanation": "Preserve ownership."
  },
  {
    "question": "A team's weekly review is mostly status updates. What change helps most?",
    "options": [
      "Move status to a written update and use the meeting for decisions",
      "Shorter",
      "More slides",
      "Cancel"
    ],
    "correctIndex": 0,
    "explanation": "Decision forum."
  },
  {
    "question": "A candidate is brilliant in one interview and weak in two others. What does a structured process say?",
    "options": [
      "Average",
      "Hire",
      "Reject",
      "Compare against the scorecard and calibrate interviewers before deciding"
    ],
    "correctIndex": 3,
    "explanation": "Evidence."
  },
  {
    "question": "You have 10 direct reports who all need weekly coaching. What is the issue?",
    "options": [
      "Fine",
      "Span of control is too large to coach well; restructure",
      "Delegate",
      "Hire more"
    ],
    "correctIndex": 1,
    "explanation": "5–8 is typical."
  },
  {
    "question": "A company OKR is 'improve retention'. A team's top goal is a new dashboard. What do you do?",
    "options": [
      "Ignore",
      "Cancel",
      "Approve",
      "Check the link to the strategy and re-derive goals if it doesn't connect"
    ],
    "correctIndex": 3,
    "explanation": "Cascade."
  },
  {
    "question": "A high-performing PM is rude to engineers. What do you do?",
    "options": [
      "Address the behavior directly; standards apply to everyone",
      "Move",
      "Praise",
      "Ignore"
    ],
    "correctIndex": 0,
    "explanation": "Culture."
  },
  {
    "question": "The CEO wants a feature you believe will hurt retention. What do you do?",
    "options": [
      "Build quietly",
      "Refuse",
      "Share evidence and alternatives, then commit if they decide",
      "Escalate"
    ],
    "correctIndex": 2,
    "explanation": "Disagree and commit."
  },
  {
    "question": "A platform team's adoption is low. What does that suggest?",
    "options": [
      "Low budget",
      "Bad tech",
      "They may not treat product teams as customers or understand their needs",
      "Wrong tool"
    ],
    "correctIndex": 2,
    "explanation": "Product mindset."
  },
  {
    "question": "After an acquisition two products overlap. What is the biggest mistake?",
    "options": [
      "Integrating",
      "Delaying decisions about the overlap and leaving teams in limbo",
      "Talking",
      "Deciding"
    ],
    "correctIndex": 1,
    "explanation": "Ambiguity."
  },
  {
    "question": "A board member challenges your strategy. What helps most?",
    "options": [
      "Engage with evidence, acknowledge uncertainty and clarify trade-offs",
      "Concede",
      "Defer",
      "Defend"
    ],
    "correctIndex": 0,
    "explanation": "Trust."
  },
  {
    "question": "You must cut 20% of budget. What principle guides you?",
    "options": [
      "Random",
      "Equal cuts",
      "Protect work most tied to strategy and customer outcomes, cut the rest explicitly",
      "Delay"
    ],
    "correctIndex": 2,
    "explanation": "Prioritize."
  },
  {
    "question": "A new PM is struggling in month two. What is the best first step?",
    "options": [
      "Reassign",
      "PIP",
      "Ignore",
      "Check expectations, context and support, then give specific feedback"
    ],
    "correctIndex": 3,
    "explanation": "Early help."
  },
  {
    "question": "What does a leadership pipeline need to work?",
    "options": [
      "Titles",
      "Stretch assignments, coaching and feedback for future leaders",
      "Time",
      "Courses only"
    ],
    "correctIndex": 1,
    "explanation": "Develop."
  },
  {
    "question": "How do you keep global teams aligned?",
    "options": [
      "Full local",
      "Random",
      "Global standards for strategy and quality, local autonomy where context matters",
      "Central control"
    ],
    "correctIndex": 2,
    "explanation": "Balance."
  },
  {
    "question": "What is the main risk of adopting AI tools without evaluation?",
    "options": [
      "Cost",
      "Speed",
      "Fun",
      "Over-trusting outputs and weakening judgement"
    ],
    "correctIndex": 3,
    "explanation": "Verify."
  },
  {
    "question": "What signals a healthy product culture?",
    "options": [
      "Candid reviews, documented decisions and customer contact",
      "Slogans",
      "Parties",
      "Perks"
    ],
    "correctIndex": 0,
    "explanation": "Observable."
  }
]
</script>

## Coding challenges

Try these on your own computer, then compare your output. Nothing you write is sent anywhere.

### A structured hiring scorecard with calibration

Implement weighted() and evaluate() for a PM hiring loop: independent interviewer scores are combined with dimension weights, a large spread between interviewers triggers calibration, otherwise the candidate needs both a passing average and no weak dimension. Rank the candidates.

**Starter code**

```python
# Structured hiring: weighted scorecard, calibration of interviewers, and a hire / no-hire recommendation.
WEIGHTS = {"outcomes": 0.35, "judgement": 0.30, "craft": 0.20, "influence": 0.15}
# scores 1-4 per interviewer (independent, written before the debrief)
FEEDBACK = {
    "Asha":  {"ann": {"outcomes": 4, "judgement": 3, "craft": 3, "influence": 3}, "ben": {"outcomes": 2, "judgement": 2, "craft": 3, "influence": 2}, "cy": {"outcomes": 3, "judgement": 4, "craft": 3, "influence": 4}},
    "Raj":   {"ann": {"outcomes": 3, "judgement": 3, "craft": 4, "influence": 3}, "ben": {"outcomes": 4, "judgement": 4, "craft": 3, "influence": 3}, "cy": {"outcomes": 3, "judgement": 3, "craft": 3, "influence": 3}},
    "Mei":   {"ann": {"outcomes": 4, "judgement": 4, "craft": 3, "influence": 4}, "ben": {"outcomes": 2, "judgement": 1, "craft": 2, "influence": 2}, "cy": {"outcomes": 4, "judgement": 3, "craft": 4, "influence": 3}},
}
BAR = 3.0          # weighted average needed to hire
MAX_SPREAD = 1.5   # interviewers differing by more than this need a calibration conversation

def weighted(scores):
    # weighted sum of the four dimension scores
    return 0

def evaluate(candidate):
    # per-interviewer weighted score, then: avg (round 2), spread = max - min (round 2),
    # weakest = dimension with the lowest average across interviewers,
    # decision: "CALIBRATE" if spread > MAX_SPREAD, else "HIRE" if avg >= BAR and the weakest dimension average >= 2.5, else "NO HIRE"
    return {"avg": 0, "spread": 0, "weakest": "", "decision": ""}

for c in ["ann", "ben", "cy"]:
    r = evaluate(c)
    print(f"{c:4s} avg={r['avg']:.2f} spread={r['spread']:.2f} weakest={r['weakest']:<9s} -> {r['decision']}")
ranking = sorted(["ann", "ben", "cy"], key=lambda c: -evaluate(c)["avg"])
print("ranking:", " > ".join(ranking))
```

**Expected output**

```text
ann  avg=3.45 spread=0.60 weakest=judgement -> HIRE
ben  avg=2.52 spread=1.95 weakest=judgement -> CALIBRATE
cy   avg=3.33 spread=0.55 weakest=outcomes  -> HIRE
ranking: ann > cy > ben
```

<details><summary>Show solution and explanation</summary>

<pre><code># Structured hiring: weighted scorecard, calibration of interviewers, and a hire / no-hire recommendation.
WEIGHTS = {&quot;outcomes&quot;: 0.35, &quot;judgement&quot;: 0.30, &quot;craft&quot;: 0.20, &quot;influence&quot;: 0.15}
# scores 1-4 per interviewer (independent, written before the debrief)
FEEDBACK = {
    &quot;Asha&quot;:  {&quot;ann&quot;: {&quot;outcomes&quot;: 4, &quot;judgement&quot;: 3, &quot;craft&quot;: 3, &quot;influence&quot;: 3}, &quot;ben&quot;: {&quot;outcomes&quot;: 2, &quot;judgement&quot;: 2, &quot;craft&quot;: 3, &quot;influence&quot;: 2}, &quot;cy&quot;: {&quot;outcomes&quot;: 3, &quot;judgement&quot;: 4, &quot;craft&quot;: 3, &quot;influence&quot;: 4}},
    &quot;Raj&quot;:   {&quot;ann&quot;: {&quot;outcomes&quot;: 3, &quot;judgement&quot;: 3, &quot;craft&quot;: 4, &quot;influence&quot;: 3}, &quot;ben&quot;: {&quot;outcomes&quot;: 4, &quot;judgement&quot;: 4, &quot;craft&quot;: 3, &quot;influence&quot;: 3}, &quot;cy&quot;: {&quot;outcomes&quot;: 3, &quot;judgement&quot;: 3, &quot;craft&quot;: 3, &quot;influence&quot;: 3}},
    &quot;Mei&quot;:   {&quot;ann&quot;: {&quot;outcomes&quot;: 4, &quot;judgement&quot;: 4, &quot;craft&quot;: 3, &quot;influence&quot;: 4}, &quot;ben&quot;: {&quot;outcomes&quot;: 2, &quot;judgement&quot;: 1, &quot;craft&quot;: 2, &quot;influence&quot;: 2}, &quot;cy&quot;: {&quot;outcomes&quot;: 4, &quot;judgement&quot;: 3, &quot;craft&quot;: 4, &quot;influence&quot;: 3}},
}
BAR = 3.0          # weighted average needed to hire
MAX_SPREAD = 1.5   # interviewers differing by more than this need a calibration conversation

def weighted(scores):
    return sum(scores[k] * w for k, w in WEIGHTS.items())

def evaluate(candidate):
    per = {i: weighted(FEEDBACK[i][candidate]) for i in FEEDBACK}
    avg = sum(per.values()) / len(per)
    spread = max(per.values()) - min(per.values())
    dims = {k: round(sum(FEEDBACK[i][candidate][k] for i in FEEDBACK) / len(FEEDBACK), 2) for k in WEIGHTS}
    weakest = min(dims, key=dims.get)
    if spread &gt; MAX_SPREAD:
        decision = &quot;CALIBRATE&quot;
    elif avg &gt;= BAR and dims[weakest] &gt;= 2.5:
        decision = &quot;HIRE&quot;
    else:
        decision = &quot;NO HIRE&quot;
    return {&quot;avg&quot;: round(avg, 2), &quot;spread&quot;: round(spread, 2), &quot;weakest&quot;: weakest, &quot;decision&quot;: decision}

for c in [&quot;ann&quot;, &quot;ben&quot;, &quot;cy&quot;]:
    r = evaluate(c)
    print(f&quot;{c:4s} avg={r[&#x27;avg&#x27;]:.2f} spread={r[&#x27;spread&#x27;]:.2f} weakest={r[&#x27;weakest&#x27;]:&lt;9s} -&gt; {r[&#x27;decision&#x27;]}&quot;)
ranking = sorted([&quot;ann&quot;, &quot;ben&quot;, &quot;cy&quot;], key=lambda c: -evaluate(c)[&quot;avg&quot;])
print(&quot;ranking:&quot;, &quot; &gt; &quot;.join(ranking))
</code></pre>

<p>Independent written scores avoid anchoring; weighting reflects what the role needs; the spread check catches disagreement that should be discussed rather than averaged away. Verified by running the Python model (the thresholds are illustrative, not a standard).</p>
</details>

### Capacity planning: PMs, leads and budget

Implement pms_needed, leads_needed and plan() to decide which bets a budget can fund in priority order, counting the PMs and the Product Leads (span of control) they require. Then see how much extra budget funds more bets.

**Starter code**

```python
# Org capacity model: how many PMs/leads are needed for a set of bets, and what does it cost?
import math
BETS = [  # (name, engineers needed, priority 1=highest)
    ("Checkout redesign", 14, 1), ("Onboarding", 9, 1), ("Search relevance", 11, 2), ("Partner API", 8, 2), ("Mobile app", 15, 3), ("Insights", 6, 3),
]
ENG_PER_PM = 7              # one PM per ~7 engineers (rounded up per bet)
SPAN = 6                    # direct reports per Product Lead
PM_COST, LEAD_COST, RECRUIT = 160_000, 200_000, 0.20     # annual cost and recruiting fee as a share of salary
BUDGET = 1_300_000

def pms_needed(engineers):
    # PMs for a bet: engineers / ENG_PER_PM rounded up
    return 0

def leads_needed(pm_count):
    # Product Leads for that many PMs: pm_count / SPAN rounded up
    return 0

def plan(bets, budget):
    # go through bets by (priority, engineers); fund a bet only if the TOTAL cost after adding it
    # (all PMs at PM_COST + all leads at LEAD_COST) stays within budget.
    # return (list of (name, pms for that bet), total PMs, total annual cost)
    return [], 0, 0

funded, pms, spent = plan(BETS, BUDGET)
print("funded:", ", ".join(f"{n} ({p} PM)" for n, p in funded))
print("unfunded:", ", ".join(n for n, _, _ in BETS if n not in {f for f, _ in funded}) or "none")
print(f"PMs: {pms}, leads: {leads_needed(pms)}, annual cost: {spent:,}")
print(f"recruiting fees: {round((pms * PM_COST + leads_needed(pms) * LEAD_COST) * RECRUIT):,}")
print(f"headroom: {BUDGET - spent:,}")
for extra in (0, 300_000, 600_000):
    print(f"budget +{extra:,} ->", len(plan(BETS, BUDGET + extra)[0]), "bets funded")
```

**Expected output**

```text
funded: Onboarding (2 PM), Checkout redesign (2 PM), Partner API (2 PM)
unfunded: Search relevance, Mobile app, Insights
PMs: 6, leads: 1, annual cost: 1,160,000
recruiting fees: 232,000
headroom: 140,000
budget +0 -> 3 bets funded
budget +300,000 -> 4 bets funded
budget +600,000 -> 5 bets funded
```

<details><summary>Show solution and explanation</summary>

<pre><code># Org capacity model: how many PMs/leads are needed for a set of bets, and what does it cost?
import math
BETS = [  # (name, engineers needed, priority 1=highest)
    (&quot;Checkout redesign&quot;, 14, 1), (&quot;Onboarding&quot;, 9, 1), (&quot;Search relevance&quot;, 11, 2), (&quot;Partner API&quot;, 8, 2), (&quot;Mobile app&quot;, 15, 3), (&quot;Insights&quot;, 6, 3),
]
ENG_PER_PM = 7              # one PM per ~7 engineers (rounded up per bet)
SPAN = 6                    # direct reports per Product Lead
PM_COST, LEAD_COST, RECRUIT = 160_000, 200_000, 0.20     # annual cost and recruiting fee as a share of salary
BUDGET = 1_300_000

def pms_needed(engineers):
    return math.ceil(engineers / ENG_PER_PM)

def leads_needed(pm_count):
    return math.ceil(pm_count / SPAN)

def plan(bets, budget):
    funded, spent, pms = [], 0, 0
    for name, eng, prio in sorted(bets, key=lambda b: (b[2], b[1])):
        need = pms_needed(eng)
        total_pm = pms + need
        cost = total_pm * PM_COST + leads_needed(total_pm) * LEAD_COST
        if cost &lt;= budget:
            funded.append((name, need)); pms, spent = total_pm, cost
    return funded, pms, spent

funded, pms, spent = plan(BETS, BUDGET)
print(&quot;funded:&quot;, &quot;, &quot;.join(f&quot;{n} ({p} PM)&quot; for n, p in funded))
print(&quot;unfunded:&quot;, &quot;, &quot;.join(n for n, _, _ in BETS if n not in {f for f, _ in funded}) or &quot;none&quot;)
print(f&quot;PMs: {pms}, leads: {leads_needed(pms)}, annual cost: {spent:,}&quot;)
print(f&quot;recruiting fees: {round((pms * PM_COST + leads_needed(pms) * LEAD_COST) * RECRUIT):,}&quot;)
print(f&quot;headroom: {BUDGET - spent:,}&quot;)
for extra in (0, 300_000, 600_000):
    print(f&quot;budget +{extra:,} -&gt;&quot;, len(plan(BETS, BUDGET + extra)[0]), &quot;bets funded&quot;)
</code></pre>

<p>Capacity is derived from bets (engineers per PM, PMs per lead) and funded in priority order until the budget binds, making trade-offs explicit. Verified by running the Python model (the ratios and salaries are illustrative assumptions).</p>
</details>
