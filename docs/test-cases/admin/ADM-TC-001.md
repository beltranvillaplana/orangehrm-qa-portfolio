# ADM-TC-001 — Verify Successful Creation of an ESS User

**Module:** Admin — User Management  
**Functionality:** Create User

### Preconditions

- The administrator is logged into OrangeHRM.
- An employee without an associated system user account exists in the PIM module.

### Test Steps

| Step | Action | Expected Result |
|---|---|---|
| 1 | Navigate to **Admin → User Management** and click **Add**. | The Add User form is displayed. |
| 2 | Set **User Role** to ESS. | ESS is selected as the user role. |
| 3 | Set **Status** to Enabled. | The Enabled option is selected. |
| 4 | Search for and select an existing employee in **Employee Name**. | The selected employee is displayed in the field. |
| 5 | Enter a valid username following the criteria: `nameSurnameRole`. | The username is accepted without validation errors. |
| 6 | Enter a valid password that meets the application's password requirements. | The password is accepted without validation errors. |
| 7 | Enter the same password in **Confirm Password**. | The confirmation password is accepted without validation errors. |
| 8 | Click **Save**. | The user is created successfully, and the application redirects to **Admin → User Management**, displaying the users list. |
| 9 | Verify that the newly created user appears in the users list. | The user is displayed with the expected username, ESS role, associated employee, and Enabled status. |
