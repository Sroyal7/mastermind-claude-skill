# Mastermind + Decision Frameworks: The Full Stack

> "The Professor didn't just have a plan. He had a plan for when the plan failed."

Mastermind gives you fast strategic reads. Decision Frameworks give you structured depth for high-stakes calls. Together they cover everything from a 30-second tactical take to a full irreversibility audit before you commit.

---

## When to Use Which

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

## The 20 Slash Commands

Install the decision-frameworks skill alongside this one. Then:

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

## The 5-Step Protocol for Hard Decisions

**Step 1 — Mastermind fast read**
Run `/mastermind`. Get the reframe, the challenged assumption, the downstream consequences, and the calibrated recommendation. Most decisions end here.

**Step 2 — Gate check**
If the decision is irreversible, run `/gate` first. If the facts aren't solid enough to analyze, stop and gather them. Structured thinking on bad facts produces confident-sounding garbage.

**Step 3 — Anchor to base rates**
Run `/baserates`. Before the inside-view analysis, ask what usually happens to decisions like yours. The Professor knew the statistics on heist success rates. You should know yours.

**Step 4 — Stress test**
Pick 1–2 frameworks based on the risk type:
- Risk of failure? → `/premortem`
- External adversary? → `/redteam` or `/wargame`
- Unknown unknowns? → `/blindspot`
- Competing options? → `/scenarios` or `/quantify`

**Step 5 — Land the call**
Every analysis ends with a recommendation: what to do, the confidence level (Verified / Reasoned / Assumed / Unknown), and what new information would change the answer.

---

## Worked Example: Product Launch Decision

This example is designed to show exactly what Decision Frameworks adds that Mastermind alone can't catch.

**Scenario:** *"We've built an AI tutoring app. We have 200 beta users, good retention, and $50K in savings. Investor wants us to raise a $500K seed round and scale now. Should we?"*

---

### With Mastermind only

> **Reframe:** The question isn't whether to raise — it's whether you're raising at the right moment or too early. $500K at this stage buys you distribution speed, but if product-market fit isn't locked, you're scaling a leaky bucket.
>
> **Assumption I'd challenge:** "Good retention" is doing a lot of work in your framing. 200 beta users who were personally recruited behave very differently from 200 users who found you organically. Which is it?
>
> **What you haven't asked:** What does the investor get out of moving fast? If they're pushing urgency, that's a negotiating signal, not a market signal.
>
> **Recommendation:** Don't raise yet. Run 30 more days of organic acquisition. If retention holds without your personal involvement in onboarding, you have signal. If it drops, you just saved yourself from scaling a problem.

**This is a solid read. But it misses two things Mastermind can't fully surface without structured tools.**

---

### Adding Decision Frameworks — what they catch that Mastermind missed

**`/premortem` — What kills this if you raise and scale now?**

> Fast-forward 18 months. You raised $500K, hired 4 people, scaled to 5,000 users. The startup failed. What happened?
>
> Most likely cause: Retention that looked like 70% at 200 users turned out to be 40% at scale — because your beta users were enthusiasts, not representative of the market. You burned through $380K trying to fix acquisition before realizing the product didn't work for mainstream students.
>
> Second cause: The investor's urgency was a signal that a competitor is coming. You raised, rushed the product, shipped bugs, and the competitor launched a cleaner product 4 months later.
>
> **Prevention:** Gate the raise on 30-day organic retention data from cold users, not recruited beta users. Don't sign until you have it.

**`/redteam` — How does a capable competitor break this?**

> If I were a well-funded competitor watching you raise $500K, here's my move: I wait until you've committed to a specific tutoring niche (based on your public hiring and marketing), then I enter that niche with 3x your budget and an established user base from an adjacent product. Your $500K disappears defending territory you just signaled.
>
> **Counter:** Before raising, don't signal your niche publicly. Raise on traction metrics, not on the specific subject area you're targeting.

**`/baserates` — What usually happens to EdTech startups that raise at 200 beta users?**

> Of EdTech startups that raised seed rounds pre-product-market-fit (defined as <1,000 organic users with >60% 30-day retention), roughly 65–70% pivoted or shut down within 24 months of the raise. The ones that succeeded had a distribution moat — a school district contract, a viral loop, or a celebrity endorsement — that made paid acquisition less critical. (Reasoned — based on EdTech failure analysis patterns; verify against current CB Insights data for your specific niche.)

---

### The Combined Final Call

**Mastermind alone** gave you: don't raise yet, validate organic retention first. Good advice.

**Mastermind + Decision Frameworks** gives you:
- **Specific failure mode** (beta user retention ≠ market retention) with a concrete prevention gate
- **Competitive threat** you hadn't modeled, and a counter-move to protect against it
- **Base rate** showing that most startups in this position that raise early fail — anchoring your optimism in what actually happens

**Final call:** Delay the raise by 45 days. Acquire 50 users with zero personal outreach (ads or organic only). If 30-day retention stays above 60% in that cohort, raise. If it drops below 50%, fix the product before taking the money.

*This is not a decision you could have landed confidently with Mastermind alone. The premortem found the specific failure mode. The red team surfaced a competitive threat. The base rates corrected for optimism bias. That's what the full stack is for.*

---

## Installing Both Skills

**Option A — Claude Cowork (recommended)**
1. Install `mastermind.skill` from this repo (Settings → Capabilities → Skills → Install from file)
2. Install the Decision Frameworks skill from the [decision-frameworks skill](https://github.com/Sroyal7) repo
3. Both are active immediately. Use `/mastermind` first, escalate with `/` commands when needed.

**Option B — Manual**
Copy `SKILL.md` from each repo into your Claude Cowork skills directory.

---

## The Underlying Principle

Mastermind is fast, pattern-based, and calibrated to the problem weight. Decision Frameworks are slow, structured, and exhaustive. The error most people make is using slow tools for fast problems and fast tools for slow problems.

The Professor was fast when speed mattered and methodical when failure was not an option. Match the tool to the stakes.

**Most decisions need Mastermind. A few need the full stack. The protocol tells you which.**
