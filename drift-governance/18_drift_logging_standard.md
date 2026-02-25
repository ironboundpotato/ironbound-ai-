# Drift Logging Standard  
**IRONBOUND-AI Drift Governance System**  
**Document: 18_drift_logging_standard.md**

The Drift Logging Standard (DLS) is the unified method for documenting all drift events across projects, namespaces, sessions, and workflows.  
Its purpose is to provide:

- A consistent record  
- A machine-readable structure  
- Operator clarity  
- Cross-session memory  
- System-wide diagnostics  
- Governance compliance  

The log captures *what drift occurred, why, how severe it was, and what was done about it.*

---

# 1. Purpose of Drift Logging

Drift must be logged because:

- Long sessions accumulate hidden distortion  
- The watchdog requires historical data  
- Corrections must be traceable  
- Operator overrides must be documented  
- Certain drifts escalate into catastrophic states if ignored  
- Cross-project contamination requires pattern recognition  
- Future workflows depend on accurate drift history  

Logging ensures the IRONBOUND governance system is accountable and auditable.

---

# 2. What Must Be Logged

Every drift event — regardless of size — must be recorded.

The following categories **must** be logged:

### **1. Role Drift**  
Incorrect reasoning mode, role confusion, or wrong specialization.

### **2. Tone Drift**  
Tone mismatch, emotional contamination, wrong density level.

### **3. Format Drift**  
Structural inconsistencies, header deviations, pattern mismatch.

### **4. Intent Drift**  
Answering instead of generating, interpreting instead of obeying.

### **5. Scope Drift**  
Outputs exceed or underfill operator boundaries.

### **6. Confidence Drift**  
Output becomes unstable, overly certain, or uncertain.

### **7. Momentum Drift**  
Predictive inertia interfering with instruction precision.

### **8. Namespace Contamination**  
Cross-folder or wrong-domain reasoning.

### **9. Cross-Project Contamination**  
Project identity leak or conceptual bleed.

### **10. Meta Drift**  
Model begins generating commentary, disclaimers, reflection, or internal reasoning.

Any of these require immediate log entry.

---

# 3. Drift Severity Levels (0–5)

### **0 — Stable**  
No drift detected.

### **1 — Micro Drift**  
Minor tone or density shift.  
→ Quick reset (MMR).

### **2 — File-Level Drift**  
Structural or intent deviation.  
→ MRP-5 required.

### **3 — Namespace Drift**  
Cross-namespace contamination.  
→ MRP-X required.

### **4 — Session Drift**  
Multiple drifts across files.  
→ Hard reset + rebind.

### **5 — Catastrophic Drift**  
Cross-project contamination, collapse of constraints, or total misalignment.  
→ Full system reset.

Severity must always be logged.

---

# 4. Drift Log Format (DLS-6)

The official log entry has **six standardized fields**.

```text
[Timestamp]  
Category: (role/tone/format/intent/scope/confidence/momentum/namespace/project/meta)  
Severity: (0–5)  
Trigger: (what caused the detection)  
Symptoms: (what was observed)  
Action Taken: (MMR, MRP-5, MRP-X, purge, rebind, reset)