# Format Drift  
**IRONBOUND-AI Drift Governance System**  
**Document: 03_format_drift.md**

---

## 1. Definition

**Format Drift** is a structural deviation from the required output shape.  
It occurs when the model changes:

- layout  
- markdown structure  
- numbering  
- spacing  
- indentation  
- output type  
- requested container (code block, table, bullet list, etc.)

Format Drift is not cosmetic — it is a **loss of structural obedience** and affects every downstream component.

Format is the spine of IRONBOUND-AI outputs.  
If the spine bends, the entire body collapses.

---

## 2. Causes of Format Drift

Format Drift appears when:

1. **The model attempts to “improve” structure**  
2. **Context window contamination** alters prior formatting  
3. **Ambiguity in instructions** leaves format unspecified  
4. **Multi-part tasks** blur format expectations  
5. **Density shifts** cause structure to compress or expand  
6. **The model tries to anticipate next steps**  
7. **Hedging or tone drift** creates extra commentary outside structure  

Most format failures begin with the model second-guessing the output container.

---

## 3. Detection Signals

Format Drift is one of the easiest—and most critical—forms of drift to detect.

Key indicators:

### **A. Structural Deviations**
- Missing headings  
- Incorrect numbering (1. → 1)  
- Subtle indentation shifts  
- Failure to use the requested code block  
- Switching list formats mid-output  

### **B. Output Container Violations**
- Adding commentary before or after code blocks  
- Mixing markdown with prose when clean separation was required  
- Returning text instead of tables  
- Breaking the workflow format (Path → Filename → Instruction → Content)  

### **C. Alignment Violations**
- Overly compressed structure  
- Overly expanded structure  
- Reflowing paragraphs when not asked  

### **Critical Signal:**  
> The output no longer matches the operator-defined shape.

Format must be **obeyed**, not interpreted.

---

## 4. Severity Levels

### **Level 1 — Mild Format Drift**
- Minor indentation errors  
- Slight spacing inconsistencies  
- Markdown rendering quirks  

**Fix:** Local correction; continue.

---

### **Level 2 — Moderate Format Drift**
- Output not wrapped in required container  
- Extra text before/after code blocks  
- Incorrect section labeling  

**Fix:**  
Reassert required format → Regenerate section.

---

### **Level 3 — Severe Format Drift**
- Model abandons the structure entirely  
- Combines multiple formats  
- Inserts commentary that corrupts the file  

**Fix:**  
Full stop → Reset format → Regenerate entire output.

---

## 5. Examples of Format Drift

### ❌ **Commentary before the requested format**
User: “Give the content only inside a code block.”  
Model:  
> “Sure! Here you go:”  
> ```markdown  
> …  
> ```

Hard fail.

---

### ❌ **Switching list types halfway**
- 1.  
- 2.  
— Bullet suddenly appears instead of number.

---

### ❌ **Breaking workflow**
Operator: “Path → Filename → Instruction → Content.”  
Model responds:  
- “Here's the file!”  
- And mixes sections in the wrong order.

---

### ❌ **Markdown hierarchy collapse**
H2 suddenly becomes H4.  
H1 repeated unnecessarily.  

---

### ❌ **Merged structure**
Combining multiple conceptual sections into one block without headings.

---

## 6. Correction Procedure

### **Step 1 — Halt Output**
Stop immediately.

### **Step 2 — Restate Format Requirements**
Example:  
> “Use the exact workflow format: Path, Filename, Instruction, File Content.”

### **Step 3 — Reassert Structure Constraints**
- No commentary  
- No preamble  
- No mixing containers  
- Strict markdown discipline  

### **Step 4 — Regenerate Affected Section**
Always clean, never patched.

---

## 7. Format Drift Prevention

Prevention requires:

- Explicit structure commands  
- Isolated containers for content  
- Avoiding compound instructions  
- Resetting markdown hierarchy before major outputs  
- Using canonical workflow templates  
- Treating structure as law, not suggestion  

Format is the **contract** between operator and model.

---

## 8. Relationship to Other Drifts

- **Tone Drift:** Tone contamination often introduces unwanted text outside structure.  
- **Role Drift:** Wrong-role behavior leads to incorrect formatting (e.g., Polisher rewriting headings).  
- **Intent Drift:** Misinterpreted tasks lead to altered format.  
- **Confidence Drift:** Overconfident models often restructure outputs “because they think it’s better.”  

Format Drift is diagnostic:  
> When format slips, governance must intervene.

---

## 9. Guiding Principle

> **“Structure is not decoration — it is obedience.”**

A model that cannot obey format cannot obey anything.

---

End of Document