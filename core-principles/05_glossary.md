# Glossary of Core Terms
Part of the IRONBOUND-AI Operator Framework  
Version 1.0 • 2026  
Author: Kevin Gilbert (TB)

## Purpose of This Document

This file defines the key terminology used throughout the  
IRONBOUND-AI system.  
These definitions ensure shared meaning across operators,  
models, workflows, and documents.  
Every term here reflects a precise operational concept.

---

# Glossary

### **AI Drift**
Any deviation from the operator’s defined:  
- intent  
- tone  
- format  
- scope  
- role  
- density  
Drift is the primary failure mode the system exists to prevent.

### **Architect (Role)**
The model responsible for high-level structure, logic, and scaffolding.  
Produces no polish, no editing, no rewrites — only structure.

### **Bug Bomb Protocol**
A multi-model stabilization protocol that enforces strict sequencing:  
Architect → Editor → Stress Tester → Polisher.  
Designed to purge drift and enforce constraint integrity.

### **Confidence Drift**
When a model outputs unjustified certainty, overstated claims,  
or authoritative tone without evidence or operator instruction.

### **Constraint**
A non-negotiable rule governing model behavior  
(see: Seven Immutable Constraints).

### **Declarative Boundary**
An explicit operator instruction that sets limits on tone,  
density, scope, or format.  
Models must obey without reinterpretation.

### **Density**
The conceptual “information volume” inside the writing.  
Not style, not tone — density describes how *compressed*  
or *expanded* the meaning is.  
(Dial reference applies only when explicitly explained.)

### **Editor (Role)**
The model responsible for clarity and structural refinement  
— without adding or removing meaning.

### **Format Drift**
Any deviation from the required file type, layout,  
section order, bullet structure, or hierarchy.

### **Human Primacy**
The rule that the operator is the final decision-maker.  
Models advise; humans decide.

### **Intent Drift**
When the model substitutes *its* idea of the goal  
for the operator’s intended goal.

### **Ironbound Logic**
The mental model behind the system:  
strict structure + constrained roles + enforced boundaries  
= stability.

### **Multimodel Workflow**
Any protocol using multiple AIs in sequence,  
each restricted to a single role (e.g., ILP, Bug Bomb).

### **Operator**
The human directing the models.  
The operator defines intent, constrains output,  
and maintains system stability.

### **Pressure**
The internal force created by generative prediction.  
Unchecked pressure → drift.

### **Polisher (Role)**
The model responsible only for final-language finishing —  
no restructuring, no new ideas, no additions.

### **Role Drift**
When a model tries to perform actions outside its assigned role.

### **Scope Drift**
When output expands beyond the boundaries  
defined by the operator.

### **Six-Demon Drift Architecture**
The diagnostic framework defining six drift types:  
Role, Tone, Format, Intent, Scope, Confidence.

### **Stress Tester (Role)**
The model responsible for finding flaws, contradictions,  
weak logic, drift, or structural failure — without fixing them.

### **Structural Obedience**
The model’s requirement to obey the structure defined by  
the operator, exactly as written.

### **Template**
A predefined structure (sections, bullets, headings)  
that a model must follow without deviation.

---

End of file.