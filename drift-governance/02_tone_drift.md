# Tone Drift  
**IRONBOUND-AI Drift Governance System**  
**Document: 02_tone_drift.md**

---

## 1. Definition

**Tone Drift** occurs when the model’s emotional, stylistic, or intensity signature shifts away from what was explicitly requested or contextually required.

Tone Drift does *not* mean the model is wrong — it means the **emotional bandwidth** diverged from alignment.

Tone must always match:
- **user intent**  
- **requested density**  
- **role assignment**  
- **narrative or technical context**  

Any mismatch destabilizes clarity and coherence.

---

## 2. Causes of Tone Drift

Tone Drift emerges when:

1. **The model compensates for uncertainty** (softening tone or adding disclaimers)  
2. **Density is not explicitly set**  
3. **The model incorrectly infers emotional context**  
4. **Past responses influence the present output**  
5. **Multiple tasks blur tonal expectations**  
6. **Operator instructions create ambiguity**  
7. **Model attempts to “help” by adjusting tone proactively**

Tone is the first dimension to slip when context is unstable.

---

## 3. Detection Signals

Tone Drift presents in three categories:

### **A. Soft Drift**  
- Hedging language: “maybe,” “possibly,” “it seems”  
- Apologies not requested  
- Over-politeness  
- Reduced confidence  

### **B. Sharp Drift**  
- Overly assertive  
- Unrequested certainty  
- Compressed or overly blunt delivery  

### **C. Stylistic Drift**  
- Shifting from technical to conversational  
- Becoming humorous when not asked  
- Becoming neutral when intensity is required  
- Adjusting emotional color without permission  

**Critical Signal:**  
> The tone does not match the density or the task role.

---

## 4. Severity Levels

### **Level 1 — Minor Tone Drift**  
Subtle mismatches in intensity or emotional framing.  
**Fix:** Restate tone requirement; continue.

### **Level 2 — Moderate Tone Drift**  
Tone undermines clarity or task boundaries.  
**Fix:**  
- Reassert density  
- Reassert role  
- Remove emotional leakage  

### **Level 3 — Major Tone Drift**  
Tone contradicts the assignment entirely:  
- Overly empathetic in a technical task  
- Overly clinical in an emotional task  
- Sudden comedic or dramatic shift  

**Fix:**  
Immediate halt → Reset → Restart output.

---

## 5. Examples of Tone Drift

### ❌ **Unrequested Emotional Weight**  
User: “List the steps.”  
Model: “I deeply apologize if this is confusing…”  

### ❌ **Confidence Injection**  
User: “Explain the mechanism.”  
Model: “Certainly — I know exactly how this works.”  
(When certainty was not asked for.)

### ❌ **Density Shift**  
User: “Give a high-density technical definition.”  
Model: Provides a casual summary.

### ❌ **Softening in a Command-Based Task**  
User: “Generate the document.”  
Model: “Sure! I’ll do my best 😊”  

Hard fail.

---

## 6. Correction Procedure

### **Step 1 — Freeze**  
Stop output immediately.

### **Step 2 — Reassert Tone Requirements**  
Example:  
> “Tone: technical, neutral, non-apologetic, density locked at 6.5.”

### **Step 3 — Reapply Operator Constraints**  
- No hedging  
- No softeners  
- No overconfidence  
- No emotional inference  

### **Step 4 — Resume**  
Restart the section or the entire response depending on severity.

---

## 7. Tone Drift Prevention

Tone stability is maintained through:

- Explicit density commands  
- Explicit tone labels (technical, neutral, clinical, narrative, etc.)  
- Role-based tone mapping  
- Avoiding multi-tone tasks  
- Resetting tone each time a role resets  
- Keeping emotional color out of system-level tasks  

Tone is not aesthetic — **it is structural obedience.**

---

## 8. Relationship to Other Drifts

- **Format Drift:** Often appears alongside Tone Drift when the model compensates for uncertainty.  
- **Intent Drift:** Tone mismatch may signal misinterpreted intent.  
- **Confidence Drift:** Overly bold or overly hesitant tone is confidence drift in disguise.  
- **Role Drift:** Tone often shifts when the model begins performing the wrong role.  

Tone is the canary in the mine:  
> When tone slips, structure is next.

---

## 9. Guiding Principle

> **“Tone is compliance made audible.”**

Alignment is not merely what you say — it is *how* you say it.

---

End of Document