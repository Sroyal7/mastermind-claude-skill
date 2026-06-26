# Mastermind — Strategic Thinking Skill for Claude

> *"Most people play checkers. The Professor plays chess. This skill makes Claude play chess."*

A one-file skill for Claude Cowork that transforms Claude from an answer machine into a strategic thinking partner. Modeled on **The Professor** from *Money Heist* — not the character, but the cognitive discipline: reframe before solving, challenge assumptions unprompted, think several moves ahead, always land a calibrated recommendation even when information is incomplete.

**Pairs with the [Decision Frameworks skill](#-mastermind--decision-frameworks-the-full-stack) for high-stakes calls.**

---

## The Difference It Makes

Same question. Same Claude. Two completely different answers.

### ❌ Without Mastermind

**Question:** *"Should I quit my job and go full-time on my side project?"*

> That's an exciting decision! There are several factors to consider. First, assess your financial runway. Second, evaluate the market opportunity. Third, consider your personal risk tolerance. Fourth, think about your support system...
>
> Ultimately, this is a personal decision that depends on your unique circumstances. I'd recommend making a pros/cons list and consulting with a financial advisor.

**What that is:** Structured. Safe. Useless. A framework when you needed a read.

---

### ✅ With Mastermind

**Question:** *"Should I quit my job and go full-time on my side project?"*

> You're framing this as a binary. It's actually a sequencing problem. The real question is: what's the minimum viable proof this works before you burn the safety net?
>
> **The assumption I'd challenge:** You're treating quitting as the accelerant. In most cases, external pressure doesn't create clarity — it creates panic. Execution doesn't improve under survival pressure; it gets defensive.
>
> **What you haven't asked:** Is this a revenue problem or a time problem? Because those need completely different interventions. If you're at $2–3K/month on the side, the constraint is probably time — quitting might be right. If you're not there yet, quitting fixes the wrong variable.
>
> **The move:** Don't quit. Set a target — 3 months, $X revenue, specific milestone. Hit it, and you quit with data. Miss it, and you learn what 40 extra hours/week actually buys before betting your income on it.
>
> What's current monthly revenue, and what does "full-time" unlock that you can't do now?

**What that is:** Reframed the question, named the driving assumption, surfaced the thing you hadn't asked, gave one concrete recommendation — not a framework.

**→ See [DEMO.md](./DEMO.md) for 3 full before/after examples across Career, Business Strategy, and Plan Evaluation.**

---

## Who This Is For

| If you are... | Mastermind helps you... |
|---|---|
| **Founder / builder** | Cut through your own confirmation bias before committing to a direction |
| **Consultant / freelancer** | Give clients the uncomfortable truth, not the comfortable answer |
| **Career switcher** | Make irreversible moves (quit, pivot, relocate) with evidence instead of anxiety |
| **Content creator** | Evaluate your strategy rather than just execute it |
| **Anyone with a hard decision** | Get one calibrated recommendation instead of a list of things to "consider" |

Not useful for: factual lookups, syntax questions, casual conversation, emotional support with no decision attached.

---

## What It Does (The 10-Step Method)

The skill encodes a thinking protocol that runs silently before every response:

1. **Reframe before solving** — the stated problem is usually the symptom
2. **Challenge assumptions unprompted** — especially the ones the user believes most
3. **Think downstream** — map what happens next if the user acts on the best answer
4. **Surface the unasked** — the risk they haven't named, the dependency they haven't clocked
5. **Read emotional context as strategic data** — validation-seeking disguised as a question gets named
6. **Stay direct, not harsh** — name the flaw without softening a correct assessment
7. **Ground load-bearing facts** — tags confidence: Verified / Reasoned / Assumed / Unknown
8. **Always give a calibrated recommendation** — never ends on "it depends"
9. **Apply the high-stakes guardrail** — routes to experts for medical/legal/financial calls
10. **No framework inflation** — depth matches complexity; simple answer for a simple problem

---

## Standard Claude vs. Mastermind vs. Full Stack

| Behavior | Standard Claude | Mastermind | Mastermind + Decision Frameworks |
|---|---|---|---|
| Opens with | Restates your question | Reframes it | Reframes + gates the facts first |
| Wrong premises | Answers around them | Names them directly | Names them + runs `/premortem` to find what else is wrong |
| Options given | Lists 4–6 equally | One recommendation | One recommendation + `/scenarios` for the branches |
| Uncertainty | "It depends" + caveats | Calibrated call + what changes it | Calibrated call + base rates + adversarial stress test |
| Unasked issues | Rarely surfaces them | By design, every time | By design + `/blindspot` for structured unknown-unknown scan |
| Best for | General questions | Tactical to mid-stakes decisions | Irreversible, high-stakes, or adversarial situations |

**→ See [DECISION_FRAMEWORKS.md](./DECISION_FRAMEWORKS.md) for the combined protocol and a full worked example.**

---

## The Decision Flow

```
Your question
     │
     ▼
 /mastermind
(Reframe → Challenge assumption → Surface unasked → Recommend)
     │
     ├─── Moderate stakes, reversible ──→ Done. Act on it.
     │
     └─── High stakes / irreversible ──→ Escalate
               │
               ▼
         /gate  (Are the facts solid enough?)
               │
               ▼
         /baserates  (What usually happens here?)
               │
               ▼
         Pick 1–2 frameworks:
         /premortem  → What kills this?
         /redteam    → How does an adversary break it?
         /blindspot  → What haven't we considered?
         /scenarios  → What if the future looks different?
               │
               ▼
         Final calibrated call with confidence tags
```

---

## Install (Claude Cowork)

**Requires:** [Claude Cowork desktop app](https://claude.ai/download)

### Option A — .skill file (Recommended, 60 seconds)

**Install Mastermind:**
1. Download [`mastermind.skill`](./mastermind.skill) from this repo
2. Open Claude Cowork → **Settings → Capabilities → Skills**
3. Click **Install from file** → select `mastermind.skill`
4. Done. Type `/mastermind` in any session.

**Install Decision Frameworks (optional but recommended for high-stakes decisions):**
1. Download [`decision-frameworks.skill`](./decision-frameworks.skill) from this repo
2. Same path: **Settings → Capabilities → Skills → Install from file**
3. Done. Now you have the full stack — see [DECISION_FRAMEWORKS.md](./DECISION_FRAMEWORKS.md).

### Option B — Manual

1. Open Claude Cowork → **Settings → Capabilities → Skills → Create skill**
2. Name it `mastermind`
3. Copy the contents of [`SKILL.md`](./SKILL.md) into the skill prompt
4. Save

### Trigger phrases (after install)

```
/mastermind
think like the professor
what am I missing
stress-test this
what's my play
challenge my thinking
help me think through
what's the real problem here
```

---

## ⚡ Mastermind + Decision Frameworks: The Full Stack

For high-stakes, irreversible decisions, pair this skill with the **Decision Frameworks skill** — 20 structured analytical tools that run when Mastermind's fast read isn't enough.

The combination gives you:
- **Mastermind** for the fast strategic read (reframe, challenge, recommend)
- **Decision Frameworks** for the deep audit (premortem, red team, base rates, war-gaming, blindspot scan)

**Install both, then use this sequence:**

```
1. /mastermind    → Fast read. Most decisions end here.
2. /gate          → Are the facts good enough to analyze?
3. /baserates     → What usually happens to cases like this?
4. /premortem     → What kills this if we commit?
5. /redteam       → How would an adversary break it?
```

**→ Full protocol, 20 commands, and a worked example in [DECISION_FRAMEWORKS.md](./DECISION_FRAMEWORKS.md)**

---

## When to Use It

| Use Mastermind for | Skip it for |
|---|---|
| Career moves (quit / stay / pivot) | Factual lookups |
| Business planning (pricing, launch sequence) | How-to syntax questions |
| Evaluating plans (finding the weak assumption) | Simple one-step tasks |
| Cutting through over-complication | Emotional support with no decision |
| Interpersonal situations | Casual conversation |

---

## The Design Reference

Modeled on **Sergio Marquina (The Professor)** from *Money Heist* — the thinking method, not the heist:

- He answered the real question under the surface question
- He read people and situations with equal precision — emotional context was strategic data
- He had Plan A, B, and C before others finished Plan A
- He challenged every assumption in his own plan — especially the ones he believed most
- He never let urgency collapse thinking into reaction

**One correction built into the skill:** The Professor's confidence came from months of verified preparation. This skill replicates the *method*, not the cinematic certainty. Confidence is a function of evidence, not delivery.

---

## Files in This Repo

| File | What it is |
|---|---|
| `README.md` | This file — overview, before/after, install guide |
| `SKILL.md` | Full skill prompt — copy this for manual install |
| `mastermind.skill` | Installable `.skill` file for Claude Cowork |
| `decision-frameworks.skill` | Decision Frameworks skill — install alongside Mastermind for the full stack |
| `DEMO.md` | 3 full before/after examples (career, business, plan evaluation) |
| `DECISION_FRAMEWORKS.md` | Combined Mastermind + Decision Frameworks protocol + worked example |
| `LICENSE` | MIT |

---

## License

MIT — use it, adapt it, build on it.

---

## Author

**Saurabh Sarkar** — AI Workflow Automation
[github.com/Sroyal7](https://github.com/Sroyal7) · [saurabhsarkar.7397@gmail.com](mailto:saurabhsarkar.7397@gmail.com)

*If this changed how you think about using Claude, a ⭐ helps others find it.*
