##  <Login /> and <Auth />

### [What is Role Based Access Control (RBAC)](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)?


Role-Based Access Control (RBAC) is a security model that regulates access to resources based on predefined roles assigned to users. It allows administrators to assign permissions and access rights to roles, and then assign those roles to individual users. This approach simplifies access control management by granting permissions based on roles rather than assigning permissions directly to users.

### Share some an example of RBAC including all possible CRUD operations and correlating roles.

An example of RBAC could be a content management system (CMS) with the following roles and corresponding CRUD operations:

* Admin role: Can create, read, update, and delete (CRUD) all content.

* Editor role: Can create, read, update, and delete content, but not modify system settings.

* Author role: Can create and update content, but cannot delete or modify other users' content.

* Viewer role: Can only read content, without any modification or deletion permissions.

### What are the Benefits of RBAC?

* Enhanced security: RBAC ensures that users have the exact privileges they need and restricts unauthorized access.

* Simplified administration: It simplifies user management by assigning and managing permissions based on roles rather than individual users.

* Scalability: As organizations grow, RBAC allows for efficient management of user access rights without becoming cumbersome.

* Compliance: RBAC aids in meeting regulatory compliance requirements by ensuring appropriate access controls are in place.

* Auditability: RBAC enables tracking and auditing of user activities and access permissions, helping with security analysis and investigations.



### Compare and Contrast the following two Libraries and the following questions. Yes, they are similarly named.

#### [react-cookie library](https://www.npmjs.com/package/react-cookie)

#### [react-cookies component](https://www.npmjs.com/package/react-cookies)



#### Describe some react-cookie features.

react-cookie: The react-cookie library provides features for working with browser cookies in React applications. It allows you to set, retrieve, and delete cookies. You can also define cookie options like expiration time, domain, and secure flag. Additionally, it provides hooks and components to manage and interact with cookies in a React-friendly way.

#### Describe some react-cookies features.
The react-cookies library provides functionalities for working with cookies in React applications. It allows you to load, save, and remove cookies using a simple API.

Some key features of react-cookies include:

Loading Cookies: You can use the cookie.load(name) method to load the value of a specific cookie. It returns undefined if the cookie does not exist.
Saving Cookies: The cookie.save(name, value, options) method enables you to set a cookie. You provide the cookie name, value, and additional options such as path, expiration date, domain, and security settings.
Removing Cookies: The cookie.remove(name, options) method allows you to remove a cookie by providing its name and optional options like path, expiration date, and domain.
The library also includes additional methods such as loadAll() to load all available cookies and select([regex]) to find cookies that match a given regular expression.

### Which library would you prefer would you prefer? Why?

The react cookie library has more documentation and downloads, making it my preferred choice. 