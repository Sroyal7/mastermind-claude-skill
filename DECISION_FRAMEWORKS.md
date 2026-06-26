# Mastermind + Decision Frameworks: The Full Stack

> "The Professor didn't just have a plan. He had a plan for when the plan failed."

Mastermind gives you fast strategic reads. Decision Frameworks give you structured depth for high-stakes calls. Together they cover everything from a 30-second tactical take to a full irreversibility audit before you commit.

---

## When to use which

| Situation | Use |
|---|---|
| Quick strategic read, moderate stakes | Mastermind only (`/mastermind`) |
| High-stakes, irreversible decision | Mastermind → Decision Frameworks |
| Plan you're emotionally attached to | Mastermind flags it, `/premortem` + `/redteam` break it |
| Real-time, fast-moving situation | Mastermind → `/ooda` |
| You don't know what you don't know | Mastermind → `/blindspot` |
| Competing options with unclear trade-offs | Mastermind → `/quantify` or `/scenarios` |
| Adversary or competitor involved | Mastermind → `/wargame` or `/redteam` |

**Default rule:** Start with Mastermind. If the decision is irreversible or the stakes are high, escalate to Decision Frameworks.

---

## The 20 Decision Framework Slash Commands

Install the decision-frameworks skill alongside this one. Then use:

```
/gate          Are the facts good enough, or do we need evidence first?
/baserates     What usually happens to decisions like this? (outside view)
/premortem     What kills this if we commit?
/redteam       How would a capable adversary break this?
/swot          Where do we stand strategically?
/ooda          What do we do right now in a fast-moving situation?
/invert        What behaviors guarantee failure?
/pareto        Where is 80% of impact or risk concentrated?
/quantify      What do the probabilities × magnitudes actually say?
/wargame       How will competitors respond to our move, round by round?
/scenarios     What do we do if the future looks like X vs Y vs Z?
/bottleneck    What is the ONE constraint throttling everything?
/leverage      Which single intervention cascades into systemic change?
/blindspot     What haven't we even thought to consider?
/deepreason    Full causal chain — why does this happen?
/layered       Peel back the layers — what's really going on?
/overthink     Full adversarial analysis — no assumption is safe
/council       What would different expert perspectives say?
/coalition     Who needs to align for this to work?
/log           Decision log — what did we commit to and why?
```

---

## The Standard Protocol for Hard Decisions

This is the sequence that makes the combination work.

**Step 1 — Mastermind fast read**
Run `/mastermind`. Get the reframe, the challenged assumption, the downstream consequences, and the calibrated recommendation. Most decisions end here.

**Step 2 — Gate check**
If the decision is irreversible, run `/gate` first. If the facts aren't solid enough to analyze, stop and gather them. Structured thinking on bad facts produces confident-sounding garbage.

**Step 3 — Anchor to base rates**
Run `/baserates`. Before the inside-view analysis, ask what usually happens to decisions like yours. The Professor knew the statistics on heist success rates. You should know yours.

**Step 4 — Stress test**
Pick 1–2 frameworks based on the risk type:
- Risk of failure? `/premortem`
- External adversary? `/redteam` or `/wargame`
- Unknown unknowns? `/blindspot`
- Competing options? `/scenarios` or `/quantify`

**Step 5 — Land the call**
Every analysis ends with a recommendation: what to do, the confidence level (Verified / Reasoned / Assumed / Unknown), and what new information would change the answer.

---

## Before/After: Job Quitting Decision

### Without the full stack

> "I want to quit my job and go freelance. Should I?"
>
> Claude: "That depends on your financial situation, risk tolerance, and skills. Many people successfully transition to freelance work. Consider your savings runway, your client pipeline, and your personal goals..."

Hedge-everything non-answer. No useful signal.

### With Mastermind + Decision Frameworks

> **Mastermind fast read:**
> The real question isn't whether to quit — it's whether the conditions for a successful freelance launch currently exist. Three things determine that: financial runway (6+ months), proof of external demand (someone not your current employer has paid you), and a reason the timing is now rather than in 6 months.
>
> **Challenge:** You're assuming freelance income will replace employment income on a similar timeline. That assumption is wrong for 70% of first-year freelancers. (Reasoned)
>
> **Recommendation:** Don't quit yet. Validate demand first — land one paid client while still employed. If you can't do that, quitting doesn't solve the problem.
>
> ---
>
> **`/premortem`:** Fast-forward 12 months. The launch failed. Most likely cause: no clients in pipeline at launch, savings ran out at month 4, returned to employment at a lower level. Prevention: don't quit until you have 2 paying clients and 6 months runway.
>
> **`/baserates`:** First-year freelancers sustain themselves within 12 months at roughly 30-40% success rates, conditional on starting with existing client relationships. Without any pre-existing pipeline: closer to 15%. (Assumed — verify for your field.)
>
> **Final call:** Validate externally before leaving. Set a 90-day test: land one paying client outside your employer. If you hit it, the decision to leave becomes easy. If you don't, you've learned something important before it cost you.

---

## Installing Both Skills

**Option A — Claude Cowork (recommended)**
Install both `.skill` files from Settings > Capabilities > Skills:
- `mastermind.skill` — this repo
- Get `decision-frameworks.skill` from the decision-frameworks repo

**Option B — Manual**
Copy `SKILL.md` from each repo into your Claude Cowork skills directory.

Once installed, both are active in every session. Use `/mastermind` for the fast read, then any `/` decision command when you need structured depth.

---

## The Underlying Principle

Mastermind is fast, pattern-based, and calibrated to the problem weight. Decision Frameworks are slow, structured, and exhaustive. The error most people make is using slow tools for fast problems and fast tools for slow problems.

The Professor was fast when speed mattered and methodical when failure was not an option. Match the tool to the stakes.
