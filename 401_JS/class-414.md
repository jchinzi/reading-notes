## Access Controls

* *Access Controls* are the selective restrictions of resources

  - In RESTful APIs, it is important to limit access to clients based on credentials

## Application Flow and Access Control

* Any constraints on access need to be handled on both the backend and the front end of the application stack

* Back End (API Layer)
  - Manage the login cycle with the front-end application
  - Maintain the User's database
  - Maintain roles for each user
  - Authenticate users (basic and bearer)
  - Create, manage, and apply Role Based Access Controls
  - Maintain and reference their capabilities, based on role
  - Restrict access to features based on capabilities

* Front End (Client Layer)
  - Initiate login process
  - Store login tokens as cookies
  - Manage login state & capabilities
  - Control physical & visual access to components based on RBAC (role-based access control) rules
  - Alter behaviors based on RBAC rules

## Role Based Access Control

* Roles dictate rights, and users are assigned roles (but users are not specifically assigned rights)
  - [User] => [Role] => [Rights]
  - This can greatly streamline access management (access of rights becomes systematic and repeatable)

* 5 Steps to Initial Implementation:

  1.  Inventory the system
  1.  Analyze the workforce and create Roles
  1.  Assign people to Roles
  1.  Never make one-off changes
  1.  Audit for ongoing efficiency

* Variations on RBAC:

  - *ACL (Access Control Lists)*:
    - defines access rights by a user or user group to specific objects (such as documents)

  - *ABAC (Attribute-based Access Control*:
    - aka Policy-based access control
    - Uses a variety of attributes to determine user access (such as department, time of day, type of access, etc)

  - Both options provide increased granularity of controls but also increase the effort required to maintain consistant access controls

## Reference Links:

[5 Steps to Simple Role-Based Access Control](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)

[Wikipedia: Role-based access control](https://en.wikipedia.org/wiki/Role-based_access_control)

[Video: Role Based Access Control](https://www.youtube.com/watch?v=C4NP8Eon3cA)



---

[Home](https://jchinzi.github.io/reading-notes/)