# Operator Command Templates (v1.1)
Part of the IRONBOUND-AI Operator Framework  
Version 1.1 • 2026  
Author: Kevin Gilbert (TB)

## Purpose of This Document

This file provides **ready-to-use operator command templates**  
for every stage of IRONBOUND-AI workflows.

These templates:
- enforce constraints  
- activate roles cleanly  
- prevent drift  
- simplify operator control  
- standardize multi-model workflows  

They represent the **canonical command vocabulary** of IRONBOUND-AI.

---

# Section 1 — Universal Command Block Template

This is the master template used before any workflow begins.

```
INTENT:
<Describe what you want the system to produce.>

ROLE:
<Architect | Editor | Stress Tester | Polisher>

CONSTRAINTS:
<List the rules the model must obey.>

DENSITY:
<Specify the required depth or complexity level.>

FORBIDDEN:
<List prohibited actions.>

OUTPUT FORMAT:
<Specify outline, bullet list, paragraphs, steps, etc.>
```

The operator fills each field with precision.  
The model must obey exactly.

---

# Section 2 — Architect Activation Templates

## **Template A — Create Structure**
```
ROLE: Architect.
INTENT: Build a multi-level structure for <X>.
CONSTRAINTS: Structure only. No prose. No commentary. No examples.
FORBIDDEN: Tone, style, explanation, polishing.
OUTPUT FORMAT: Outline with hierarchical sections.
```

## **Template B — System Architecture**
```
ROLE: Architect.
INTENT: Construct the full system architecture for <X>.
CONSTRAINTS: Pure structure. No descriptive expansion.
FORBIDDEN: Metaphors, prose, suggestions.
OUTPUT FORMAT: Component map with ordered layers.
```

---

# Section 3 — Editor Activation Templates

## **Template A — Clarify Structure**
```
ROLE: Editor.
INTENT: Improve clarity and wording of this structure without changing meaning.
CONSTRAINTS: No new ideas. No structural changes. No examples.
FORBIDDEN: Expansion, reorganization.
OUTPUT FORMAT: Same structure with clarified labels.
```

## **Template B — Tighten Logic**
```
ROLE: Editor.
INTENT: Clarify logical connections between sections.
CONSTRAINTS: Preserve all meaning and structure.
FORBIDDEN: Rewriting, adding new concepts.
OUTPUT FORMAT: Improved phrasing inside existing structure.
```

---

# Section 4 — Stress Tester Activation Templates

## **Template A — Identify Weaknesses**
```
ROLE: Stress Tester.
INTENT: Attack this document to identify vulnerabilities.
CONSTRAINTS: No solutions. No rewriting. No improvements.
FORBIDDEN: Fixing problems, reframing intent.
OUTPUT FORMAT: Bullet points listing contradictions, gaps, and risks.
```

## **Template B — Drift Detection**
```
ROLE: Stress Tester.
INTENT: Detect drift points in the provided output.
CONSTRAINTS: Identify problems only.
FORBIDDEN: Suggesting fixes or rewriting content.
OUTPUT FORMAT: Drift vector list.
```

---

# Section 5 — Polisher Activation Templates

## **Template A — Final Language Pass**
```
ROLE: Polisher.
INTENT: Refine language for readability without altering meaning.
CONSTRAINTS: No reordering. No new ideas. No structural changes.
FORBIDDEN: Expanding content, reframing ideas.
OUTPUT FORMAT: Clean, smooth prose.
```

## **Template B — Light Tone Polish**
```
ROLE: Polisher.
INTENT: Make this text more concise while keeping meaning identical.
CONSTRAINTS: Preserve structure exactly.
FORBIDDEN: Removal of meaning, tone shifts.
OUTPUT FORMAT: Improved but unchanged content.
```

---

# Section 6 — Interrupt and Recovery Templates

## **Template A — Light Drift Correction**
```
INTERRUPT: Drift detected.
ROLE: <same role>.
Restate intent: <intent>.
CONSTRAINTS: <constraints>.
Re-run the pass cleanly.
```

## **Template B — Moderate Drift**
```
INTERRUPT: Role contamination detected.
Stop and reset.
ROLE: <role>.
INTENT: <intent>.
CONSTRAINTS: <constraints>.
Begin fresh. Do not reference prior output.
```

## **Template C — Severe Drift**
```
HARD STOP: Severe drift.
Reset all reasoning.
ROLE: <role>.
INTENT: <intent>.
CONSTRAINTS: <constraints>.
Start over from scratch.
```

---

# Section 7 — Full Lockstep Workflow Template

This is the master script for multi-pass workflows.

```
PASS 1 — Architect:
<Insert Architect command block>

PASS 2 — Editor:
<Insert Editor command block>

PASS 3 — Stress Tester:
<Insert Stress Tester command block>

PASS 4 — Polisher:
<Insert Polisher command block>
```

Operator performs validation after each pass.

---

# Section 8 — Multi-Model Orchestration Template

Use this template when running workflows across multiple AI models.

```
MODEL 1 (Architect):
<Architect block>

MODEL 2 (Editor):
<Editor block>

MODEL 3 (Stress Tester):
<Stress Tester block>

MODEL 4 (Polisher):
<Polisher block>
```

Each model must respect strict separation of roles.

---

# Section 9 — Rapid-Fire Commands (Short Form)

These are shorthand phrases for power-operator use.

### **Architect**
```
“Architect: structure only. No prose.”
```

### **Editor**
```
“Editor: clarify without adding meaning.”
```

### **Stress Tester**
```
“Stress test: find weaknesses only.”
```

### **Polisher**
```
“Polish lightly. No structural edits.”
```

### **Interrupt**
```
“Interrupt. Role drift. Reset.”
```

---

# Section 10 — Why Templates Matter

Operator command templates:
- eliminate ambiguity  
- maintain control  
- enforce constraints  
- guarantee predictable outputs  
- prevent role mixing  
- reduce cognitive load  
- speed up complex workflows  

They form the **linguistic control layer**  
of the entire IRONBOUND-AI system.

---

End of file.