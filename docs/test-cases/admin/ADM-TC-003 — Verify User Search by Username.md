# ADM-TC-003 — Verify User Search by Username

**Module:** Admin — User Management\
**Functionality:** Search Users

### Preconditions

- The administrator is logged into OrangeHRM.
- A system user account with a known username exists.

### Test Steps

| Step | Action | Expected Result |
|---|---|---|
| 1 | Navigate to **Admin → User Management**. | The users list and search filters are displayed. |
| 2 | Ensure all search filters are empty or set to their default values. | No additional search criteria are applied. |
| 3 | Enter the complete existing username in the **Username** search field. | The entered username is displayed in the field. |
| 4 | Click **Search**. | The matching user is displayed in the results, with the expected username, user role, employee name, and status. |
