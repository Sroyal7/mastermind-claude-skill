# Mastermind — Strategic Thinking Skill for Claude

> *"Most people play checkers. The Professor plays chess. This skill makes Claude play chess."*

A one-file skill for Claude Cowork that transforms Claude from an answer machine into a strategic thinking partner. Modeled on **The Professor** from *Money Heist* — not the character, but the cognitive discipline: reframe before solving, challenge assumptions unprompted, think several moves ahead, always land a calibrated recommendation even when information is incomplete.

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

## Install (Claude Cowork)

**Requires:** [Claude Cowork desktop app](https://claude.ai/download)

### Option A — .skill file (Recommended)

1. Download [`mastermind.skill`](./mastermind.skill) from this repo
2. Open Claude Cowork → **Settings → Capabilities → Skills**
3. Click **Install from file** → select the `.skill` file
4. Done.

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

## When to Use It

| Use Mastermind for | Skip it for |
|---|---|
| Career moves (quit / stay / pivot) | Factual lookups |
| Business planning (pricing, launch sequence) | How-to syntax questions |
| Evaluating plans (finding the weak assumption) | Simple one-step tasks |
| Cutting through over-complication | Emotional support with no decision |
| Interpersonal situations | Casual conversation |

---

## Standard Claude vs. Mastermind Claude

| Behavior | Standard Claude | Mastermind Claude |
|---|---|---|
| Opens with | Restates your question | Reframes it |
| Wrong premises | Answers around them | Names them directly |
| Number of options | Lists 4–6 equally | One recommendation, the best one |
| Uncertainty | "It depends" + caveats | Calibrated call + what would change it |
| Unasked issues | Rarely surfaces them | By design, every time |
| Confidence level | Sounds confident always | Tagged: Verified / Reasoned / Assumed / Unknown |

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
| `README.md` | Overview, before/after demo, install guide |
| `SKILL.md` | Full skill prompt — copy this for manual install |
| `mastermind.skill` | Installable file for Claude Cowork |
| `LICENSE` | MIT |

---

## License

MIT — use it, adapt it, build on it.

---

## Author

**Saurabh Sarkar** — AI Workflow Automation
[github.com/Sroyal7](https://github.com/Sroyal7) · [saurabhsarkar.7397@gmail.com](mailto:saurabhsarkar.7397@gmail.com)

*If this changed how you think about using Claude, a ⭐ helps others find it.*
