# Customer Login Smoke Test Cases

| Test Case ID | Test Case Title | Test Steps | Expected Result |
| :--- | :--- | :--- | :--- |
| **ST-01** | **Verify Successful Login** | 1. Enter a valid **Username**.<br>2. Enter a valid **Password**.<br>3. Click the **LOG IN** button. | User is successfully logged in and redirected to the "Account Overview" page. |
| **ST-02** | **Verify Navigation to Registration** | 1. Click on the **Register** link. | User is redirected to the "Signing up is easy!" registration form page. |
| **ST-03** | **Verify Navigation to Forgot Login Info** | 1. Click on the **Forgot login info?** link. | User is redirected to the "Customer Lookup" page. |
| **ST-04** | **Verify Password Masking** | 1. Type any characters into the **Password** field. | Characters are masked (dots/asterisks) for security. |
| **ST-05** | **Basic Login Failure (Empty Fields)** | 1. Leave both fields blank.<br>2. Click the **LOG IN** button. | Error message is displayed; user is not logged in. |
| **ST-06** | **Verify Pasting Credentials (Login Manager Compatibility)** | 1. Copy a valid username and **Paste (Ctrl+V)** it into the Username field.<br>2. Copy a valid password and **Paste** it into the Password field.<br>3. Click **LOG IN**. | The fields accept pasted data, and the login is successful. |

