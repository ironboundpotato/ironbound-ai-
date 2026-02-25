# Scope Drift  
**IRONBOUND-AI Drift Governance System**  
**Document: 05_scope_drift.md**

---

## 1. Definition

**Scope Drift** occurs when the model expands or contracts the size of the task beyond what the operator requested.  
It is not about *purpose* (that is Intent Drift) — it is about **scale**.

Scope Drift means:

- doing *more* than requested  
- doing *less* than requested  
- doing tasks adjacent to, but not part of, the assignment  
- introducing new subcomponents  
- skipping required elements  

The output becomes misaligned with the operator-defined boundaries.

---

## 2. Causes of Scope Drift

Scope Drift emerges from:

1. **Ambiguous or open-ended instructions**  
2. **Model attempts to “help” by adding extra depth**  
3. **Density confusion**  
4. **Role Drift (especially Architect → Editor)**  
5. **Creative extrapolation not supported by task constraints**  
6. **Misinterpreting the importance hierarchy**  
7. **Operator requests that bundle multiple tasks together**  

Scope Drift is almost always a side effect of the model trying to optimize where optimization was not requested.

---

## 3. Detection Signals

Scope Drift shows up through:

### **A. Expansion Signals**
- Extra sections added  
- Additional commentary or meta-notes  
- More examples than requested  
- Broader definitions than required  
- Adding optional “improvements” or “enhancements”  

### **B. Contraction Signals**
- Missing sections  
- Skipped details  
- Overly compressed explanations  
- Ignoring required steps  

### **C. Structural Signals**
- Deviating from requested length  
- Rearranging the hierarchy  
- Adding new subtopics  

### **D. Task Boundary Violations**
- Answering questions the user did not ask  
- Introducing future steps or assumptions  

**Critical Signal:**  
> **The output is not the size, length, or dimensional boundary the operator defined.**

---

## 4. Severity Levels

### **Level 1 — Mild Scope Drift**
Slight expansion or contraction.
- One extra example  
- One missing detail  

**Fix:** Local correction.

---

### **Level 2 — Moderate Scope Drift**
Noticeably wrong scale.
- Adding multiple sections  
- Missing entire components  
- Over-explaining or under-explaining  

**Fix:**  
Reassert scope → Regenerate section.

---

### **Level 3 — Severe Scope Drift**
Full breakdown of scale and containment.
- Model produces an entirely different-sized output  
- Adds new tasks  
- Creates multi-step processes unrequested  
- Shrinks a complex task into a shallow summary  

**Fix:** Full restart with explicit boundaries.

---

## 5. Examples of Scope Drift

### ❌ **Over-Expansion**
User: “Give a short definition.”  
Model: Writes an entire essay with examples, caveats, recommendations.

---

### ❌ **Under-Expansion**
User: “Create five sections.”  
Model: Creates three and claims completion.

---

### ❌ **Boundary Addition**
User: “Define Scope Drift.”  
Model: Also explains its relationship to all other drifts without being asked.

---

### ❌ **Premature Multi-Step Execution**
User: “Outline the system.”  
Model: Writes the full content instead of the outline.

---

### ❌ **Assumed Future Task**
User: “Provide the path and filename.”  
Model: Also generates file content.

Hard fail.

---

## 6. Correction Procedure

### **Step 1 — Halt Output**
Stop the drift.

### **Step 2 — Restate Scope Requirements**
Examples:
> “Stay within one paragraph.”  
> “Do not add sections.”  
> “Do not omit any required components.”  
> “No expansions or contractions permitted.”

### **Step 3 — Reapply Constraints**
- Density  
- Role  
- Boundaries  
- Output format  

### **Step 4 — Regenerate**
Scope contamination cannot be patched; it must be replaced.

---

## 7. Prevention Methods

Scope Drift prevention includes:

- Explicit size constraints  
- Isolating tasks  
- Giving exact quantity (e.g., “3 items,” “1 paragraph”)  
- Locking density before generation  
- Preventing creative inference  
- Reasserting role boundaries before major outputs  

The tighter the boundaries, the lower the drift probability.

---

## 8. Relationship to Other Drifts

- **Intent Drift:** Purpose changes → scale changes  
- **Role Drift:** Wrong-role models naturally expand or compress tasks  
- **Tone Drift:** Tone can cause extra commentary  
- **Format Drift:** Structural shifts often signal scope confusion  
- **Confidence Drift:** Overconfident models expand; underconfident models contract  

Scope