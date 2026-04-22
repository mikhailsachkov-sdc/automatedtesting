### **Bug Report PAR-4: Bill Pay missing field validation**

**Title:** Bill Pay module allows submission of empty form
**Environment:** Firefox 149 and Chromium 147 (Environment-independent)

**Description:**
The "Bill Pay" form does not validate that required payee information is provided. Clicking "Send Payment" without any data results in an inconsistent UI state or a successful submission message for a null transaction.

**Steps to Reproduce:**
1. Log in to ParaBank.
2. Navigate to **Bill Pay**.
3. Leave all fields (Payee Name, Address, City, State, Zip Code, Phone, Account, Verify Account, Amount) empty.
4. Click **Send Payment**.

**Expected Result:**
The form should highlight missing fields with error messages (e.g., "Payee name is required") and block the transaction.

**Actual Result:**
The system proceeds to the confirmation page, often showing "Bill Payment Service" with no details or a generic error that does not specify the missing fields.

**Suggested Fix:**
Implement mandatory field validation on the Bill Pay form to ensure all payee and transaction details are provided before processing.
