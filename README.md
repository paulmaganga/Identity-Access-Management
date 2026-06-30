
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
* <img width="1003" height="747" alt="Creating Groups" src="https://github.com/user-attachments/assets/7d0c6642-9e94-43ca-8e8d-684283daddef" />


### 3. Account Lifecycle Management
* Configured **Password Policies** (complexity, history, and lockout thresholds) to protect against unauthorized access.
* Practiced account maintenance, including disabling/enabling accounts, resetting passwords, and handling account lockouts.
* Simulated user onboarding and offboarding by moving accounts between OUs and updating group memberships.

### 4. Delegation of Administration
* Practiced the concept of "Delegation of Control" by granting specific, limited administrative permissions (e.g., password resets) to a junior-level security group, demonstrating an understanding of tiered administration.
* <img width="1013" height="783" alt="Creating User and Password" src="https://github.com/user-attachments/assets/278b0b89-bcda-404d-8d98-7d49d6f86764" />
<img width="1005" height="780" alt="Creating Permission" src="https://github.com/user-attachments/assets/ef50bdbb-e07f-480f-82e1-08d2439ac8cc" />
<img width="1016" height="867" alt="New User changing Password" src="https://github.com/user-attachments/assets/c6d3d493-2ca3-4e68-b4b6-5457767b97b7" />



## Key Learnings
* **Security Principles:** Developed a deeper understanding of the **Principle of Least Privilege**—ensuring users have exactly the access they need, and no more.
* **Scalability:** Learned how group-based management significantly reduces the administrative overhead of managing large numbers of users.
* **Audit Readiness:** Understood the importance of structured OUs for creating readable, audit-friendly environments for enterprise security compliance.
