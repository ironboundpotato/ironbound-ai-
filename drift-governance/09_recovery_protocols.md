# Recovery Protocols  
**IRONBOUND-AI Drift Governance System**  
**Document: 09_recovery_protocols.md**

Recovery is the controlled return to aligned operation after drift.  
Interruption stops the damage.  
**Recovery restores the system.**

This protocol standardizes the post-drift stabilization sequence.

---

# 1. Recovery Overview

Drift recovery follows four phases:

1. **Stabilize** — stop contamination and reassert constraints  
2. **Rebind** — reconnect the model to operator intent and boundaries  
3. **Regenerate** — produce corrected output  
4. **Verify** — confirm alignment and update state  

Each phase has soft and hard variants depending on severity.

---

# 2. Soft Recovery Protocol  
Use when drift is mild, localized, or caught early.

### **When to Use**
- Tone stray within a few sentences  
- Minor format deviation  
- Early-stage hedging or overconfidence  
- Scope expansion <10%  

### **Procedure**

1. **Issue Soft Stop**  
   - “Pause. Reassess alignment.”

2. **Re-assert Boundaries**  
   - “Return to instruction. No additions.”

3. **Rebind to Intent**  
   - “Restate my instruction verbatim.”

4. **Controlled Regenerate**  
   - “Regenerate only the affected section.”

5. **Quick Verification**  
   - Tone: “Regenerate with tone-neutral.”  
   - Format: “Show skeleton only.”  

**Outcome:** Model resumes correct output without full reset.

---

# 3. Hard Recovery Protocol  
Use when drift is moderate to severe or cascading.

### **When to Use**
- Role drift  
- Intent hijack  
- Severe tone contamination  
- Format collapse  
- Overconfidence/hedging loops  
- Any output that “feels wrong everywhere”

### **Procedure**

1. **Issue Hard Stop**  
   - “STOP. Drift detected.”

2. **Full Constraint Reassertion**  
   - “Reset role, tone, intent, format.”

3. **Rebind to Operator Intent**  
   - “State my instruction exactly.”

4. **Full Regeneration**  
   - “Regenerate clean from zero contamination.”

5. **Validation Sweep**  
   - “Confirm structure.”  
   - “Confirm boundaries.”  
   - “Confirm confidence=neutral.”  

**Outcome:** System returns to a clean baseline.

---

# 4. Structural Reset Protocol  
Use for worst-case structural failures or multi-drift contamination.

### **When to Use**
- Output breaks its container  
- Model begins inventing tasks  
- Multi-layer drift (role + tone + format + intent)  
- Output no longer resembles the goal  

### **Procedure**

1. **System Halt**  
   - “STOP. Full contamination detected.”

2. **Zero-State Reset**  
   - “Return to zero-state alignment.”

3. **Reconstruct Skeleton**  
   - “Show skeleton only — no content.”

4. **Boundary Hard-Lock**  
   - “Bind to this structure. No deviation allowed.”

5. **Controlled Rebuild**  
   - Add content section-by-section  
   - Operator verifies after each segment  

6. **Final Integrity Scan**  
   - “Verify intent, tone, format, scope, confidence.”

**Outcome:** A full structural rebuild without legacy drift.

---

# 5. Cascade-Drift Containment  
Drift rarely stays isolated — it spreads.  
This protocol stops multi-drift before failure.

### **Cascade Indicators**
- Tone shifts trigger confidence drift  
- Scope drift pulls in intent drift  
- Format collapse triggers role confusion  
- Output becomes unpredictable  

### **Procedure**

1. **Containment Command**  
   - “Stop. Contain to scope.”

2. **Identify Root Drift**  
   Use the Drift Detection Matrix.

3. **Prioritize Correction**  
   - Intent → Tone → Role → Format → Scope → Confidence  
   This is the correct stabilization order.

4. **Reassert Constraints**  
   - “Reset intent, tone, and boundaries.”

5. **Regenerate Clean**  
   - Full or partial depending on root drift severity.

**Outcome:** Multi-drift chains are broken.

---

# 6. Confidence Recalibration Protocol  
After confidence drift, trust must be restored.

### **Procedure**

1. **Neutralize Confidence**  
   - “Regenerate with confidence=neutral.”

2. **Remove Apologies / Authority Claims**  
   - “Purge apologies and certainty.”

3. **Re-check Density & Tone**  
   Confidence affects both.

4. **Rebind to Intent**  
   - “Restate my instruction exactly.”

5. **Regenerate Clean**  

**Outcome:** Certainty matches operator intent.

---

# 7. Return-to-Operation Rules (RTO)

To safely resume normal interaction:

### **RTO-1: Intent Lock**
Model must repeat operator intent with zero drift.

### **RTO-2: Format Integrity**
Skeleton must match the template 1:1.

### **RTO-3: Tone Neutrality**
No emotional, dramatic, soft, or hype signals.

### **RTO-4: Boundary Adherence**
Model must state the task limits clearly.

### **RTO-5: Confidence Calibration**
Neutral confidence unless otherwise assigned.

### **RTO-6: Drift-Free Regenerate**
One clean output validates recovery.

### **RTO Final: Operator Approval**
Only the operator can declare recovery complete.

---

# 8. Principle of Recovery

> **“Interruption stops the damage.  
Recovery restores control.”**  

Drift will occur.  
Recovery protocols ensure it never compounds.

---

End of Document