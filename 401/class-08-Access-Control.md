## Access Control (ACL)

Given a proper and valid user with a set of permissions, we can grant or restrict access to anything in our server.

### Reading
___
### [5 steps to RBAC](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)

#### What is Role Based Access Control (RBAC) 
"RBAC is the idea of assigning system access to users based on their role within an organization. The system needs of a given workforce are analyzed, with users grouped into roles based on common job responsibilities and system access needs. Access is then assigned to each person based strictly on their role assignment. With tight adherence to access requirements established for each role, access management becomes much easier."

#### Why do we care?
"With the proper implementation of RBAC, the assignment of access rights becomes systematic and repeatable. Further, it is much easier to audit user rights, and to correct any issues identified."

#### Describe a Role/Permission heirarchy that you might implement using RBAC.

"You might have a basic user role, which includes the access any employee would need, such as email and the intranet site. Another role might be a customer service rep, that would have read/write access to the customer database, and a customer database administrator, that would have full control of the customer database. "

#### What approach might you take to implement RBAC?

* ***Identify Roles:*** Start by identifying the different roles or groups of users that exist within your system. For example, you may have roles such as "Admin," "Manager," "Employee," or "Guest." Each role represents a specific set of permissions and privileges.

* **Define Permissions**: Once you have identified the roles, define the permissions associated with each role. Permissions can be actions or operations that a user is allowed or restricted to perform. For example, an admin role might have permissions like "create user," "delete user," or "manage settings," while an employee role might only have permissions like "view documents" or "submit requests."

* **Assign Roles to Users**: Assign appropriate roles to each user in your system based on their responsibilities and access requirements. This can be done during user registration or through an administration interface. Make sure to consider the principle of least privilege, where users are only granted the minimum permissions necessary to perform their tasks.

* **Implement Access Control:** In your application's code or security layer, implement access control mechanisms that check the user's role and the required permissions for accessing certain resources or performing specific actions. This can be done through conditional statements or by integrating RBAC libraries or frameworks provided by your programming language or framework of choice.

* **Role Assignment and Management**: Provide functionality to assign and manage roles dynamically. This allows administrators to add or remove roles from users as their responsibilities change. Additionally, consider implementing features like role inheritance, where a user can inherit permissions from higher-level roles.

* **Regular Auditing and Review**: Periodically review and audit your RBAC implementation to ensure that roles and permissions are appropriately assigned and that there are no security loopholes. Remove any unnecessary or unused roles and permissions, and update access control rules as needed.

[Wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)

#### If Authentication is “you are who you say you are,” what is Authorization?

You have permission to do what you are doing.

#### Name three primary rules defined for RBAC.

Three primary rules are defined for RBAC:

1. **Role assignment:** A subject can exercise a permission only if the subject has selected or been assigned a role.
2. **Role authorization:** A subject's active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized.
3. **Permission authorization:** A subject can exercise a permission only if the permission is authorized for the subject's active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized.


#### Describe RBAC to a non-technical friend.

In simple terms, RBAC is like having different keys that open different rooms based on your role or position within a system. It helps ensure that people can only access what they need to do their job or fulfill their responsibilities while keeping everything else secure.



### Videos

[RBAC tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)

#### What Are access rights Associated with? The User? or The Role? Explain.

"Access rights are associated with roles in RBAC. Roles define the different responsibilities or positions within a system, and access rights determine what actions or resources a role is allowed to access. Users are then assigned to specific roles, and by inheriting the access rights associated with those roles, they are granted the corresponding permissions.


#### Access Rights, or Authorization, is activated after a user successfully does what?

Access rights, or authorization, are activated after a user successfully authenticates themselves. Authentication is the process of verifying the identity of a user, typically through a username and password or other means of identification. Once the user's identity is confirmed, authorization comes into play, where the system determines what actions or resources the user is permitted to access based on their assigned role and associated access rights.




#### Explain how RBAC might benefit a business.

RBAC can benefit a business in several ways:

1. **Improved Security:** RBAC helps enforce the principle of least privilege, ensuring that users only have access to the resources necessary for their role. This reduces the risk of unauthorized access and potential security breaches.

2. **Simplified Access Management:** RBAC simplifies the process of granting and revoking access rights. Instead of managing permissions for each user individually, access can be managed at the role level. This streamlines access management and reduces administrative overhead.

3. **Enhanced Compliance:** RBAC provides a clear audit trail by associating actions and resource access with specific roles. This can help with compliance requirements by demonstrating that access is controlled and monitored, which is important for industries with regulatory standards.

4. **Increased Efficiency:** RBAC improves efficiency by ensuring that users have access to the resources they need to perform their roles effectively. It eliminates the time-consuming process of requesting and granting access on a case-by-case basis.

5. **Scalability and Flexibility:** RBAC accommodates changes in organizational structure and user roles without significant administrative effort. It allows businesses to scale and adapt their access management easily as roles evolve or new roles are added.

Overall, RBAC provides a structured and organized approach to access control, enhancing security, simplifying administration, supporting compliance, and improving operational efficiency for businesses of all sizes." -ChatGPT


### Reflection

What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-08/)?

Know how to add access controls.

### Things I want to know more about

It will be interesting to see how all this is implemented within the code. 