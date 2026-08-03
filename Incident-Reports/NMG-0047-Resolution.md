# Incident Report: NMG-0047

## Ticket Information

**Ticket Number:** NMG-0047  
**Affected User:** Jane Cooper (jcooper@NMG.com)  
**Priority:** High  
**Resolved By:** IT New Hire  
**Date Resolved:** July 25, 2026

---

## Issue Reported

Jane Cooper was unable to access HR shared resources. Although she could successfully log into her computer, she received **"Access Denied"** when attempting to access HR systems. Her desktop policies, mapped drives, and overall user environment also differed from those of her HR teammates.

---

## Root Cause Analysis

The investigation determined that Jane Cooper's Active Directory account had been configured incorrectly in two ways:

- Her user account was located in the **Operations Organizational Unit (OU)** instead of the **HR OU**.
- She was assigned to the **Operations-Users** security group instead of the **HR-Users** security group.

Because Active Directory applies permissions and policies based on Organizational Units and security group membership, Jane received the Operations configuration instead of the HR configuration. This resulted in incorrect desktop policies, mapped drives, and denied access to HR resources.

---

## Resolution

The following corrective actions were performed:

1. Moved Jane Cooper's Active Directory account from the **Operations OU** to the **HR OU**.
2. Removed her membership from the **Operations-Users** security group.
3. Added her to the **HR-Users** security group.
4. Verified that her account reflected the correct Organizational Unit and security group membership.

---

## Verification

The issue was verified by:

- Confirming Jane's account appeared within the **HR Organizational Unit**.
- Confirming her membership in the **HR-Users** security group.
- Verifying that the incorrect Operations group membership had been removed.
- Confirming the Active Directory configuration matched the intended HR user configuration.

---

## Lessons Learned

This incident demonstrated that user access issues are not always caused by passwords or authentication failures. Incorrect Organizational Unit placement and security group assignments can also affect permissions, desktop policies, mapped drives, and resource access. Performing a structured investigation before making changes helped identify and resolve the root cause efficiently.
