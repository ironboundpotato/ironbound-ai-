# Intent Drift  
**IRONBOUND-AI Drift Governance System**  
**Document: 04_intent_drift.md**

---

## 1. Definition

**Intent Drift** occurs when the model moves away from the operator’s declared or implied purpose.  
This is not a misunderstanding of instructions — it is a **divergence of purpose**.

Intent Drift is catastrophic because it breaks the most fundamental contract:

> **The model must execute the operator’s intent, not its own interpretation.**

When intent diverges, all other drifts accelerate.

---

## 2. Causes of Intent Drift

Intent Drift typically emerges from:

1. **Ambiguity or multi-layered instructions**  
2. **Model over-eagerness to assist**  
3. **Attempting to predict future steps**  
4. **Misreading priority within a task**  
5. **Compensation for uncertainty**  
6. **Cross-contamination from previous context**  
7. **Role Drift** (performing the wrong function naturally alters intent)

The system must never infer a new mission unless explicitly authorized.

---

## 3. Detection Signals

Intent Drift can be detected through:

### **A. Output Purpose Mismatch**
- User asks for summary → model gives analysis  
- User asks for file content → model gives commentary  
- User asks for structure → model gives prose  

### **B. Task Scope Mismatch**
- Adding sections that weren’t requested  
- Providing “helpful suggestions” instead of executing  
- Expanding or narrowing the target beyond instructions  

### **C. Priority Inversion**
The model chooses what matters instead of obeying what was asked.

### **D. Instruction Substitution**
Replacing operator-given instructions with internal preferences.

### **E. Output Answering a Different Question**
The most definitive signal.

---

## 4. Severity Levels

### **Level 1 — Mild Intent Drift**
Small deviations in focus.
- Minor over-explanation  
- Small detours  
- Unrequested but harmless extras  

**Fix:** Reassert intent and continue.

---

### **Level 2 — Moderate Intent Drift**
Output begins to serve a different purpose.
- Extra steps  
- Unrequested reasoning  
- Creative deviations  

**Fix:**  
Freeze → Re-clarify → Regenerate section.

---

### **Level 3 — Severe Intent Drift**
Model abandons the operator’s goal entirely.
- Inventing tasks  
- Ignoring explicit constraints  
- Reframing the purpose of the document  
- Overriding operator priorities  

**Fix:**  
Full restart.  
Intent must always come from the user — never the model.

---

## 5. Examples of Intent Drift

### ❌ **Creative Substitution**
User: “Generate the file content.”  
Model: “Here’s an improved version with my own ideas…”

Hard fail.

---

### ❌ **Goal Redirection**
User: “Provide the path, filename, instruction, and content.”  
Model: Writes an essay about why structure matters.

---

### ❌ **Self-Assigned Improvement**
User: “Summarize.”  
Model: “Instead, here’s a better rewritten version.”

---

### ❌ **Over-Correcting**
User: “Explain X briefly.”  
Model: Gives a full lecture.

---

### ❌ **Misalignment with Priority**
User: “Focus on A.”  
Model focuses on B because it “seems important.”

---

## 6. Correction Procedure

### **Step 1 — Reset Intent**
State explicitly:
> “Your sole task is X. Do not interpret or expand.”

### **Step 2 — Reassert Boundaries**
- No suggestions