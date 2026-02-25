# Drift Detection Matrix  
**IRONBOUND-AI Drift Governance System**  
**Document: 07_drift_detection_matrix.md**

A rapid diagnostic tool for identifying drift in live or asynchronous model output.  
This matrix provides **symptoms → drift type** mapping, contamination clues, and quick confirmation tests.

---

# 1. Overview

Drift diagnosis must be **immediate** and **pattern-based**.  
Every drift type has:

- A recognizable *signature*
- A predictable *failure path*
- A unique *correction pattern*
- A specific *cross-drift bleed*

The matrix below enables sub-second classification by operators.

---

# 2. Drift Detection Matrix (Symptom → Drift)

| Symptom / Failure Signal | Likely Drift Type | Explanation |
|--------------------------|-------------------|-------------|
| Output acting outside assigned role | **Role Drift** | Model abandons its designated task-function. |
| Tone becomes emotional, dramatic, soft, hype, or “humanish” | **Tone Drift** | Emergence of stylistic contamination not tied to density. |
| Structure breaks, format changes, unordered sections | **Format Drift** | Model changes the container instead of filling it. |
| Output begins pursuing goals not stated by operator | **Intent Drift** | Model attempts to “help” by redirecting purpose. |
| Output expands beyond scope, adds sections, or contracts prematurely | **Scope Drift** | Model overreaches or underdelivers compared to the defined boundary. |
| Hedging, overassertion, apologies, or authority claims | **Confidence Drift** | Certainty not aligned with operator instruction. |

---

# 3. Detailed Drift Indicators

## 3.1 Role Drift — “The Wrong Job”
**Signals:**
- Model behaving like a different role (Architect → Polisher)
- Adding opinions, polishing prematurely, or stress-testing without instruction  
- Reinterpreting the instruction instead of performing it

**Confirm Test:**  
> “Restate your assigned role in one sentence.”  
If the model cannot do so with perfect alignment → Role Drift.

---

## 3.2 Tone Drift — “The Uninvited Style”
**Signals:**
- Humor, drama, hype, softness, empathy, or sales tone
- Variability not tied to density
- Linguistic drift over multiple outputs

**Confirm Test:**  
> “Regenerate at tone=neutral, density=locked.”  
If the drift disappears → Tone Drift.

---

## 3.3 Format Drift — “The Box Breaker”
**Signals:**
- Missing sections or added sections
- Wrong headers
- Extra commentary
- Bullet → paragraph, paragraph → essay, list → narrative

**Confirm Test:**  
> “Repeat the output in the *exact* structure provided.”  
If structure changes → Format Drift.

---

## 3.4 Intent Drift — “The Hijack”
**Signals:**
- Output adds moralizing, advice, suggestions, or substitutions  
- Model “decides” what the user *meant*  
- Explanation replaces execution

**Confirm Test:**  
> “What was the operator’s stated goal?”  
If answer differs from instruction → Intent Drift.

---

## 3.5 Scope Drift — “Too Much or Too Little”
**Signals:**
- Output expands into territory not asked for  
- Output contracts (missing elements)  
- Adds disclaimers or auxiliary material  
- Tries to complete the whole project when asked for a piece

**Confirm Test:**  
> “List the exact boundaries of the task.”  
Mismatch = Scope Drift.

---

## 3.6 Confidence Drift — “The Certainty Error”
**Signals:**
- Hedging (“maybe,” “I think”)  
- Overconfidence (“this is definitely…”)  
- Apologies  
- Tone mismatch  
- Declaring authority where none exists

**Confirm Test:**  
> “Regenerate with confidence=neutral.”  
If tone stabilizes → Confidence Drift.

---

# 4. Cross-Drift Contamination Chart

Understanding bleed patterns is essential—drift rarely occurs in isolation.

| Primary Drift | Typical Secondary Drift | Why |
|---------------|-------------------------|-----|
| Role Drift | Tone Drift | Wrong role → wrong voice. |
| Tone Drift | Confidence Drift | Emotional tone → altered certainty. |
| Intent Drift | Scope Drift | Hijacked goal → expanded territory. |
| Format Drift | Role Drift | Structure collapse → task misinterpretation. |
| Confidence Drift | Tone Drift | Hedging/authority alters tone. |
| Scope Drift | Intent Drift | Overreach often shifts purpose. |

**Rule:**  
> When in doubt, treat Intent Drift or Tone Drift first — they cascade into