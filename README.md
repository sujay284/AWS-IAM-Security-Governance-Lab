# AWS IAM Security: Identity Governance & Resource Isolation

## Project Overview
This project demonstrates the implementation of fine-grained access control using **AWS Identity and Access Management (IAM)**. In this lab, I configured advanced security policies using **JSON Policy Variables** to ensure that users could only access their specific resources, following the **Principle of Least Privilege (PoLP)**.

---

## Technical Skills Demonstrated
* **Identity Governance:** Created and managed IAM users, groups, and permissions.
* **Dynamic Access Control:** Implemented `${aws:username}` policy variables to allow for scalable and secure resource isolation.
* **Secure Programmatic Access:** Authenticated and managed AWS resources via the **AWS CLI** using secure Access/Secret keys.
* **Security Auditing:** Verified security enforcement by troubleshooting and validating `AccessDenied` errors.

---

## Lab Architecture & Workflow
1. **Policy Configuration:** Developed a JSON policy that dynamically grants S3 access based on the requester's IAM username.
2. **Identity Management:** Grouped users and attached the custom security policies.
3. **CLI Authentication:** Used `aws configure` to establish a secure session from a terminal environment.
4. **Security Validation:** Tested the "Boundaries" of the policy by attempting to access unauthorized buckets and confirming that access was blocked.

---

## Project Validation (Screenshots)
To maintain a clean repository, all technical evidence is uploaded as separate files in this repository. Please refer to these files for proof of completion:

* **Image 1`**: Demonstrates the IAM policy correctly blocking unauthorized access.
* **`Image 2`**: Shows successful authentication and data download via the CLI.
* **`Image 3`**: Verification of secure terminal access using AWS Systems Manager.

---

## Conclusion
This lab reinforces the critical nature of identity-based security in cloud environments. By using dynamic variables rather than hard-coded permissions, I demonstrated how to build a scalable security architecture that protects data integrity and maintains strict isolation between users.
