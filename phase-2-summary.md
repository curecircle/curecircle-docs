# CureCircle – Phase 2: Multi-Step Registration Form

This document summarizes the four steps implemented in the multi-step registration form of the CureCircle platform.

---

## 📄 File:
`/frontend/signup-bootstrap.html`

---

### 🔹 Step 1: Select Role
A dropdown allows the user to select their role:
- Student
- Graduate – Medical
- Graduate – Nursing

The selected role determines which document the user needs to upload in Step 3.

---

### 🔹 Step 2: Academic Path
The user navigates through four dependent dropdowns:
1. Faculty  
2. Degree  
3. Field  
4. Subspecialty

These are dynamically loaded from the JSON file:
`/config/academic_structure_full.json`

Each dropdown is enabled only after the previous one is selected.

---

### 🔹 Step 3: Upload Document
The user uploads a required document.
- The upload label updates dynamically based on the selected role.
- If the file is an image, a preview is displayed.
- If it's a PDF or other file, a default icon is shown instead.

---

### 🔹 Step 4: Summary
A Bootstrap-styled table summarizes the user’s input:
- Selected Role
- Faculty
- Degree
- Field
- Subspecialty
- Uploaded file name

This step ends with a **non-functional Submit button** (as placeholder for future backend connection).

---

✅ This completes Phase 2. Messaging, notifications, and chat features will begin in Phase 3.
