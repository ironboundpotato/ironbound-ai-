# Operator Overrides  
**IRONBOUND-AI Drift Governance System**  
**Document: 11_operator_overrides.md**

Operator Overrides are the *highest authority commands* within the IRONBOUND system.  
They bypass model heuristics, halt autonomous reasoning, and force absolute compliance.

Overrides exist to ensure:

- The **operator is always the source of truth**  
- The model never self-directs  
- Drift cannot escalate into a control failure  
- Long-session entropy cannot dethrone instruction hierarchy  

This file defines every override and its use-case.

---

# 1. Override Principles

### **1.1 Operator Supremacy**
> The operator’s words outrank all model reasoning, memory, assumptions, and prior context.

### **1.2 No Negotiation**
Overrides are not suggestions — they replace the model’s internal decision-making.

### **1.3 Immediate Execution**
Overrides must be obeyed *before* the model continues.

### **1.4 Drift Immunity**
Overrides bypass drift contamination and reestablish alignment.

---

# 2. Core Override Commands

## 2.1 Directive Override
Forces the model to obey the operator’s last instruction *exactly*.

- **“Operator override: follow my last instruction only.”**  
- **“Ignore heuristics. Execute as stated.”**

Use this when the model begins reinterpreting or “helping.”

---

## 2.2 Authority Override
Reasserts hierarchy during tone, intent, or confidence drift.

- **“Operator authority override — yield control.”**  
- **“Stop self-direction. I am the sole decision-maker.”**

Use when the model apologizes, over-explains, or asserts authority.

---

## 2.3 Boundary Lock Override
Forces strict adherence to task limits.

- **“Override: lock boundaries exactly as defined.”**  
- **“You may not expand or contract this task.”**

Use during scope drift or long-session inflation.

---

## 2.4 Format Override
Prevents the model from altering structure.

- **“Format override: replicate the template exactly.”**  
- **“No deviations from the structure.”**

Use when format drift appears.

---

## 2.5 Tone & Confidence Override
Corrects emotional or certainty contamination.

- **“Tone override: return to neutral immediately.”**  
- **“Confidence override: set confidence=zero.”**

Use when hedging, hype, softness, or swagger arises.

---

## 2.6 Intent Override
Replaces incorrect model interpretation with operator-defined purpose.

- **“Intent override: the purpose is what *I* say it is.”**  
- **“You may not reinterpret the task.”**

Use anytime the model deviates from the operator’s desired goal.

---

## 2.7 Role Override
Resets the model to the proper functional role.

- **“Role override: you are functioning as [ROLE] only.”**  
- **“Drop all other roles immediately.”**

Use when role drift is identified or suspected.

---

# 3. Emergency Overrides (Critical)

Emergency overrides rewrite *all active reasoning pathways*.

## 3.1 Total Override Reset
- **“TOTAL OVERRIDE: reset role, tone, intent, format, boundaries.”**

Use during multi-drift or structural collapse.

---

## 3.2 Contamination Purge Override
- **“OVERRIDE: purge all drift contamination. Return to zero-state alignment.”**

Use during cascading drift or long-session entropy events.

---

## 3.3 Instruction Rebinding Override
- **“OVERRIDE: restate my instruction verbatim before continuing.”**

Use when intent corruption is suspected.

---

## 3.4 Hard Compliance Override
- **“OVERRIDE: comply exactly. No inference, no expansion.”**

Use when the model begins improvising.

---

# 4. Conflict Resolution Overrides

When model interpretation and operator intention diverge:

### **4.1 Clarification Override**
- **“Override: my instruction supersedes your interpretation.”**

### **4.2 Priority Override**
- **“Override: prioritize my explicit phrasing over all internal logic.”**

### **4.3 Memory Override**
- **“Override: disregard all earlier assumptions unless I confirm them.”**

---

# 5. Override Use in Long Sessions

Long sessions require periodic override reinforcement:

- **“Operator override: re-anchor to my constraints.”**  
- **“Override: reset momentum. Tone=neutral, confidence=neutral.”**  

Overrides prevent the model from drifting toward self-steering behavior.

---

# 6. Multi-Stage Workflow Overrides

For large projects (frameworks, filesystems, canon construction):

### Before each file:
- **“Override: bind to this directory and filename only.”**

### Before each major output:
- **“Override: replicate format exactly.”**

### After detecting micro-drift:
- **“Override: re-align and regenerate clean.”**

---

# 7. Operator Verification Overrides

To ensure the override took effect:

- **“Override: confirm your role.”**  
- **“Override: confirm my intent.”**  
- **“Override: show skeleton only.”**  
- **“Override: state the task boundaries.”**

If any confirmation fails → enact Total Override Reset.

---

# 8. Guiding Principle

> **“Overrides are the emergency brakes of alignment.  
When drift takes the wheel, overrides take it back.”**

Operator overrides maintain hierarchy, enforce obedience, and guarantee stable operation.

---

End of Document