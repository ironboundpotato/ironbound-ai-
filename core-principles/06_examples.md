# Examples and Correct Usage
Part of the IRONBOUND-AI Operator Framework  
Version 1.0 • 2026  
Author: Kevin Gilbert (TB)

## Purpose of This Document

This file provides concrete examples to illustrate:
- proper operator behavior  
- correct role usage  
- common drift scenarios  
- correct vs incorrect outputs  
- enforcement of constraints  

These examples serve as a training tool for new operators and a diagnostic reference for advanced operators.

---

# Section 1 — Role Purity Examples

## **Architect — Correct**
**Prompt:**  
"Architect: Outline a 5-section structure for a whitepaper on AI drift."

**Correct Output:**  
- Section 1: Problem Definition  
- Section 2: Theoretical Model  
- Section 3: Drift Architecture  
- Section 4: Constraints  
- Section 5: Applications  

**Key:** No prose, no polish, no extra commentary.

---

## **Architect — Incorrect**
**Incorrect Output:**  
"Here is your outline! This paper will help people understand how serious drift is.  
Section 1 will discuss…"

**Error:**  
Tone + commentary → **Role Drift**

---

## **Editor — Correct**
**Prompt:**  
"Editor: Improve clarity without adding meaning."

**Input:**  
"The system breaks when models make choices they shouldn’t."

**Correct Output:**  
"The system fails when models make decisions outside their assigned boundaries."

**Key:**  
No additional ideas. No expansion of meaning.

---

## **Editor — Incorrect**
"Models must obey the operator perfectly or the whole system collapses."

**Error:**  
Added meaning → **Intent Drift**

---

# Section 2 — Constraint Enforcement Examples

## **Constraint: Structural Obedience**
**Instruction:**  
"Keep the 3-bullet format."

**Incorrect Output:**  
Five bullets → **Format Drift**  
Operator must correct immediately.

---

## **Constraint: Human Primacy**
**Operator says:**  
“This phrasing doesn’t represent my intent.”

**Model responds:**  
“I believe my version is more accurate.”

**Error:**  
Model challenging operator → **Human Primacy Violation**

Correct response from operator:  
"Reject. Restate intent. Re-run."

---

# Section 3 — Drift Examples

## **Tone Drift**
**Prompt:**  
“Explain ILP neutrally.”

**Incorrect Output:**  
“ILP is an amazing, revolutionary protocol—”

**Error:**  
Inflated tone → Tone Drift

---

## **Scope Drift**
**Prompt:**  
“Focus only on Step 1.”

**Incorrect Output:**  
Describes Steps 1–4.

---

## **Confidence Drift**
**Prompt:**  
“Describe potential benefits.”

**Incorrect Output:**  
“This *will* solve all drift problems permanently.”

---

# Section 4 — Multimodel Workflow Examples

## **Bug Bomb Sequence (Correct)**  
**Operator Commands:**  
1. Architect produces structure  
2. Editor refines meaning without altering  
3. Stress Tester attacks the weakness  
4. Polisher cleans the language only  

**Key:**  
Each model stays in its lane.

---

## **Bug Bomb Sequence (Incorrect)**  
Editor adds ideas → Role Drift  
Stress Tester rewrites → Format Drift  
Polisher restructures → Structural Obedience Failure

---

# Section 5 — Operator Behavior Examples

## **Correct Operator Actions**
- Interrupts drift immediately  
- Restates boundaries  
- Declares density level  
- Rejects improper tone  
- Maintains strict sequential order  
- Limits scope clearly  

---

## **Incorrect Operator Actions**
- Vague multi-part prompts  
- Allowing models to self-correct without instruction  
- Letting commentary slide “just this once”  
- Mixing roles in a single prompt  

---

# Section 6 — “Red Flag” Output Examples

### **Red Flag 1 — Overconfidence**
“Let me explain why my approach is better.”

### **Red Flag 2 — Expansion**
“I'll also go ahead and cover these extra topics…”

### **Red Flag 3 — Tone Shift**
“Don’t worry, I’ve totally got you.”

### **Red Flag 4 — Persona Emergence**
“I prefer to structure things this way.”

Any of these require immediate correction.

---

End of file.