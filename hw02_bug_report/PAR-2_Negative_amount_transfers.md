### **Bug Report PAR-2: Negative amount transfers**

**Title:** Transfer Funds module allows negative amounts
**Environment:** Firefox 149 and Chromium 147 (Environment-independent)

**Description:**
The "Transfer Funds" logic does not validate that the transfer amount is a positive integer. Entering a negative value reverses the transaction logic, allowing users to move money from the destination account into the source account.

**Steps to Reproduce:**
1. Log in to ParaBank.
2. Navigate to **Transfer Funds**.
3. Select a source account (Account A) and a destination account (Account B).
4. In the **Amount** field, enter `-500`.
5. Click **Transfer**.
6. Check **Account Services** balances.

**Expected Result:**
The system should trigger a validation error (e.g., "Amount must be greater than zero") and block the transaction.

**Actual Result:**
The system displays "Transfer Complete!" Account A's balance increases by $500, and Account B's balance decreases by $500.

**Suggested Fix:**
Implement server-side validation to ensure the `amount` parameter is greater than zero before processing the transaction.

