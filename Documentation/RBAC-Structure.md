# Role-Based Access Control (RBAC) Structure

| Department | Organizational Unit (OU) | Security Group Name | Assigned Users (Usernames) | Access Level / Permissions |
| :--- | :--- | :--- | :--- | :--- |
| Finance | OU=Finance,DC=NMG,DC=com | Finance-Users | dchen, kmills, rhayes, lpark | Access to finance files, payroll systems, and departmental shared drives |
| HR | OU=HR,DC=NMG,DC=com | HR-Users | storres, jwhitfield, mgrant, jcooper | Access to employee records, payroll systems, benefits portal, and onboarding documentation |
| IT | OU=IT,DC=NMG,DC=com | IT-Users | mjohnson, ppatel, tbrooks, acoleman | Domain administration, service desk systems, and core network configuration access |
| Operations | OU=Operations,DC=NMG,DC=com | Operations-Users | bfoster, crivera, nross | Access to facility controls, scheduling applications, and logistics shared folders |

---

## RBAC Design Summary

This Active Directory environment uses Role-Based Access Control (RBAC) to assign permissions based on each employee's department rather than individual user accounts. Users are organized into departmental Organizational Units (OUs) and assigned to department-specific security groups. This approach simplifies administration, improves consistency, and reduces the risk of permission errors when onboarding or managing employees.
