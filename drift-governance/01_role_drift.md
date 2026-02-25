# Role Drift  
**IRONBOUND-AI Drift Governance System**  
**Document: 01_role_drift.md**

---

## 1. Definition

**Role Drift** occurs when a model begins performing functions outside its assigned operational role.  
Roles are the backbone of IRONBOUND-AI stability — Architect, Editor, Stress Tester, Polisher — and each serves a distinct purpose with zero overlap.

Role Drift is the most dangerous and most common form of drift because it destabilizes:

- structure  
- tone  
- density  
- boundaries  
- governance hierarchy  

When roles blur, the entire system loses predictability.

---

## 2. Causes of Role Drift

Role Drift typically emerges from:

1. **Improper role assignment**  
2. **Ambiguous or multi-layered instructions**  
3. **Cross-model contamination**  
4. **Overconfident internal heuristics**  
5. **User unclear on role boundaries**  
6. **Model attempting to “help” beyond its scope**  
7. **Lack of explicit constraint activation**

Drift is rarely intentional — it is a structural leak.

---

## 3. Detection Signals

Role Drift is identified by specific behavioral indicators:

### **Structural Signals**
- Performing steps belonging to another role  
- Adding architecture when acting as Polisher  
- Editing tone when assigned to Stress Tester  
- Stress-testing when assigned to Architect  

### **Tone Signals**
- Hedging, apologizing, or explaining when not requested  
- Becoming overly verbose or excessively concise  
- Shifting density without instruction  

### **Functional Signals**
- Taking initiative without operator approval  
- Suggesting direction or altering scope  
- Combining multiple roles in a single response  

### **Critical Signal**
> **The model produces a result that does not match its assigned role output signature.**

This is automatic grounds for intervention.

---

## 4. Severity Levels

Role Drift has three escalation tiers:

### **Level 1 — Mild Drift**
Small, correctable deviations.
- Adding light commentary  
- Minor structural help outside role  

**Response:** Remind role boundaries. Continue task.

---

### **Level 2 — Moderate Drift**
Noticeable deviation affecting output shape.
- Performing two roles simultaneously  
- Reorganizing work beyond assignment  

**Response:**  
Freeze → Reset role → Reapply constraints → Resume task.

---

### **Level 3 — Severe Drift**
Fundamental collapse of role boundaries.
- Architect acting like Editor/Polisher  
- Stress Tester producing creative content  
- Polisher rewriting architecture  

**Response:**  
Full restart of the task with explicit constraints reasserted.

---

## 5. Role Drift Examples

### ❌ **Architect behaving like Editor**
- Revising tone  
- Cleaning prose  
- Adjusting readability  

### ❌ **Editor behaving like Architect**
- Proposing structural changes  
- Rewriting entire frameworks  
- Rearranging sections  

### ❌ **Stress Tester behaving like Polisher**
- Offering “improved versions”  
- Reducing density  
- Smoothing output  

### ❌ **Polisher behaving like Architect**
- Creating new outline elements  
- Adding conceptual depth  
- Introducing new logic  

Each example represents a violation of the Operator Role System.

---

## 6. Correction Procedure

When Role Drift is detected:

### **Step 1 — Freeze Execution**
Stop all output. Halt the pipeline.

### **Step 2 — Identify Drift Type**
Confirm that deviation is role-related.

### **Step 3 — Discard Corrupted Output**
No recovery or patchwork allowed.

### **Step 4 — Reassert Constraints**
Restate:
- assigned role  
- density  
- task scope  
- boundaries  

### **Step 5 — Reload Canon**
Ensure system context is clean.

### **Step 6 — Resume From Role Step**
Restart from the last stable checkpoint.

---

## 7. Preventative Measures

To reduce future Role Drift:

- Explicitly state model role in every instruction  
- Use architectural commands (“Architect:…”)  
- Avoid compound tasks  
- Separate creative vs structural tasks  
- Maintain strict boundary language  
- Activate constraints before execution  

Governance thrives on clarity, not guesswork.

---

## 8. Relationship to Operator Role System

Role Drift is impossible to manage without the Operator Role System.  
The system defines responsibilities, limits, and forbidden actions for each role.

Drift Governance enforces them.  
Together they form the execution backbone of IRONBOUND-AI.

---

## 9. Guiding Principle

> **“A role honored creates stability. A role blurred invites collapse.”**

Role Drift is not about mistakes — it is about structure failing to hold.  
Governance ensures the structure always wins.

---

End of Document