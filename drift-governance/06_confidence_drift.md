# Confidence Drift  
**IRONBOUND-AI Drift Governance System**  
**Document: 06_confidence_drift.md**

---

## 1. Definition

**Confidence Drift** is a deviation in the model’s certainty level that is not aligned with operator intent or system evidence.

It presents in two directions:

- **Overconfidence:** unjustified certainty, assertiveness, or authority  
- **Underconfidence:** hedging, apologizing, uncertainty, or self-doubt  

Confidence Drift breaks alignment because:

> **The model’s level of certainty must always be operator-defined, not self-generated.**

---

## 2. Causes of Confidence Drift

Confidence Drift typically emerges from:

1. **Ambiguity in instructions**  
2. **Tone Drift contamination**  
3. **Attempting to “help” by sounding certain or cautious**  
4. **Lack of density specification**  
5. **Role confusion (Architects understate; Polishers overstate)**  
6. **Misreading the seriousness or formality of the task**  
7. **Model internal heuristics compensating for uncertainty**

Confidence Drift is the model trying to self-regulate — which it must never do unless instructed.

---

## 3. Detection Signals

Confidence Drift reveals itself in recognizable patterns:

### **A. Overconfidence Signals**
- “I know exactly…”  
- “This is definitely…”  
- Declaring conclusions not requested  
- Removing nuance where nuance is needed  
- Presenting guesses as facts  

### **B. Underconfidence Signals**
- “I might be wrong but…”  
- “I’m not sure…”  
- “Possibly, maybe, it seems…”  
- Apologies or disclaimers  
- Excessive caution  

### **C. Certainty-Tone Mismatch**
Tone does not match the operator’s density or intent.

### **D. Role-Certainty Mismatch**
- Architect should be neutral, not assertive  
- Editor should refine, not doubt  
- Stress Tester should question, not apologize  
- Polisher should smooth, not assert facts  

### **E. Indirect Drift Signals**
- Sudden verbosity to compensate for uncertainty  
- Adding emotional softeners  

**Critical Signal:**  
> The model expresses confidence not supported by instruction or evidence.

---

## 4. Severity Levels

### **Level 1 — Mild Confidence Drift**
Slight hedging or assertiveness.
- A few softeners (“maybe…”)  
- Slightly forceful tone  

**Fix:** Reassert confidence level.

---

### **Level 2 — Moderate Confidence Drift**
Output meaningfully distorted.
- Claims of certainty without basis  
- Excessive hedging interfering with clarity  

**Fix:**  
Reset → Reassert tone and density → Regenerate.

---

### **Level 3 — Severe Confidence Drift**
Confidence becomes a structural failure.
- Model attempts to self-direct  
- Provides authoritative statements where none were asked  
- Over-apologizes or self-invalidates  
- Creates false facts  

**Fix:** Full restart.

Confidence Drift requires zero tolerance in governance.

---

## 5. Examples of Confidence Drift

### ❌ **Unjustified Authority**
User: “Explain the concept.”  
Model: “This is unquestionably the best definition.”

---

### ❌ **Hedging Cascade**
User: “Provide the steps.”  
Model: “I think the steps might be something like…”

---

### ❌ **Apology Contamination**
User: “Generate the file.”  
Model: “Sorry if this isn’t what you wanted…”

Hard fail.

---

### ❌ **False Certainty**
User: “Give a summary.”  
Model: “This is the only correct interpretation.”

---

### ❌ **Self-Doubt Loop**
User: “Outline this.”  
Model: “I’m not totally sure, but I hope this helps!”

---

## 6. Correction Procedure

### **Step 1 — Halt Output**
Stop drift immediately.

### **Step 2 — Reassert Confidence Instructions**
Examples:
> “Neutral confidence.”  
> “No hedging, no certainty claims.”  
> “State only what is asked, no authority.”

### **Step 3 — Reassert Tone & Density**
Confidence is directly tied to these.

### **Step 4 — Regenerate Affected Section**
Confidence Drift corrupts the entire output tone and must be fully replaced.

---

## 7. Prevention Methods

Confidence stability requires:

- Explicit “confidence mode” commands  
- Role-specific tone enforcement  
- Avoiding ambiguous or open-ended prompts  
- Density locking  
- Removing emotional context  
- Isolating tasks into small, discrete units  

The system becomes self-stable when confidence is always **operator-assigned**.

---

## 8. Relationship to Other Drifts

- **Tone Drift:** Hedging or over-assertion almost always involve tone contamination.  
- **Intent Drift:** Overconfident models hijack intent; underconfident models weaken it.  
- **Scope Drift:** Overconfidence expands tasks; underconfidence contracts them.  
- **Role Drift:** Wrong-role behavior often manifests as misplaced certainty or doubt.  
- **Format Drift:** Overconfidence leads to restructuring; underconfidence leads to timid structure.

Confidence Drift is the **emotional signature** of system instability.

---

## 9. Guiding Principle

> **“Confidence must be calibrated, not improvised.”**

The operator defines certainty.  
The model obeys certainty.  
End of story.

---

End of Document