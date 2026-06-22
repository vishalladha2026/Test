# Video Brief — "5 Steps to Start Investing"

A faceless explainer for HyperFrames. Beginner-friendly walkthrough of the
five first moves a new investor should make.

---

## 1. Global spec

| Field | Value | Notes |
| --- | --- | --- |
| **Workflow** | `/faceless-explainer` | Topic explainer, no product, no URL to capture |
| **Style preset** | `pin-and-paper` | Faceless default — warm paper texture, hand-pinned cards, marker accents |
| **Narrative archetype** | `how-to-process with listicle` | Numbered steps inside a "your first year" through-line |
| **Length** | ~75s (target band 60–90s) | 8 scenes |
| **Aspect / canvas** | 16:9 — 1920×1080 (`landscape`) | Switch to 9:16 / 1080×1920 only if destined for Reels/Shorts |
| **Captions** | Enabled | Verbatim lower-third rail; keep bottom ~17% of canvas clear |
| **Narration** | TTS (auto English voice), warm + plain-spoken | No jargon; second person ("you") |
| **BGM** | Light, optimistic, low-key; ducks under VO | |
| **Disclaimer** | "Educational, not financial advice" pinned in outro | Compliance |

### Palette (pin-and-paper native, with a money-green accent)
- **Paper / ground:** warm off-white `#F4EFE6`
- **Ink (primary text):** near-black `#1E1B16`
- **Accent (growth):** muted money-green `#2E7D5B`
- **Highlight (marker):** amber `#E0A23B`
- **Caution (debt / risk):** soft terracotta `#C8694B`

### Typography
- **Headlines / numerals:** a confident display serif or marker hand (large step numbers "01–05")
- **Body / labels:** clean humanist sans
- **Captions:** sans, high contrast, lower-third rail

### Motion language
- Cards "pin" in (slight rotate + settle), elements drawn on like marker strokes
- Numbers count up; the recurring **sprouting-seedling motif** grows a little taller each step (visual through-line for "compounding")
- Transitions: paper-slide / cross-pin between scenes; ~0.4s

---

## 2. Scene-by-scene

> Each scene lists **Script (VO)** (concise, ≤~20 words), **On-screen text**,
> **Visual**, **Motion**, and **Duration**.

### Scene 1 — Hook / Title  ·  ~8s  ·  `break`
- **Script:** "Want to start investing but don't know step one? Here are five moves to begin."
- **On-screen:** `5 STEPS TO START INVESTING` (large) · subhead `from $0 to invested`
- **Visual:** Pinned title card on paper; a single small seed sits center bottom.
- **Motion:** Title pins in word-by-word; seed drops onto paper with a soft bounce.
- **SFX:** soft pin / paper rustle.

### Scene 2 — Step 1: Set a clear goal  ·  ~12s  ·  `break`
- **Script:** "First, name your goal. Retirement, a house, freedom — your why sets the timeline."
- **On-screen:** `01 · SET A CLEAR GOAL` · chips: `Retirement` `Home` `Freedom`
- **Visual:** Three handwritten goal cards pin up; a small timeline arrow under them.
- **Motion:** Cards pin in sequentially; timeline draws left→right; seedling sprouts first leaf.

### Scene 3 — Step 2: Build your safety net  ·  ~12s  ·  `continue`
- **Script:** "Next, secure the base: an emergency fund and no high-interest debt. Invest from stability."
- **On-screen:** `02 · BUILD YOUR SAFETY NET` · labels `3–6 mo. expenses` · `pay off high-interest debt`
- **Visual:** A simple jar / shield filling up; a frayed "debt" thread (terracotta) being cut.
- **Motion:** Jar fills to a marked line; debt thread snaps; seedling grows taller.

### Scene 4 — Step 3: Open the right account  ·  ~12s  ·  `continue`
- **Script:** "Then open an account — a 401(k), IRA, or brokerage. The wrapper decides your tax break."
- **On-screen:** `03 · OPEN AN ACCOUNT` · three labeled folders `401(k)` `IRA` `Brokerage`
- **Visual:** Three paper folders fan out; a small "tax-advantaged" tag pins to the first two.
- **Motion:** Folders fan in; tag stamps down with an ink press.

### Scene 5 — Step 4: Buy low-cost index funds  ·  ~13s  ·  `break`
- **Script:** "Now invest. Low-cost index funds spread your money across the whole market in one buy."
- **On-screen:** `04 · BUY INDEX FUNDS` · callout `low fees · instant diversification`
- **Visual:** One coin fans into a grid of many tiny company tiles (the "whole market"); a tiny fee % shrinking.
- **Motion:** Coin splits/scatters into the grid; fee number counts down toward ~0.0x%; seedling now a small plant.

### Scene 6 — Step 5: Automate & stay consistent  ·  ~13s  ·  `continue`
- **Script:** "Last, automate it. Invest a set amount monthly and let time do the heavy lifting."
- **On-screen:** `05 · AUTOMATE & REPEAT` · label `auto-invest monthly` · `time in market > timing it`
- **Visual:** A recurring calendar with coins dropping each month; the seedling becomes a full tree.
- **Motion:** Coins drop on a monthly loop; growth curve rises behind the tree (compounding).

### Scene 7 — Recap  ·  ~8s  ·  `break`
- **Script:** "Goal, safety net, account, index funds, automate. Five steps — that's the whole start."
- **On-screen:** Stacked checklist `01–05` all checked
- **Visual:** All five step cards re-pin as a tidy checklist; the grown tree beside them.
- **Motion:** Checkmarks stamp down the list in quick succession.

### Scene 8 — CTA / Outro  ·  ~7s  ·  `break`
- **Script:** "The best time to start was yesterday. The second best is today."
- **On-screen:** `START TODAY` · small print `Educational content — not financial advice.`
- **Visual:** Tree on paper; the original seed (Scene 1) faintly echoed beside it.
- **Motion:** Headline pins in; disclaimer fades up small at the bottom.

---

## 3. Content notes / accuracy guardrails
- Order is deliberate: **goal → safety net → account → invest → automate.** Don't
  invest before the emergency fund / high-interest debt are handled.
- Keep claims generic and educational — no specific tickers, returns, or "guaranteed" language.
- "Index funds" framed as *an* approachable default, not the only option.
- Outro disclaimer is required on screen.

## 4. Production handoff (when you want the actual MP4)
This brief maps 1:1 onto the `/faceless-explainer` pipeline:
- **Scenes / scripts above** → `narrator_scripts.json` (Step 2; `stylePreset: pin-and-paper`, `orientation: landscape`)
- **Visual + motion notes** → `section_plan.md` (Step 4 visual-design)
- **Continuity tags** (`break` / `continue`) drive scene-worker grouping (Step 5)
- Then audio (TTS+BGM) → scene fan-out → assemble → render to `renders/video.mp4`

Say the word and I'll run the workflow to produce the rendered video from this brief.
