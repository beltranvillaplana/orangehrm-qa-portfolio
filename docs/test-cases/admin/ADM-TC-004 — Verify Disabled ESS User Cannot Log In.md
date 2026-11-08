# ADM-TC-004 — Verify Disabled ESS User Cannot Log In

**Module:** Admin — User Management\
**Functionality:** User Status — Disable Account

### Preconditions

- The administrator is logged into OrangeHRM.
- An Enabled ESS user account exists with known valid credentials.
- Successful login with this ESS account has been verified, and its session has been closed.

### Test Steps

| Step | Action | Expected Result |
|---|---|---|
| 1 | Navigate to **Admin → User Management** and search for the ESS account using its complete username. | The matching user is displayed. |
| 2 | Click **Edit** for the matching user. | The Edit User form is displayed. |
| 3 | Set **Status** to Disabled and click **Save**. | The change is saved, and the application returns to the users list. |
| 4 | Search for the same username and check its status. | The account is displayed with Disabled status. |
| 5 | Open the login page in a separate private window with no active session. | The login form is displayed. |
| 6 | Enter the ESS account’s valid username and password, then click **Login**. | Access is denied, the login page remains displayed, and the message “Account disabled” appears. |

### Cleanup

- Restore the ESS account’s status to **Enabled** using the administrator session.
