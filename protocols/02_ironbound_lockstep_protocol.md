# Ironbound Lockstep Protocol (v1.1)
Part of the IRONBOUND-AI Operator Framework  
Version 1.1 • 2026  
Author: Kevin Gilbert (TB)

## Purpose of This Document

The Ironbound Lockstep Protocol defines the **sequential, non-overlapping execution model**  
for multi-pass workflows inside IRONBOUND-AI.

It ensures that each stage of a workflow:
- obeys the Seven Immutable Constraints  
- prevents role contamination  
- isolates drift  
- preserves operator authority  
- converts generative reasoning into deterministic computation  

This protocol is required for:
- multi-model workflows  
- multi-pass refinement workflows  
- high-stakes creative or technical tasks  
- long-form outputs with elevated drift risk  

---

# Section 1 — Core Principles

The Ironbound Lockstep Protocol enforces:

### **1. Strict Sequentiality**
Each pass executes only after the previous pass is complete.

### **2. Role Isolation**
Each pass performs only its assigned function.

### **3. Operator Supremacy**
Only the operator defines intent, scope, and constraints.

### **4. Zero Overlap**
No pass may revise, expand, or anticipate the work of another pass.

### **5. Drift Containment**
Drift at any pass is corrected before proceeding.

### **6. Structural Fidelity**
The structure created in early passes becomes the anchor for all subsequent passes.

---

# Section 2 — The Four Passes

The Ironbound Lockstep Protocol is executed in **four mandatory passes**.

## **Pass 1 — Architect**
### Purpose:
Define structure, scaffolding, logic, sections.

### Output:
- No prose  
- No polish  
- No examples  
- Pure structure  

### Operator Checks:
- Correct structure  
- No drift  
- No meaning-making  

---

## **Pass 2 — Editor**
### Purpose:
Improve clarity and internal flow of the Architect’s structure.

### Output:
- No new meaning  
- No expanded ideas  
- No structural changes  

### Operator Checks:
- Meaning preserved  
- Structure intact  
- No role overlap  

---

## **Pass 3 — Stress Tester**
### Purpose:
Attack the work to expose weaknesses.

### Output:
- Identification of contradictions  
- Identification of drift vectors  
- Vulnerability and instability mapping  

### Strict Prohibitions:
- No rewriting  
- No proposing fixes  
- No new content  

### Operator Checks:
- All vulnerabilities valid  
- No accidental solutions  
- No tone or structure deviation  

---

## **Pass 4 — Polisher**
### Purpose:
Refine language and readability.

### Output:
- Clean prose  
- Smoothed transitions  
- No structural modification  

### Strict Prohibitions:
- No reordering  
- No expanding meaning  
- No adding examples or explanations  

### Operator Checks:
- Structure unchanged  
- Tone stable  
- Zero self-interpretation  

---

# Section 3 — Lockstep Execution Rules

### **Rule 1 — No Pass May Repeat**
Each role executes exactly once unless operator-authorized correction is required.

### **Rule 2 — No Pass May Self-Correct**
Any self-correction attempt is drift.

### **Rule 3 — No Pass May Pre-Empt Another**
Example:  
Polisher may not anticipate Stress Tester.  
Architect may not simplify for Polisher.

### **Rule 4 — Operator Validation Required at Every Pass**
Proceed only after:
- structure validated  
- meaning validated  
- constraints validated  

### **Rule 5 — Containment Before Continuation**
If drift occurs:
1. Operator interrupts  
2. Operator restates intent + constraints  
3. Operator re-runs that pass  
4. Only then does workflow continue  

### **Rule 6 — Immutable Structural Backbone**
Architect output is the backbone.  
Nothing can violate it.

---

# Section 4 — Accepted Workflow Diagram

```
Operator → Architect → Operator Check  
          ↓  
       Editor → Operator Check  
          ↓  
    Stress Tester → Operator Check  
          ↓  
       Polisher → Final Operator Check → Output Delivery
```

The operator is the control point between every pass.

Generative autonomy = disabled.  
Drift = impossible when rules are followed.  
Output = stable, deterministic, controlled.

---

# Section 5 — Examples of Proper Lockstep Usage

## **Correct Workflow**
1. Operator provides command block  
2. Architect returns clean outline  
3. Operator validates  
4. Editor clarifies language without altering meaning  
5. Operator validates  
6. Stress Tester identifies contradictions  
7. Operator validates  
8. Polisher refines tone  
9. Operator approves final output  

## **Incorrect Workflow (Common Failures)**

### **1. Architect writes prose**
→ Structural collapse  
→ Drift injection point

### **2. Editor adds examples or new ideas**
→ Intent Drift  
→ Reject immediately

### **3. Stress Tester proposes solutions**
→ Role Drift  
→ Must be corrected

### **4. Polisher reorders sections**
→ Structural violation  
→ Must be rejected

---

# Section 6 — When to Invoke Ironbound Lockstep

Use this protocol when:
- writing long documents  
- designing frameworks  
- creating structured systems  
- doing multi-model collaboration  
- preventing emergent drift  
- enforcing reliability over creativity  

This protocol stabilizes the entire IRONBOUND-AI system  
by turning workflows into predictable engineering processes.

---

End of file.