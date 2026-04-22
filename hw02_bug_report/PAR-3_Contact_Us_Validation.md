### **Bug Report PAR-3: Contact Us form missing validation**

**Title:** Contact Us form allows submission with empty fields
**Environment:** Firefox 149 and Chromium 147 (Environment-independent)

**Description:**
The "Contact Us" form does not validate that required fields (Name, Email, Phone, Message) are filled before submission. A user can send an empty support request, which results in "empty" records in the support system.

**Steps to Reproduce:**
1. Navigate to the ParaBank homepage.
2. Click on the **Contact Us** icon (envelope) or link.
3. Leave all fields (Name, Email, Phone, Message) empty.
4. Click the **Send to Support** button.

**Expected Result:**
The system should display validation errors for each required field (e.g., "Name is required") and prevent submission.

**Actual Result:**
The system displays a success message: "Thank you [Name]. A ParaBank representative will be contacting you." (even though [Name] is blank).

**Suggested Fix:**
Add client-side and server-side validation to ensure all fields are populated with valid data before allowing submission.
