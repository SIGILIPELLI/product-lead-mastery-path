# Coaching PMs on Discovery & Delivery

The strongest pull on a Product Lead is to do the PM job better than the PM
can, and to call that leadership. You spot the bad problem statement, so you
rewrite it. You know the interview question they should have asked, so you
ask it. Each intervention is locally correct and cumulatively disastrous:
you get four squads that can only operate at the speed of your attention,
and four PMs who never developed the judgement you keep supplying.

Coaching is the alternative, and it is slower on any single instance and
enormously faster over a quarter. The mechanic is simple to state and hard
to hold: you intervene on *process and questions*, not on answers. This
module gives you the diagnostic to find where a PM is actually stuck, the
question banks for discovery and delivery, and the rule for when coaching is
the wrong tool entirely.

## Diagnose before you coach

"My PM is struggling with discovery" is four different problems with four
different responses. Guessing wrong wastes months.

| Root cause | How it looks | What it is not | Your move |
|---|---|---|---|
| **Skill** | Genuinely doesn't know how to run an unbiased interview | Not laziness | Teach: model it once, then watch them do it |
| **Confidence** | Knows what to do, waits for permission | Not incompetence | Give explicit authority and a low-stakes rep |
| **Context** | Good process, wrong problem — doesn't know the strategy | Not bad craft | Fix the cascade, not the PM |
| **Capacity** | Knows and can, has no hours | Not prioritisation failure alone | Remove something, publicly |
| **Environment** | Eng lead won't engage with discovery | Not a PM problem at all | Your peer conversation, not their coaching plan |
| **Will** | Doesn't believe discovery is worth it | Not a coaching gap | Performance conversation (Module 3), not coaching |

The last row is the one Leads get wrong most often. Coaching someone who
doesn't want to do the job is a way of avoiding a harder conversation, and
it burns two quarters.

## Coaching discovery: the question bank

Never supply the customer insight. Supply the question that would have
produced it — and let them go find it.

| PM says | Don't say | Ask instead |
|---|---|---|
| "Customers want a bulk-upload feature" | "That's a solution, not a problem" | "What were they doing right before they asked for that? Walk me through the last time you watched someone do it." |
| "I interviewed five customers, they all liked it" | "You led the witness" | "What's the strongest thing anyone said *against* it? If nothing, what would you have to hear to drop this?" |
| "We don't have time for discovery this quarter" | "Make time" | "What's the most expensive thing we could be wrong about here? How cheaply could we find out?" |
| "The data shows drop-off at step 3" | "Go talk to users" | "What are the three possible explanations, and which one would each look different under?" |
| "Sales says we'll lose the deal without it" | "Sales always says that" | "Which deals, what size, and what did those customers do instead when we didn't have it?" |
| "The prototype tested well" | "Define 'well'" | "What did people do that surprised you? Anything you didn't design for?" |
| "I can't get customer time" | "I'll set it up" | "Who inside the company talks to these customers every day, and what would it take to sit in on three of those calls this week?" |

The pattern to internalise: every good coaching question converts a
conclusion back into the evidence it should have rested on. Your PM should
leave the 1:1 with a task, not an answer.

## Coaching delivery: shifting from status to system

Delivery coaching goes wrong when it becomes status-checking with a friendly
face. The distinction is whether you're asking about *this* slip or about
the pattern that produces slips.

| PM's delivery symptom | Status question (avoid) | System question (use) |
|---|---|---|
| Estimates always 1.5× over | "Will it land Friday?" | "Look at your last five items. What category of work is missing from every estimate?" |
| Scope grows mid-sprint | "What got added?" | "Who can add scope without talking to you, and what would it take to change that?" |
| Squad is blocked on another team | "Have you chased them?" | "When did you first know this dependency existed, and what would have surfaced it a month earlier?" |
| Launches are chaotic | "Is the launch plan done?" | "What's on your launch checklist that wasn't there three launches ago? What should be?" |
| Engineers reverse-engineer intent from tickets | "Write better tickets" | "Pick the last ticket an engineer asked you to clarify. What was missing, and is it missing from most of them?" |
| The PM is the bottleneck on every decision | "You need to delegate" | "List last week's decisions. Which ones needed *you* specifically? Push two of them down and tell me what happened." |

## The coaching contract

Vague coaching is unmeasurable and drifts forever. Make it a written,
time-boxed contract — one skill at a time.

