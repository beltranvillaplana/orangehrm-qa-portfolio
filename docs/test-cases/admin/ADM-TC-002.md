# ADM-TC-002 — Verify Duplicate Username Is Rejected

**Module:** Admin — User Management\
**Functionality:** Create User — Username Validation

### Preconditions

- The administrator is logged into OrangeHRM.
- An employee without an associated system user account exists in the PIM module.

### Test Steps

| Step | Action | Expected Result |
| ---- | ------ | --------------- |
| 1 | Navigate to **Admin → User Management** and click **Add**. | The Add User form is displayed. |
| 2 | Set **User Role** to ESS. | ESS is selected as the user role. |
| 3 | Search for and select the employee without an associated system user account. | The selected employee is displayed in **Employee Name**. |
| 4 | Set **Status** to Enabled. | The Enabled option is selected. |
| 5 | Enter the existing username in **Username** | The validation message “Already exists” is displayed below **Username**. |
| 6 | Enter a valid password and the same value in **Confirm Password**. | Both password fields are completed without validation errors. |
| 7 | Attempt to submit the form using **Save**. | The application prevents user creation and keeps the Add User form displayed with the duplicate username validation |
