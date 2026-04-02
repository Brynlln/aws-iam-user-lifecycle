# aws-iam-user-lifecycle
AWS IAM project demonstrating Joiner, Mover, Leaver lifecycle with RBAC
# AWS IAM User Lifecycle Project (Joiner–Mover–Leaver)

## Overview

This project demonstrates a full Identity and Access Management (IAM) lifecycle using AWS.
It simulates how organizations manage user access securely through onboarding, role changes, and offboarding.

---

##  Objectives

* Implement IAM user lifecycle (Joiner, Mover, Leaver)
* Apply Role-Based Access Control (RBAC)
* Enforce least privilege principles
* Demonstrate secure deprovisioning

---

##  Technologies Used

* AWS IAM (Identity and Access Management)
* AWS Management Console

---

##  Project Breakdown

### 1. Joiner (User Creation)

* Created IAM user `john.doe`
* Granted initial access via **Developers group**
* Attached policy: `AmazonS3ReadOnlyAccess`

Screenshots:

* User creation
* Group assignment

---

### 2. Mover (Role Change / Privilege Escalation)

* Added user to **Admins group**
* Assigned `AdministratorAccess` policy
* Simulated promotion and increased access

Screenshots:

* Admin group creation
* Permission upgrade

---

### 3. Leaver (Deprovisioning)

* Removed user `john.doe`
* Ensured complete access revocation

Screenshots:

* Before deletion
* Deletion confirmation
* After deletion

---

## Key Concepts Demonstrated

* Identity lifecycle management
* Role-Based Access Control (RBAC)
* Least privilege vs privilege escalation
* Secure user deprovisioning
* Prevention of orphaned accounts

---

## Resume Value

This project demonstrates hands-on experience with:

* AWS IAM user and group management
* Access control design and enforcement
* Real-world security best practices

---

## 📁 Project Structure

```
screenshots/
  ├── joiner/
  ├── mover/
  ├── leaver/
```

---

## Future Improvements

* Implement MFA for users
* Create custom IAM policies
* Integrate with Active Directory (hybrid IAM)
* Automate provisioning using scripts or Terraform
