# Healthcare LIMS Testing Project  
QA project simulating a Laboratory Information Management System (LIMS), focusing on healthcare workflows, data validation, and patient safety.

---

## 🎯 What this project demonstrates
- QA for regulated healthcare environments  
- Risk-based testing with patient safety impact  
- Validation of clinical data (units, ranges, abnormal results)  
- Workflow testing across multiple steps  
- API + data integrity validation  

---

## 🛡️ Compliance Considerations
- Sensitive patient data handling  
- Data integrity for medical decision-making  
- Confidentiality and validation constraints  

---

## 🧩 Modules
- Patient registration  
- Test ordering  
- Sample tracking  
- Result management  

---

## 📊 Test Coverage
- Registration validation ✔️  
- Order validation ✔️  
- Sample lifecycle ✔️  
- Result validation ✔️  
- API validation ⚠️ partial  

---

## 🧠 QA Strategy
- Focus on critical data accuracy  
- Edge cases on medical ranges  
- Validation of abnormal conditions  
- Multi-step workflow integrity  

---

## 💼 Business Impact
Errors in this system can lead to:
- Incorrect medical decisions  
- Delayed diagnosis  
- Patient safety risks  

---

## 🐞 Sample Bug
**Title:** Critical patient results not flagged  

**Steps:**
1. Register patient  
2. Order potassium test  
3. Enter result: 9.8 mmol/L  
4. Retrieve result  

**Expected:** Critical flag = TRUE  
**Actual:** FALSE  

**Severity:** Critical  
**Priority:** High  

---

## 🧠 Root Cause Hypothesis
Potential failure in threshold validation logic for critical ranges.