| Element | Rule | Example |
|---|---|---|
| One skill | Never more than one at a time | "Framing problems from evidence rather than requests" |
| Observable target | What you'll both see when it's working | "Every roadmap item opens with one line of customer evidence" |
| Reps | The specific practice, with a cadence | "Three customer conversations a week, notes shared Friday" |
| Your role | Exactly what you will and won't do | "I'll review notes and ask questions. I won't rewrite your problem statements." |
| Checkpoint | A date, not "ongoing" | "6 weeks — 15 March" |
| Escalation path | What happens if it doesn't move | "If unchanged, this becomes a performance conversation" |

The "your role" row protects both of you. Without it, you'll drift back into
doing the work, and the PM will reasonably conclude that's the arrangement.

## Worked example: coaching Ravi out of request-taking

Ravi runs Meridian's Onboarding squad. He's well-organised, ships reliably,
and his roadmap is a prioritised queue of things other people asked for.
Amara has been fixing this by rewriting his roadmap items herself before
reviews — for two quarters.

**Diagnosis first.** She runs the table. Not will — Ravi asks for feedback
constantly. Not capacity — his calendar has room. Not environment — his eng
lead is engaged. It's skill plus confidence: he has never seen discovery run
properly (his last company had a research team that handed over findings),
and he treats a stakeholder request as an instruction because saying no to
the partner-success director feels above his pay grade.

**The contract.** One skill: framing problems from evidence. Target: every
roadmap item opens with one line of customer evidence, and at least one item
per month gets killed by discovery. Reps: three customer conversations a
week. Amara's role, stated explicitly: "I will read your notes and ask
questions. I will not rewrite your problem statements any more — including
in reviews, where you may be uncomfortable for a bit." Checkpoint: six
weeks.

**Week 1 — she models once.** Amara runs one customer interview with Ravi
watching, then debriefs on her own mistakes: two leading questions, one
place she should have asked "when did you last do that?" instead of "would
you use this?" Modelling failure teaches more than modelling success.

**Week 2 — the temptation.** Ravi brings a problem statement that is still a
feature request in disguise: "carriers need a bulk-upload tool." Amara has
the correct restatement in her head and does not say it. She asks the
question-bank version: "What were they doing right before they asked for
that?" Ravi doesn't know. He goes and finds out: they were re-keying data
from a TMS export because the field mapping failed silently. The real
problem — silent mapping failures — is bigger than bulk upload and cheaper
to fix.

**Week 4 — the structural fix.** Ravi still can't say no to partner-success.
This isn't a coaching problem; it's an authority problem, and coaching
someone through a structural obstacle is cruel. Amara moves intake to a
monthly triage she attends, and says in that meeting, in front of the
director: "Ravi owns what goes on this roadmap. Bring requests here and he
decides." That single sentence does more than six weeks of 1:1s.

**Week 6 — checkpoint.** Four of six roadmap items now open with customer
evidence; two were killed after discovery. The two items without evidence
are both compliance work, which is legitimate — Amara notes it rather than
forcing the rule. She closes the contract, writes the evidence down for the
performance file, and opens a new one on a different skill: influencing the
eng lead on sequencing.

**The part Amara had to sit with:** in weeks 1-3 the roadmap was visibly
worse than when she was rewriting it. That dip is not a sign the coaching is
failing. It is the cost of transferring the skill, and a Lead who can't
tolerate it will be rewriting roadmaps forever.

## Cheat sheet

| Trap | Correction |
|---|---|
| Supplying the answer because it's faster | Supply the question; they bring the answer next week |
| Coaching a will problem | That's a performance conversation, not coaching |
| Coaching around a structural blocker | Fix the structure yourself; it's your job, not theirs |
| Coaching three skills at once | One skill, one checkpoint, one date |
| "Ongoing" coaching | Every contract has an end date and an escalation path |
| Delivery 1:1s that are status meetings | Ask about the pattern, not this week's slip |
| Rewriting their artefacts before reviews | State that you'll stop, then actually stop |
| Panicking at the quality dip | The dip is the skill transferring; hold it |

## Exercise

Pick one PM you currently over-help.

1. Run the six-row diagnostic honestly. Name the root cause, and write the
   evidence for it. If you land on "will," stop — go to Module 3 instead.
2. Write the coaching contract, all six rows, with a real date. Pay
   particular attention to the "your role" row: name the specific thing you
   do for them that you're going to stop doing.
3. Take three things you said in your last 1:1 with them that were answers.
   Rewrite each as a question from the relevant bank.
4. Identify one structural obstacle in their way that no amount of coaching
   will fix. Write the sentence you'll say, in whose meeting, to remove it.
5. Diary the checkpoint now. At the checkpoint, write down the evidence
   either way — good evidence needs recording at the moment it happens.
