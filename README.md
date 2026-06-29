
# Lab: Identity & Access Management (IAM)

## Objective
To implement a secure and scalable Identity and Access Management strategy within an Active Directory environment. This lab focuses on user provisioning, organizational structure, and role-based access control (RBAC) to ensure the Principle of Least Privilege.

## Technical Environment
- **Domain Controller:** Windows Server 2022
- **Management Tool:** Active Directory Users and Computers (ADUC)
- **Key Concepts:** Organizational Units (OUs), Security Groups, User Account Lifecycle

## Lab Workflow: Step-by-Step

### 1. Organizational Unit (OU) Design
* Designed a hierarchical OU structure (e.g., *Company -> Departments -> IT, HR, Sales*) to logically organize users and delegate administrative authority.
* Created specialized OUs for service accounts and computer objects to improve network maintainability.

### 2. User & Group Provisioning
* Created standardized user accounts following enterprise naming conventions.
* Implemented **Security Groups** based on job functions (e.g., *Sales_Group, IT_Admins*).
* Assigned users to these groups to streamline permission management rather than assigning permissions on a per-user basis.

### 3. Account Lifecycle Management
* Configured **Password Policies** (complexity, history, and lockout thresholds) to protect against unauthorized access.
* Practiced account maintenance, including disabling/enabling accounts, resetting passwords, and handling account lockouts.
* Simulated user onboarding and offboarding by moving accounts between OUs and updating group memberships.

### 4. Delegation of Administration
* Practiced the concept of "Delegation of Control" by granting specific, limited administrative permissions (e.g., password resets) to a junior-level security group, demonstrating an understanding of tiered administration.

## Proof of Implementation
*(Replace the following with your actual file names)*
* **ADUC Structure:** ![OU Hierarchy](aduc-ou-structure.png)
* **Group Membership:** ![Group Members](group-membership.png)

## Key Learnings
* **Security Principles:** Developed a deeper understanding of the **Principle of Least Privilege**—ensuring users have exactly the access they need, and no more.
* **Scalability:** Learned how group-based management significantly reduces the administrative overhead of managing large numbers of users.
* **Audit Readiness:** Understood the importance of structured OUs for creating readable, audit-friendly environments for enterprise security compliance.
