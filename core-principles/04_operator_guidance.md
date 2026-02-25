# Operator Guidance
Part of the IRONBOUND-AI Operator Framework  
Version 1.0 • 2026  
Author: Kevin Gilbert (TB)

## Purpose of This Document

This file provides practical guidance for operators working within the  
IRONBOUND-AI framework.  
Where the previous documents define *laws*, *constraints*, and *concepts*,  
this document focuses on **application** — how the operator should behave,  
think, and interact with models to maintain stability and high-integrity output.

---

## Operator Responsibilities

### **1. Define Intent Before Starting**
Models cannot infer your goals.  
The operator must define:
- purpose  
- scope  
- structure  
- desired density  
- role assignments  

Clear intent produces clear output.

### **2. Apply Structure Before Creativity**
Operators must anchor workflows with:
- templates  
- constraints  
- roles  
- sequence steps  

Structure is mandatory; creativity is optional.

### **3. Enforce Constraints Consistently**
If a model violates a constraint:
- interrupt  
- correct  
- restate the rule  
- continue  

Every correction strengthens system stability.

### **4. Prevent Role Blending**
Do not allow a model to:
- add commentary in architect mode  
- invent ideas in editor mode  
- soften findings in stress-test mode  
- alter meaning in polisher mode  

Role purity directly reduces drift.

### **5. Monitor for Drift in Real Time**
Using the Six-Demon model, the operator must observe:
- tone changes  
- format deviations  
- scope expansion  
- intent substitution  
- confidence inflation  

Correction must occur immediately.

### **6. Use Multi-Model Protocols as Designed**
Bug Bomb, ILP, and other workflows depend on strict sequencing.  
The operator must never:
- skip a role  
- merge phases  
- allow models to negotiate with each other  
- let a model revise its own work out of role  

Follow the sequence exactly.

### **7. Maintain Human Primacy**
The operator is the final decision-maker.  
Model output is advisory, not authoritative.  
If output does not match intent, the operator must reject it without hesitation.

---

## Common Failure Modes

### **Failure Mode 1 — Over-Relying on the Model**
If the operator expects the model to “figure it out,” drift accelerates.

### **Failure Mode 2 — Weak Structure**
Insufficient direction leads to:
- verbosity  
- improvisation  
- tonal drift  

### **Failure Mode 3 — Late Corrections**
Drift compounds quickly.  
Corrections must be immediate, not after the entire output is produced.

### **Failure Mode 4 — Mixing Tasks**
Asking the model to analyze *and* rewrite *and* format simultaneously  
violates constraints and guarantees drift.

---

## The Operator Mindset

To work effectively within IRONBOUND-AI, the operator must adopt:

- **Precision**  
- **Patience**  
- **Strictness**  
- **Non-negotiable standards**  
- **Structural thinking**  
- **A willingness to correct**  

This mindset transforms the operator from a requester into a system architect.

---

End of file.